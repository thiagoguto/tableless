---
title: Angular 5 + UIKit 3
authors: Thiago Augusto
type: post
date: 2018-02-16
excerpt: Use o UIKit 3 na sua proxima aplicação
categories:
  - Artigos
  - Design
  - Código
  - JavaScript
  - Angular 5
  - UIKit 3
  - Tecnologia e Tendências
tags:
  - CSS
  - UX e Design
  - HTML
---
Hoje em dia o frameworks CSS passou a ser indispensável na criação de um projeto com um prazo curto.
Nesse artigo, vou mostrar como utilizar o UIKIT 3 dentro do seu projeto angular 5.

### Pre-requisitos:
Para realizar os passos contidos nesse tutorial, você vai precisar ter instalado:
- Nodejs
- Angular-cli

Para saber se você já tem esses programas instalados no seu computador, basta abrir o seu terminal, e digitar o seguintes comando:

	node -v 
	npm -v
	ng -v

### Instalação:
Depois de verificar que já temos o que precisamos, vamos iniciar um novo projeto, utilizando o compilador LESS para criar nossas folhas de estilo.
Navegue ate a pasta onde deseja criar o seu projeto e digite o seguinte comando:

	 ng new meuProjeto --style=less

Vou explicar esse comando antes de partir para as outras configurações.
	
	* ng new  → diz para o Angular-cli que vamos criar um projeto angular
	* meuProjeto → é o nome do projeto que será criado. O Angular-cli vai criar uma pasta 	com o nome do projeto e colocar todos os seus arquivos dentro dessa pasta.
	* --style=less → com esse comando dizemos ao Angular-cli que nosso padrão de folha de 	estilos é o LESS.
Depois que o Angular-cli terminar de rodar o comando teremos uma pasta com o nome do nosso projeto. Vamos entrar na pasta e configurar nossa instalação para utilizar folhas de estilo do UIKit 3.

	cd meuProjeto //entrar na pasta do projeto
	npm install uikit --save //instalar a biblioteca do UIKit 3 dentro do nosso projeto.  
  
### Configuração: 
  Depois de instalar a biblioteca uikit3 dentro do nosso projeto, o que precisamos agora é editar o arquivo de configuração do angular. Abra o arquivo  de configuração com seu editor de codigo preferido. Nesse tutorial utilizarei o Visual Studio Code.
	
	code .angular-cli.json

Encontre a seção  chamada styles, e adicione o caminho dos arquivos less do uikit. Seu arquivo deve ficar com algo parecido com isso.

"styles": [
	"../node_modules/uikit/src/less/uikit.theme.less”",
	"styles.less"
]

Agora vamos adicionar os arquivos js e icones, na seção scripts. Seu arquivo deve ficar com algo parecido com isso.

"scripts": [
	"../node_modules/uikit/dist/js/uikit.min.js",
	"../node_modules/uikit/dist/js/uikit-icons.min.js"
]
Salve e feche o arquivo.

### Rodando Seu Projeto:
Agora que ja configuramos nosso projeto so precisamos rodar o servidor.
  ng serve -o
Se tudo correu como deveria, você vera o arquivo de boas vindas do angular, com os estilos personalizados. Agora você pode configurar seu projeto utilizando as classes do UIKit 3.

Caso você não conheça o UIKit 3, segue o link para consulta.
https://getuikit.com/

Obrigado por ler esse artigo e até a próxima oportunidade.



  
  
