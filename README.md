# monitoramento_GPS_aula16_maloca

### Sistema de Rastreamento de Ambulância em Tempo Real com ESP32 e GPS

### Objetivo

O objetivo deste projeto é monitorar, em tempo real, a localização de uma ambulância utilizando um ESP32 e um módulo GPS NEO-6M. Os dados de latitude e longitude são enviados para um servidor web, que exibe a rota percorrida em um mapa interativo, permitindo um acompanhamento preciso do deslocamento do veículo.

O código do 'server.js' está no arquivo server.js

O código do ESP32 para o Arduino está no arquivo _arduino

### Materiais Utilizados
- 1x ESP32
- 1x Módulo GPS NEO-6M
- 1x Cabo micro-USB
- Jumpers para conexão
- Acesso à internet via Wi-Fi
- Plataforma Glitch para hospedagem do servidor

### Configuração do ESP32
1. Instale a IDE Arduino (caso ainda não tenha).
2. Instale a biblioteca TinyGPS++ na IDE Arduino.
3. Carregue o código atualizado no ESP32.
4. No código do ESP32, configure a rede Wi-Fi e a URL do servidor.
5. Abra o Monitor Serial para verificar se os dados do GPS estão sendo recebidos corretamente.

### Configuração do Servidor Web
Criação do servidor no Glitch:
Acesse Glitch e crie uma conta.
Crie um novo projeto Node.js.
Acesse a aba server.js, localizado na parte inferior esquerda da tela.
Substitua o código padrão pelo código do servidor fornecido.

### Instalação das dependências:
- No terminal do Glitch, localizado na parte inferior da tela, execute o comando:
- npm install express
- O servidor será iniciado automaticamente.

### Configuração no ESP32:
- Copie a URL do projeto no Glitch.
- Substitua essa URL no código do ESP32 para que os dados sejam enviados corretamente.

### Visualização da localização:
* Acesse o comando Preview e clique em Open Preview Pane ou Preview in a new window. Localizado na parte inferior da tela, (Ícone Lupa), para visualizar o mapa.

### Uso do Sistema
1. Ligue o ESP32 com o módulo GPS conectado.
2. Aguarde a conexão Wi-Fi ser estabelecida.
3. O ESP32 enviará periodicamente as coordenadas GPS para o servidor.
4. No navegador, acesse o servidor para visualizar a localização e a rota da ambulância
em tempo real.
