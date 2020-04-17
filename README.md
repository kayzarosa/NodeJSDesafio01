<h1 align="center">
    <img alt="Rocketseat GoStack" src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/bootcamp-header.png" width="200px" />
</h1>

## Rocketseat

# :rocket: Desafio 1: Conceitos do NodeJS
> Se divirta criando os seus repositórios.

## Versão

<a href="https://nodejs.org/pt/"> NodeJS 12.14.1 </a>

## Instalação

````sh
yarn
````

## Iniciar uma API

````sh
yarn dev
````

## Usando a API

Criar um novo repositório com método POST, chame uma URL http://localhost:3333/repositories/ e informe o corpo da requisição:

Corpo da requisição:

JSON

````sh
{
	"title": "Desafio 01",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
		"NodeJS",
		"React"
	]
}
````

Ele retorna todos os projetos cadastrados e o que acabou de ser cadastrado:

JSON

````sh
{
    "id": "b5fe2f8a-32c2-44a1-89ef-7d089d21481f",
    "title": "Desafio 01",
    "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
    "techs": [
        "NodeJS",
        "React"
    ],
    "likes": 0
}
````

Buscando todos os repositórios registrados, método GET, chame um URL http://localhost:3333/repositories/

Ele retorna todos os repositórios cadastrados:

JSON

````sh
[
    {
        "id": "f6b6e9de-bd64-4306-9ca7-b18c0a2551f4",
        "title": "Desafio 01",
        "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
        "techs": [
            "NodeJS alterando",
            "React alterando"
        ],
        "likes": 3
    },
    {
        "id": "89e52368-6fa9-4b57-8046-1b4ac569b9b9",
        "title": "Desafio 02",
        "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
        "techs": [
            "NodeJS",
            "React"
        ],
        "likes": 0
    }
]
````
Alterando um repositório cadastrado de acordo com o código informado, método PUT, chame um URL http://localhost:3333/repositories/ Código do repositório


````sh
http://localhost:3333/repositories/89e52368-6fa9-4b57-8046-1b4ac569b9b9
````

Corpo da requisição:

JSON
````sh
{
	"title": "Desafio 2",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
		"NodeJS"
	]
}
````

Ele retorna todos os repositórios registrados, in:

JSON

````sh
{
	"id": "89e52368-6fa9-4b57-8046-1b4ac569b9b9",
	"title": "Desafio 02",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
	    "NodeJS"
	],
	"likes": 0
}
````

Excluindo um repositório registrado de acordo com o código informado, método DELETE, chame um URL http://localhost:3333/repositories/ Código do repositório


````sh
http://localhost:3333/repositories/89e52368-6fa9-4b57-8046-1b4ac569b9b9
````

Ele retornou o código de sucesso:

````sh
200
````

Para dar like no repositório com método POST, chame uma URL http://localhost:3333/repositories/b5fe2f8a-32c2-44a1-89ef-7d089d21481f/like:

Ele retorna o repositório com o número de likes atribuidos a ele:

JSON

````sh
{
    "id": "b5fe2f8a-32c2-44a1-89ef-7d089d21481f",
    "title": "Desafio 01",
    "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
    "techs": [
        "NodeJS",
        "React"
    ],
    "likes": 5
}
````

Feito com ♥ by Kayza :wave:
