# manejo-solo-tomate-nodered

Painel Node-RED do projeto "Manejo do Solo e Monitoração da Lavoura de Tomate", da disciplina Instrumentação e Experimentação (IPRJ/UERJ, 2026).

O arquivo `flows.json` tem o fluxo completo do painel: a parte que recebe os dados do ESP32 pelo HiveMQ Cloud (MQTT) e a parte visual do dashboard.

## Requisitos

- Node-RED 4.1.8
- @flowfuse/node-red-dashboard 1.30.2

## Como usar

1. Instalar o @flowfuse/node-red-dashboard pelo Manage palette.
2. Importar o flows.json (menu > Import).
3. No nó "Servidor Hive", informar usuário e senha do broker (não estão no arquivo).
4. Fazer o Deploy e abrir http://127.0.0.1:1880/dashboard e http://127.0.0.1:1880 

Tópicos usados: tomate/leituras e tomate/estado.
