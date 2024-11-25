# Trabalho de Conclusão de Curso Análise de Desenvolvimento de Sistemas - Fatec Ipiranga

## Grupo:

* Anderson Iwamizu - 2040482223037
* Pedro Luiz da Silva Domiêncio - 2040482213025
* Rosana Della Bruna - 2040482213016
* Vanessa Souza da Silva - 2040482213004


## Dina Filmes:

![Logo da Dina Filmes.](./imagens/logo.png "Logo da Dina Filmes.")

Dina Filmes é uma aplicação web em que os usuários poderão criar listas de filmes (favoritos, à assistir e já assistidos) e também poderão interagir entre si através de comentários. Além disso, o usuário administrador poderá fazer a moderação dos comentários. 

O sistema foi desenvolvido em Angular (frontend) e Spring Boot (backend), com bando de dados em MySQL.

## Passos para executar o projeto Dina Filmes:

* Fazer um clone deste repositório no computador local
* Entrar no MySQL Workbench (senha nos computadores da FATEC Ipiranga: 123456) e digitar o seguinte comando:
`create database dina`
* Entrar com o VS Code na pasta Backend (necessário ter o JDK instalado) e inserir a chave do servidor de e-mail e a senha do MySQL Workbench da Fatec Ipiranga no arquivo application.properties:
```
spring.datasource.password=123456 // aqui é senha do MySQL Workbench da Fatec Ipiranga
spring.mail.password=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 // aqui é a nossa chave privada do servidor de e-mail (ficará exposta aqui temporariamente por conta da apresentação do TCC)
``` 
* Procurar o arquivo BackendApplication.java, clicar com o botão direito e escolher a opção Run Java para executar o backend.
* Na pasta clonada pegar o arquivo seed.sql que contém os dados iniciais do banco de dados e executar no MySQL Workbench (esse passo deve ser após o backend estar sendo executado).
* Entrar com o VS Code na pasta Frontend. Abrir um terminal com bash ou cmd (não pode ser PowerShell) e digitar o seguinte comando para instalação do angular:
`npm install`
* Para executar o frontend após a instalação, digitar o seguinte comando:
`npm start`

* Acessar o [http://localhost:4200/](http://localhost:4200/) pelo navegador (Chrome ou Edge)

## Notas

É necessário que as seguintes portas estajam livres para que o projeto seja executado:

* API: 8081
* Frontend: 4200
* Mysql: 3306