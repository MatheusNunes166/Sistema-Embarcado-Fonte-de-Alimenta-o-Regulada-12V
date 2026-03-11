# Sistema-Embarcado-Fonte-de-Alimentação-Regulada-12V

Este repositório contém o projeto de uma fonte que converte tensão alternada da tomada em 12V contínuos e estáveis, ideal para alimentar Arduinos, sensores e outros circuitos eletrônicos. O circuito foi desenvolvido no Proteus 8 Professional e já inclui o layout da placa pronta para fabricação.

Funcionamento Resumido

A energia chega pelo conector J2 vinda de um transformador. A ponte de diodos BR1 retifica a corrente (organiza para um único sentido). O capacitor C1 de 1000uF filtra as oscilações, reduzindo o ripple. O regulador LM7812 mantém a saída fixa em exatos 12V, independente de pequenas variações na entrada. Os capacitores C2 e C3 de 100nF eliminam ruídos de alta frequência. O LED D1 com resistor R1 indica que a placa está energizada.

<img width="1091" height="238" alt="{D68EB3C4-B96D-466E-95E2-F06F7A61F20C}" src="https://github.com/user-attachments/assets/bd6f60f6-3ea4-49d4-95af-1650015cb724" />

A Placa

Dimensões: 80mm x 40mm. Camada única (Bottom Copper). Trilhas dimensionadas para a corrente necessária. Componentes organizados em fluxo lógico da entrada para a saída.

<img width="341" height="547" alt="{B790AD3A-9BF1-41E9-A485-D948191DB72E}" src="https://github.com/user-attachments/assets/ed4be6e7-b233-4760-b30e-82d7e8a16b90" />

<img width="327" height="487" alt="{37992ECA-9AEF-4D3A-A3D4-1DDCC4DB4FF1}" src="https://github.com/user-attachments/assets/6c48867f-d090-4bce-be98-9ff0bffedae7" />

<img width="281" height="447" alt="{097AF015-D189-454B-8187-9879278EE99C}" src="https://github.com/user-attachments/assets/4c31c433-c417-4d2a-9d31-c491c75915f9" />

Lista de Materiais

Componente	Referencia	Descrição	Qtd
Borne de Entrada	J2	Conector para transformador	1
Ponte Retificadora	BR1	Ponte de diodos 2W005G	1
Capacitor de Filtro	C1	Eletrolítico 1000uF / 25V	1
Capacitores	C2, C3	Cerâmico 100nF	2
Regulador	U1	CI L7812 (TO-220)	1
Resistor	R1	1kΩ	1
LED	D1	LED Vermelho 5mm	1
Borne de Saída	J1	Conector para carga 12V	1

| LED Indicador | D1 | LED Vermelho 5mm | 1 |
| Borne de Saída | J1 | Conector fêmea para carga (12V DC) | 1 |
