# Projeto: Fonte de Alimentação Linear Regulada 12V DC

Esse repositório guarda o projeto completo de uma fonte de alimentação linear de 12V, que desenvolvi como parte de um protótipo para um carregador ou alimentador estável. A ideia aqui era criar algo simples, confiável e seguro — ideal para alimentar pequenos circuitos ou projetos eletrônicos que exigem uma tensão bem comportada.

## Descrição do Projeto

O objetivo deste circuito é converter a tensão alternada (AC) proveniente de um transformador em uma tensão contínua (DC) estável de **12 Volts**. Essa estabilidade é fundamental para alimentar microcontroladores, sensores e circuitos de automação sem variações que possam causar erros de leitura ou danos aos componentes.



<img width="1091" height="238" alt="{D68EB3C4-B96D-466E-95E2-F06F7A61F20C}" src="https://github.com/user-attachments/assets/bd6f60f6-3ea4-49d4-95af-1650015cb724" />


## Funcionamento Etapa por Etapa

1. **Entrada (AC):** O conector **J2** recebe a tensão do secundário de um transformador.
2. **Retificação:** A ponte de diodos **BR1** realiza a retificação em onda completa, garantindo que a corrente flua em apenas um sentido.
3. **Filtragem Primária:** O capacitor eletrolítico **C1 (1000uF)** atua como um reservatório de carga, suavizando a "onda" da tensão e reduzindo o *ripple*.
4. **Regulação:** O U1 **7812** (Regulador Linear) garante que, independentemente de oscilações na entrada, a saída permaneça em exatos 12V.
5. **Estabilização e Ruído:** Os capacitores **C2 e C3 (100nF)** filtram ruídos de alta frequência para uma saída mais "limpa".
6. **Sinalização:** O conjunto **R1 + D1 (LED)** indica visualmente que a placa está energizada e regulada.
7. **Saída (DC):** O conector J1 é o terminal de saída do projeto. É através dele que você conecta o dispositivo que deseja carregar ou alimentar com os 12V DC estabilizados.

## Especificações da PCB

O layout da placa de circuito impresso foi desenvolvido respeitando as seguintes normas técnicas:

* **Dimensões da Placa:** 80mm x 40mm (Formato Retangular).
* **Camada de Trilha:** Single Layer (**Bottom Copper** - Cor Azul).
* **Organização:** Componentes alinhados em fluxo lógico (Entrada -> Processamento -> Saída).

<img width="341" height="547" alt="{B790AD3A-9BF1-41E9-A485-D948191DB72E}" src="https://github.com/user-attachments/assets/ed4be6e7-b233-4760-b30e-82d7e8a16b90" />

<img width="336" height="569" alt="{E1B34C44-3F3F-489E-845E-62EF6CADCB0A}" src="https://github.com/user-attachments/assets/c64dca8a-7f56-4661-b3d7-5ac9cff3c318" />

<img width="331" height="604" alt="{89170E42-59EC-46EA-B7F0-CDF43A863870}" src="https://github.com/user-attachments/assets/49fbe13c-4347-4cb3-8b68-b57339ad7faf" />


## Lista de Materiais (BOM)

| Componente | Referência | Descrição Técnica | Qtd |
| :--- | :--- | :--- | :--- |
| Borne de Entrada | J2 | Conector macho para secundário de transformador | 1 |
| Ponte Retificadora | BR1 | Ponte de diodos 2W005G | 1 |
| Capacitor de Filtro | C1 | Eletrolítico 1000uF / 25V | 1 |
| Capacitores de Desacoplamento | C2, C3 | Cerâmico 100nF | 2 |
| Regulador de Tensão | U1 | CI L7812 (Encapsulamento TO-220) | 1 |
| Resistor | R1 | 1kΩ (Limitador de corrente do LED) | 1 |
| LED Indicador | D1 | LED Vermelho 5mm | 1 |
| Borne de Saída | J1 | Conector fêmea para carga (12V DC) | 1 |
