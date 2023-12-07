Irrigação Inteligente com Arduino

Este repositório contém o código fonte e informações relacionadas a um projeto de irrigação inteligente utilizando Arduino. O projeto é desenvolvido para monitorar a temperatura do solo e controlar um sistema de irrigação com base nessa leitura.

*Especificações Técnicas*

Componentes Utilizados
Arduino Uno: Placa de desenvolvimento baseada em microcontrolador ATmega328.

Sensor de Temperatura: Utiliza um pino analógico (A1) para medir a temperatura do solo.

Display LCD: Conectado aos pinos digitais para exibir informações sobre a temperatura e o estado do sistema.

Motor da Bomba d'Água: Controlado pelos pinos digitais 10 e 11.

LEDs e Campainha: Utilizados para indicar o estado do sistema.

*Bibliotecas*

LiquidCrystal: Utilizada para controlar o display LCD.

Conversão de Temperatura
A temperatura é medida através da leitura analógica do sensor conectado ao pino A1. A conversão da leitura para temperatura em graus Celsius é feita da seguinte maneira:

TemperatureCelsius
=
(
Voltage
−
0.5
)
×
100.0
TemperatureCelsius=(Voltage−0.5)×100.0

Onde 
Voltage
=
analogRead
(
temp
)
×
5.0
1023.0
Voltage=analogRead(temp)× 
1023.0
5.0
​
 .

*Configuração do Projeto*

Conexões Físicas:

Conecte o sensor de temperatura ao pino analógico A1.
Conecte o display LCD aos pinos digitais 2 a 7.
Conecte o motor da bomba d'água aos pinos digitais 10 e 11.
Conecte LEDs (vermelho e verde) aos pinos digitais 12 e 9.
Conecte a campainha ao pino digital 8.
Upload do Código:

Utilize a IDE do Arduino para abrir o arquivo Circuito-de-irrigação-com-arduino.ino.
Selecione o tipo de placa (Arduino Uno) e a porta correta.
Faça o upload do código para o Arduino.

Funcionamento do Sistema:

O sistema monitora continuamente a temperatura do solo. Se a temperatura exceder 50 graus Celsius, o sistema é ativado, indicando a necessidade de irrigação. Os LEDs e a campainha sinalizam visual e auditivamente o estado do sistema.

Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) ou propor melhorias através de pull requests.

Licença
Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
