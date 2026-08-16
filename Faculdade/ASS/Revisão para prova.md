#ass

**KVM** é uma sigla que significa Kernel-based Virtual Machine e é uma tecnologia de virtualização de código aberto que permite que um único servidor físico execute múltiplas máquinas virtuais (VMs), cada uma com seu próprio sistema operacional. O **KVM** funciona integrando-se ao kernel do Linux, transformando-o num hypervisor.

**Hypervisor** é um software que permite que várias máquinas virtuais (VMs) sejam executadas em um único computador físico, atuando como ponte entre as VMs e o hardware subjacente, além de controlar e alocar recursos (como CPU, memória e armazenamento).

Formato **qcow2** é um formato de armazenamento de discos virtuais (imagens de disco), amplamente utilizado em virtualização, conhecido por sua eficiência e recursos avançados como compactação, snapshots e provisionamento fino.

**Kernel** é o núcleo de um sistema operacional, o componente central que atua como ponte entre o hardware e o software do computador, gerenciando recursos do sistema como memória, o processador, e os dispositivos de entrada e saída.

**ABI (Application Binary Interface)** é uma especificação que define como diferentes componentes de software, como programas, bibliotecas e o kernel, se counicam em nível binário.

Uma **Thread** é uma unidade de execução de um programa, ela representa um fluxo de controle independente dentro de um processo.

**Swapping** em sistemas operacionais é uma técnica de gerenciamento de memória que permite ao sistema mover processos da memória RAM para o disco rígido, essa técnica é usada para lidar com situações onde a memória RAM é insuficiente para abrigar todos os processos que precisam ser executados simultaneamente.

**Socket** basicamente se trata de um canal de comunicação que permite que dois processos troquem dados.

# Comandos Libvirt
O **Libvirt** é uma **API** e ferramenta de código aberto para gerenciar virtualização de plataformas, que permite interagir com diferentes tecnologias de virtualização como KVM, Xen, VMware ESXi e QEMU.
- virsh: é um utilitário de linha de comando utilizado para gerenciar máquinas virtuais (VMs) através da **API** **Libvirt**. Que permite criar, iniciar, interromper listar e interagir com VMs.
	- virsh shutdown <nome_vm>: desliga uma VM específica utilizando seu nome
	- virsh list --all: lista todas as VMs
	- virsh start <nome_vm>: inicia uma VM específica utilizando seu nome
	- virsh dombklist <nome_vm>: lista os dispositivos de uma VM em bloco
	- virsh domifaddr <nome_vm>: faz uma lista de endereços MAP e IP de uma VM
	- virsh dumpxml --inatctive <nome_vm> > <nome.xml>: salva as informações de uma VM em um arquivo XML
	- virsh define <nome.xml>: define novamente uma VM a partir de um arquivo XML
- virt-top: monitoramento de desempenho de VMs
- qemu-img: manipulação de discos virtuais (principalmente no formato qcow2)
- qemu-nbd: permite conectar discos virtuais ao hospedeiros (host)

# Conhecendo o sistema
- sudo -i: acessa o usuário root da máquina
- uname -a: apresenta ao usuário o Kernel e ABI (application binary interface)
- timedatectl: apresenta o fuso horário, com data e hora local e outras informações sobre o fuso horário
- lsblk: este comando serve para listar os informações sobre dispositivos de bloco do sistema, como discos rígidos, SSDs, partições e dispositivos removíveis.
- df -hT: verificaos pontos de montagem e o espaço em disco
- lscpu: usado para verificar CPU(s) e Thread(s)
- free -m: o comando free mostra a quantidade de memória livre e usada no sistema
- uptime: apresenta quanto tempo o computador está ligado, quantos usuários tem logados e outras informações
- top: usado para monitorar o desempenho do sistema em tempo real, mostrando informações sobre processos em execução como uso de CPU, memória e outras métricas.
- iostat -m 5: esse comando serve para exibir estatísticas de entrada/saída do sistema, especialmente focando no desempenho de discos e partições
- ifstat -b 5: exibe estatísticas da interface de rede, como tráfego de entrada e saída, erros e outros indicadores de desempenho.

