# SentinelaOrbital – Sistema de Alerta Climático Comunitário

## Descrição do Projeto

O SentinelaOrbital é um sistema de monitoramento climático baseado em Arduino, desenvolvido para simulação em Tinkercad/Wokwi, que integra sensores locais e atuadores para emitir alertas visuais e sonoros em situações de risco climático.

O projeto busca oferecer uma solução simples e acessível para comunidades vulneráveis, transformando dados em ação preventiva.

---

## Objetivo da Solução

- Monitorar temperatura, chuva e luminosidade em tempo real.
- Classificar o clima em bom, médio, ruim e catástrofe iminente.
- Emitir alertas visuais (LEDs) e sonoros (buzzer em modo sirene) em caso de risco extremo.
- Exibir informações de forma clara em um LCD 16x2 I2C e no Monitor Serial.
- Demonstrar como tecnologias de baixo custo podem auxiliar comunidades vulneráveis.

---

## Componentes Utilizados

- Arduino Uno
- Sensor TMP36 (temperatura)
- Potenciômetro (simulação de chuva)
- Fotoresistor (LDR)
- LCD 16x2 I2C
- LED Verde
- LED Amarelo
- LED Laranja
- LED Vermelho
- Buzzer Piezo
- Resistores de 220Ω
- Resistor de 10kΩ
- Protoboard
- Jumpers

---

## Funcionamento

### Coleta de Dados

Os sensores realizam a leitura das condições ambientais:

- TMP36 → temperatura entre -5°C e 45°C.
- Potenciômetro → intensidade da chuva de 0% a 100%.
- LDR → nível de luminosidade.

### Processamento

O Arduino analisa os dados recebidos e classifica a situação em quatro níveis:

- Verde → Bom
- Amarelo → Médio
- Laranja → Ruim
- Vermelho → Catástrofe Iminente

### Alertas

As informações são apresentadas através de:

- LCD 16x2 I2C
- Monitor Serial
- LEDs indicadores
- Buzzer com alerta sonoro

---

## Estrutura do Circuito

| Componente | Porta |
|------------|--------|
| TMP36 | A0 |
| Potenciômetro | A1 |
| LDR | A2 |
| LCD I2C SDA | A3 |
| LCD I2C SCL | A4 |
| LED Verde | 9 |
| LED Amarelo | 10 |
| LED Laranja | 11 |
| LED Vermelho | 12 |
| Buzzer | 13 |

---

## Instruções de Execução

1. Abra o projeto no Tinkercad ou Wokwi.
2. Carregue o código no Arduino.
3. Inicie a simulação.
4. Ajuste o potenciômetro para simular chuva.
5. Modifique a luminosidade do LDR.
6. Observe o comportamento dos LEDs e do buzzer.
7. Acompanhe os dados exibidos no LCD e no Monitor Serial.

---

## Aplicação Prática

- Auxílio a comunidades rurais e ribeirinhas.
- Monitoramento de riscos relacionados a enchentes e eventos climáticos extremos.
- Funcionamento independente de conexão com a internet.
- Possibilidade de integração futura com soluções de Edge Computing e monitoramento remoto.

---

## Tecnologias Utilizadas

- Arduino Uno
- Linguagem C/C++
- Tinkercad
- Sensores Analógicos

---

## Integrantes

- Gabriel Freitas da Silva Carvalho — RM 570881
- Erick Martins Picolo — RM 572892
- Guilherme Marcon Dantas — RM 572171
- Luiz Felipe Cardoso de Oliveira — RM 569782

---

## Disciplina

Projeto desenvolvido para a disciplina **EDGE COMPUTING & COMPUTER SYSTEMS** da FIAP.

---

## Repositório e Simulação

- Simulação Tinkercad/Wokwi: https://www.tinkercad.com/things/jhmfi8btEm2-sentinelaorbital?sharecode=uRK4noRkB0Ud4ao_gNv5gKvGQ0gfekJaIeS270rwrxc
- Link do vídeo explicativo: https://www.youtube.com/watch?v=lAFlxzMOKls
- Vídeo demonstrativo: inserir link.
