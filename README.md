# Cypress_and_cucumber
Projeto para testes com Cypress_and_cucumber com estrutura para page objects e elements

### Primeiros passos
* - 1.	Instalar Node.js: acesse o site oficial, baixe e instale a versão para seu computador. (link: https://nodejs.org/en/ )
* - 2.	Escolher uma IDE de JavaScript para programar: usaremos o VS Code neste tutorial. (link: https://code.visualstudio.com/download )
* - 3.	Instalar o Cypress > abra o terminal do VsCode e digite o comando abaixo:
####	npm install cypress:9.7.0
* - 4. Instalar o Cypress com Cucumber:

* I) Crie uma pasta onde ficarão os arquivos do seu projeto. Abra o terminal do windows e acesse essa mesma pasta com o seguinte comando:
cd /your/project/path
 
* II) Tendo acessado a pasta do projeto, execute o comando de instalação:
npm install --save-dev cypress cypress-cucumber-preprocessor
 
* III) Ainda dentro da pasta do seu projeto, execute o seguinte comando para que o Cypress termine de criar os arquivos locais:
####npx cypress@9.7.0 open

Na sequencia o cypress será aberto.

===================================

### Para testes manuais com o Cypress o comando é o ### npx cypress@9.7.0 open

### E para testes automáticos é o  ### npm test.