# Hierarquia de diretórios do GNU/Linux
* /
	* bin/: esta pasta contém os programas básicos do SO (exemplos: ls, cp)
	* dev/: arquivos de dispositivos (geralmente para I/O)
	* etc/:esta pasta contém arquivos de configurações (geralmente modificáveis apenas pelo root)
	* usr/: contém a maior parte dos programas e bibliotecas instalados no SO
		* bin/
		* man/
		* lib/
		* local/
		* sbin/
		* share/
	* home/: home de usuários (desktop no windows)
	* lib/: contém arquivos de bibliotecas básicas do SO (como a .so)
	* sbin/: possui programas básicos geralmente usados pelo root
	* tmp/: arquivos temporários que podem ser apagados ao término de um processo ou na reinicialização
	* var/: possui arquivos de log (de bancos de dados e etc)
		* lob/
		* tmp/

# GRUB: Grand Unified Boot Loader 
Um dos gerenciadores de inicialização usados no GNU/Linux (boot loader), ele permite selecionar diferentes versões do kernel, incluindo parâmetros de inicialização. Opcionalmente o GRUB faz a carga do initramfs (initrd) usado para auxiliar o kernel na inicialização, ele pode também carregar outros SOs (Windows) além do GNU/Linux (chainloader).
O GRUB é carregado pela BIOS ou UEFI do computador, ele possui o seu próprio kernel, com linguagem, módulos e comandos próprios.
Arquivos/diretórios de configuração:
- /boot/grub/config.cfg: arquivo usado na inicialização, esse arquivo é gerado automaticamente através do grub-mkconfig
- /etc/default/grub e grub.d/: são variáveis e parâmetros do grub usados pelo grub-mkconfig para gerar o arquivo config.cfg
- /etc/grub.d: scripts usados pelo grub-mkconfig para compor o cabeçalho e itens de menu do config.cfg

## Passos de inicialização do GRUB
1. A BIOS ou o firmware UEFI inicializa o hardware e buscam pelo código de boot através da ordem de inicialização (dispositivos, rede e etc)
2. Encontrado o código de boot, a BIOS/firmware carrega e executa-o
3. O núcleo (pequeno kernel) do GRUB é carregado
4. O núcleo do GRUB entra em execução, passando a ter acesso aos discos e sistemas de arquivos
5. O GRUB identifica a partição de boot e carrega o dispositivo de configurações.
	1. Variável prefix do ambiente GRUB contém a localização do arquivo grub.cfg, módulos e demais arquivos auxiliares
6. O GRUB apresenta o menu de opções de sistemas operacionais ao usuário

# Systemd
Mais avançado que seus predecessores (System V e Upstart), possuindo paralelismo de inicialização, uma abordagem top-down e controle de status de processos.
**Unit** é qualquer coisa que precisa ser iniciada no SO e controlada pelo systemd, existem os seguintes tipos de units:
- Target Units: agrupamento de outras Units, a inicialização de um target implica na inicialização de todas as Units vinculadas a ele.
- Service Units: controla um processo ou serviço
- Socket Units: Sockets ?? (geralmente de rede)
- Mount Units: representação dos pontos de montagem no systemd

![[Pasted image 20250518200817.png]]

## Comandos Systemd
- systemctl get-default: para verificar qual é o default.target
- systemctl set-default multi-user.target: para modificar o default.target para o multi-user.target (requer reboot)
- system.unit=multi-user.target: é usado para selecionar um target durante o boot (GRUB), adicionando o parâmetro na inicialização do kernel.
- systemctl list-units --type target: usado para listar todos os targets registrados
- systemctl list-dependencies: para listar a dependência entre targets e damais Units