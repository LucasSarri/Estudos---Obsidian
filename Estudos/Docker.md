# Como criar um container docker
Irei realizar a criação de um container docker para apresentar de maneira simples de criar um container docker, com um exemplo e explicação. Execute o comando a seguir no terminal:

```terminal
docker run --name teste-postgres -e "POSTGRES_PASSWORD=teste-123" -p 5433:5432 -d postgres
```

Onde nesse comando:
- O atributo **--name** especifica o nome do container a ser gerado (No exemplo a cima é teste-postgres)
- O atributo **-e** define as variáveis ambiente, no caso é **POSTGRES_PASSWORD** que é a senha do usuário administrador (**postgres**)
- O atributo **-p** indica a porta em que se dará a comunicação com o **PostgreSQL**, no exemplo é a **5433**, a qual será mapeada para a porta padrão **5432** do **SGBD** dentro do container
- O atributo **-d** indica que o container em questão será executado como um serviço em background
- Por fim o atributo **postgres** no final indica qual é a imagem que será utilizada para a geração do container.
***
# Listando containers docker
Para se listar todos os containers do docker, utilize o comando a seguir:

```terminal
docker container ls -a
```

***
# Excluindo containers no docker
Para se excluir um container docker específico é preciso pegar o id do mesmo, através da listagem, informando o comando a seguir:

```terminal
docker container rm <container ID> 
```