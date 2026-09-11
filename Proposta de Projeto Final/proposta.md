# Plataformas de Hardware para Internet das Coisas
##### Docente: Luiz de França Afonso Ferreira Filho
##### Discente: Leandro Antony Batista Lemos

## Proposta de Projeto Final - HIoT:

# Estação de Monitoramento Agrícola com ESP32
### Propósito e problema
O projeto possui como propósito específico auxiliar no manejo de irrigação de hortas, vasos ou canteiros, resolvendo o problema comum de rega, a qual é feita de forma manual e sem critério algum, gerando desperdício de água, estresse hídrico por excesso ou falta de umidade. 
### Descrição da solução
A proposta consiste na construção de uma estação de monitoramento que medirá continuamente a umidade do solo, a temperatura e a umidade do ar, e a luminosidade do ambiente, usando um microcontrolador ESP32 conectado a um sensor de umidade do solo, um sensor DHT22 para temperatura e umidade do ar, e um sensor de luminosidade BH1750.
### Funcionamento e comunicação
O ESP32 faz leituras periódicas desses sensores e atrávés da conectividade Wi-Fi, enviaos dados coletaos pela internet para um back (via protocolo MQTT), que armazenará o histórico das medições. Tais dados serão exibidos em tempo real em um dashboard web, no qual será viável acompanahar a variação da umidade do solo e das demais variáveis de condições ambientais ao longo do dia, de forma remota e por qualquer dispositivo conectado à internet.
### Tarefa em tempo real
A tarefa em tempo real do sistema consiste em identificar de forma automática o momento em que a umidade do solo cai abaixo de um limiar mínimo definido e, a partir disso, realizar uma ação imediata como o acionamento de um relé conectado a uma bomba ou uma válvula solenoide, podendo até enviar uma notificação por bot de telegram se configurado para isso, avisando assim o responsável pela horta.
### Conclusão
Dessa forma o projeto combina o uso prático de um microcontrolador em uma aplicação IoT com comunicação externa via internet a uma interface de visualização remota entregando uma solução de utilidade real para o gerenciamento eficiente de rega em pequena escala.