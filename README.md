# cypress_and_cucumber
cypress_and_cucumber with page objects

![image](https://user-images.githubusercontent.com/33332202/234431217-6ad511d7-f88d-403a-beb4-0c959a0a05c1.png)
![image](https://user-images.githubusercontent.com/33332202/234431378-2555b580-1555-4859-9438-e62cd41796b8.png)


Etapas para criar um projeto de teste com BDD
![image](https://user-images.githubusercontent.com/33332202/234430711-817e5b4d-f8fa-4108-9391-7bf90b3582cd.png)
npm install cucumber
npm install cypress@9.7.0 cypress-cucumber-preprocessor
npm init –y

Configurar cypress-cucumber-preprocessor: 

1. Adicione ao arquivo cypress/plugins/index.js o seguinte script:


    const cucumber = require(‘cypress-cucumber-preprocessor’).default

    module.exports = (on, config) => { On(‘file:preprocessor’, cucumber()) } 


2. Configurar pasta dos arquivos de teste editando o arquivo package.json:

{

    "scripts": {   "test": cypress@9.7.0 run --browser chrome },
    
    "cypress-cucumber-preprocessor": {  "step_definitions": "cypress/support/steps“ },
    
    "dependencies": {
    
        "cypress": "^9.7.0",
        
        "cypress-cucumber-preprocessor": "^4.3.1"
        
    }
}


Execução manual: npx cypress open
Execução autom: npm test

Instalar xpath
npm install -D cypress-xpath

No arquivo index.js da pasta support adicionar:
require('cypress-xpath');

