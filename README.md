# GS2025_Edge

Integrantes: 

Filip Arnhold - RM559294
Matheus Ricardo - RM560099
Marcos Azuma - RM559883

Descrição do Projeto:

O SIMURB (Simulador Urbano de Riscos de Enchentes) é uma solução que visa monitorar em tempo real o nível de água em áreas de risco, utilizando sensores conectados a um microcontrolador Arduino Uno.
A proposta é criar um sistema que, através de processamento local, seja capaz de identificar situações de risco de enchente e alertar autoridades e a população.
O sistema atua de forma preventiva, processando dados diretamente no Arduino, acendendo LEDs indicadores de risco e enviando informações para um broker MQTT, simulando a comunicação para um dashboard de monitoramento.

Solução Proposta:

Cidades sofrem com enchentes recorrentes devido à ausência de sistemas de monitoramento eficazes.
O SIMURB oferece uma solução de baixo custo, capaz de fornecer dados em tempo real sobre o nível da água, auxiliando a tomada de decisão antes que a enchente aconteça.
Por isso nosso objetivo é:
- Medir o nível da água em bueiros, rios e pontos críticos.
- Processar os dados localmente no Arduino.
- Indicar o nível de risco através de LEDs.
- Simular envio de dados para um broker MQTT, representando a integração com dashboards e sistemas de alerta.

Impacto da Solução:

- Aumenta a velocidade de resposta em situações de risco de enchente.
- Solução de baixo custo, replicável e escalável.
- Ajuda na tomada de decisão de autoridades e moradores em situações de risco.
- Promove cidades mais inteligentes e resilientes.

Componentes Utilizados:

| Componente                      | Função                                |
| ------------------------------- | ------------------------------------- |
| Arduino Uno                     | Microcontrolador principal            |
| Sensor Ultrassônico HC-SR04     | Medição do nível da água              |
| LEDs (Verde, Amarelo, Vermelho) | Indicadores visuais de status         |
| Buzzer                          | Alarme sonoro para alerta crítico     |
| Comunicação Serial (TX/RX)      | Simula envio de dados                 |

Funcionamento do Sistema:

1. O sensor ultrassônico mede o nível da água (em cm).
2. O Arduino processa localmente esse dado, sem depender da nuvem.
3. Dependendo do nível medido, aciona:
    - LED Verde: Nível seguro.
    - LED Amarelo: Atenção.
    - LED Vermelho + Buzzer: Alerta de enchente.
4. O Arduino simula o envio dos dados via porta Serial, que pode ser lida por um dashboard.

Link da simulação: https://wokwi.com/projects/432931740007068673

Como executar o projeto:

1. Acesse o projeto no Wokwi.
2. Observe a simulação dos sensores de nível de água.
3. Verifique a sinalização dos LEDs e do Buzzer de acordo com os valores medidos.
4. Acompanhe os dados sendo enviados pela porta Serial.



