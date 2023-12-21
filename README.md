# 🌐 Consumindo e tratando dados de uma API

Para a realização desse projeto, utilizei a biblioteca, do Node.js, chamada JSON Server que simula uma API RESTful a partir de um arquivo JSON. 

### 👣 Passo 1 : Instalação do JSON Server
Para instalação da biblioteca usei o comando:

    npm install -g json-server

Isso fará com que o JSON Server seja instalado globalmente em seu sistema, e você estará pronto para utilizá-lo em qualquer projeto.

### 👣 Passo 2: Preparando o arquivo JSON

O arquivo JSON videos.json, que está dentro da pasta backend do projeto ```Vidflow\backend\videos.json```, servirá como a fonte de dados para o JSON Server simular uma ```API fake```.

### 👣 Passo 3: Inicialização do JSON Server

Execute o seguinte comando para iniciar o JSON Server e usá-lo com o arquivo videos.json:

    json-server --watch backend/videos.json
Obs.:

    --watch: Este é um dos argumentos que você pode fornecer opcionalmente ao comando JSON Server. 
    A opção --watch é usada para especificar que o servidor deve ficar "observando" 
    um arquivo JSON específico para quaisquer mudanças. 
    Isso significa que se você modificar o arquivo videos.json, 
    o JSON Server automaticamente recarregará os dados para refletir as alterações.

O JSON Server será iniciado e começará a servir uma `API REST` falsa com base nos dados do arquivo `videos.json`, o que vai nos permitir o consumo dos dados para o VidFlow.
