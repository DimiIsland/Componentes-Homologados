# Componentes Homologados
O objetivo deste repositório é manter um histórico organizado de componentes homologados, a maioria já utilizados em diversos projetos por mim e outros vistos em outros projetos. Então devido à produção em grande quantidade da maioria desses componentes em diversos projetos, estou colocando-os numa lista de componentes testados e homologados. Além de conter algumas dicas úteis ao dimensionar diversos componentes para o seu projeto.

# Lista de componentes

### Resistores
•	Você pode comprá-los em kits com todos os valores de série, mas os valores mais comuns de 1/4 Watts, 5% ou 1% são:

•	10R - Para limitar a corrente na saída de Op.Amps.

•	100R - Para limitar a corrente nas entradas.

•	330R - Resistor para coletor/emissor.

•	390R - Resistor para coletor/emissor.

•	470R - Resistor para coletor/emissor, forte pull-up para linhas I2C. E porque limita a corrente a aproximadamente ~1mA em 5V. 

•	560R - Resistor para coletor/emissor, forte pull-up para linhas I2C.

•	1K - Baixa corrente/baixo brilho para Led’s de qualquer cor, divisores de tensão, proteção de entradas, se for necessário um forte pull-up.

•	1.2K - Divisores de tensão.

•	1.5K - Divisores de tensão.

•	2.2K - Divisores de tensão.

•	3.3K - Divisores de tensão.

•	3.9K - Divisores de tensão.

•	4.7K -Divisores de tensão. Um valor médio que com 10K divide um 5V em ~3.3V,  bom para microcontroladores e entradas de recepção.

•	10K - Pull-ups/Pull-downs, resistores para coletor.

•	22K - Pull-ups/Pull-downs, pull-ups de pino reset em microcontroladores.

•	100K até 2M7 - Controle de ganho em OpAmps e amplificadores discretos, pull-downs em circuitos analógicos...

•	Nota: Muitas dessas informações de aplicação de resistores, vêm de "Kit Njay de Resistências 1/4W" e é usado com permissão.

### Capacitores
•	Os valores mais comuns são:

•	10 a 33pf – Usado 2 de mesmo valor com cristais osciladores em microcontroladores, ver datasheet do microcontrolador para recomendação de valores conforme frequência do cristal.

•	100nF – Filtrar ruídos genéricos.

•	4.7uF - Também utilizado como capacitor de bypass em paralelo com 100nF.

•	10uF – Próximo à alimentação de CIs, muito comum em smd.

•	100uF - Polarizado, para filtragem, próximo ao regulador de tensão.

•	1000uF - Polarizado, para suavizar a ondulação nas fontes de alimentação da rede.

•	2200uF - Polarizado, para suavizar a ondulação nas fontes de alimentação da rede.

### Indutores
•	Indutores Cilíndricos:

•	3uH a 1mH : Dimensionar para o dobro da corrente nominal do circuito, pois quando aquecem perdem suas propriedades, também dimensionar de acordo com a frequência de trabalho usada.

•	Mais detalhes:

•	https://embarcados.com.br/indutores/

•	Como fabricar seu Indutor caseiro:

•	https://www.youtube.com/watch?v=awyLYgu6ODM

### Leds
•	Muitas cores: vermelho, amarelo, verde, laranja, azul, branco, infravermelho, Ultravioleta (não muito comum), Led’s RGB.

•	Sugiro usar led’s de alto brilho (2500 a 7000 milicandelas –mcd de 3 ou 5mm), pois mesmo com um resistor alto (~100K) eles ascendem bem, consumindo correntes menores que 1mA do circuito.

•	Exemplo: Resistor 100 K e led 3000 mcd junto ao pino Rx do Microcontrolador de 5V, consome 30uA e não interfere na recepção de sinais. Em 3V3 pode ser usado um de 39K, 43K ou 47K.

### Diodos Retificadores
•	1N4001 até 1N4007 - Diodos retificadores, 1 A, (1 - 50V, 2 - 100V, 3 - 200V, 4 - 400V, 5 - 600V, 6 - 800V, 7 - 1000V).

•	1N4937 - Diodo rápido 600V 1A pth

•	1N5406 - Diodo retificador 3A 600V pth 

•	10A10 - Diodo pth 10A 1000V

•	MUR820 - Diodo encapsulamento TO-220 8A 200V Ultra rápido ( usado no secundário de fontes chaveadas com dissipadores).

### Diodos de Sinal
•	1N4148 - Diodo de sinal, 100V, 200mA. Nota: Em baixas tensões 1N5917/8/9 são equivalentes a 1N4148, 1N400x.

•	1L4148 – Diodo de sinal 100V, 200mA, smd 

### Diodos Zener
•	BZX79B3V3 - Diodo Zener, 3.3V, 1/2W, 2%.

•	BZX79B5V1 - Diodo Zener, 5.1V, 1/2W, 2%.

•	TZX12C - Diodo Zener, 12V, 1/2W, 2%.

•	CDBV3-40S-G - Proteção de entrada - diodos série, 40V, 200mA.

### Diodos Zener Ajustáveis
•	TL431ACZ - Referência de tensão, tensão de saída ajustável de 2,5 a 36 V, dissipador de 1 a 100mA, precisão de tensão de 1% e 2%.

### Diodos Schottky
•	1N5817 - Diodo Schottky, 20V, 1A, Comutação rápida.

•	1N5819 - Schottky Diodes & Rectifiers 1A, 40V, comutação rápida.

•	SS14 – Schottky 1A 40V

•	SS24 – Schottky 2A 40V

•	SS34 - Schottky Diodes & Rectifiers 3A 40V

•	1N5822 - Pode ser usado como uma grande gama VariCAP, Schottky diodo, 40V, 3A.

•	BAT85S - Diodo Schottky, 30V, 200mA. Equivalente a BAT54.

### Diodo Supressor de Tensão
•	P6KE6.8A - DO-15, 175C, 600W, Unidirecional, pth

•	P6KE6.8CA - 5.8Vr 600W 57A 5% Bidirecional, pth

•	P6KE33A -  600W, 33V, 5%, Unidirectional, pth

•	P6KE33CA -  600W, 33V, 5%, Bidirecional, pth

•	SMBJ5.0A - 600W 5V 5% Unidirecional smd

•	SMBJ5.0CA 600W 5V 5% Bidirecional smd

•	SMBJ26A 26V 600W Unidirecional smd

•	SMBJ26CA 26V 600W bidirecional smd

•	SMCJ5.0CA - 5V 1500W bidirecional, DO-214 smd

•	SMCJ26CA - 30.4V, 1500W, bidirecional, DO-214 smd

### Diac
•	DB3 -  DO-35, 28V...36V, 2A

### Transistores BJT
•	BC547 - BJT, npn, ruído figura 2 dB, 50V, 100mA, largura de banda 300MHz, 500mW.
Terminando com x para cada intervalo beta: A - 110 a 220, B - 200 a 450, C - 420 a 800.

•	BC557 - BJT, pnp, ruído figura 2 dB, -50V, -100mA, largura de banda 150MHz, 500mW, par complementar de BC547.
Terminando com x para cada intervalo beta: A - 110 a 220, B - 200 a 450, C - 420 a 800.

•	BC549C - BJT, baixo ruído, npn, beta alto 420 a 800, ruído figura 1.2 dB, 30V, 100mA, largura de banda 300MHz, 500mW.
Terminando com x para cada intervalo beta: A - 110 a 220, B - 200 a 450, C - 420 a 800.

•	BC559C - BJT, baixo ruído, pnp, beta 420 a 800, baixo ruído, ruído figura 1.2 dB, -30V, -100mA, largura de banda 150MHz, 500mW, par complementar de BC549C.
Terminando com x para cada intervalo beta: A - 110 a 220, B - 200 a 450, C - 420 a 800.

•	BC817 – NPN , 800mA, 45V, SOT23-3 smd

•	BC807 - PNP, 800mA, 45V, SOT23-3 smd 

•	ZXTN25012EFH - NPN 12V 6A smd

•	ZXTN25012EFLTA - 12V 2A fab. Diodes smd

•	ZXTN25012EZTA - NPN 12V 6,5A smd

•	ZXTN25060BZ - NPN 60V 5A smd

•	FMMT458TA - NPN, 400V, 0,25A 0,5W SOT23 smd

•	2N3904 - BJT, genérico, npn, 40V, 200 mA, largura de banda 300 Mhz, 625 mW, figura de ruído 5db, sinal.

•	2N3906 - BJT, genérico, pnp, -40 V, -200mA, 250 MHz, 625 mW, ruído figura 4db, sinal, par complementar do 2N3904.

•	BD135 - BJT, npn, média potência, beta 100, 45 V, 1,5 A, 1,25 W, amplificador de áudio.

•	BD136 - BJT, pnp, média potência, beta 100, -45 V, -1,5 A, 1,25 W, amplificador de áudio, par complementar de BD135.

•	BD139 – BJT, npn, 1,5A, 80V

•	KSP10 - Este é um substituto para o bom e velho BF199. BJT, npn, transistor RF, largura de banda 650 MHz a 1GHz, 25V, beta 60, 60 mA, 350 mW.

•	TIP31CG - BJT, alta potência, npn, 100 V, 3 A, 40 W, 3 MHz, beta 20.

•	TIP32CG - BJT, alta potência, pnp, -100 V, -3 A, 40 W, 3 MHz, beta 20, par complementar de TIP31CG.

•	TIP41CG - BJT, alta potência, npn, 100 V, 6 A, 65 W, 3 MHz, beta 20.

•	TIP42CG - BJT, alta potência, pnp, -100 V, -6 A, 65 W, 3 MHz, beta 20, par complementar de TIP41CG.

•	TIP122 - BJT, darlington de alta potência, npn, 100 V, 5 A, 65 W, beta min 1000, TO220.

•	TIP127 - BJT, darlington de alta potência, pnp, -100 V, -5 A, 65 W, beta min 1000, TO220, par complementar de TIP122.

•	2N6027 - Este é um substituto para o bom e velho 2N26469.

•	PUT - Transistor Unijuncional Programável, 40 V, 300 mW.
Este é um componente que tem uma zona de "resistência negativa". O 2N2646 foi utilizado em osciladores com saída tendo "baixa impedância", ou seja, somente com um "transistor", era possível fazer um oscilador que aciona diretamente um alto-falante de baixa potência.

•	ULN2003A - chip, sete matrizes darlington, corrente de saída 500 mA, tensão de saída 50 V, diodos de supressão integrados para cargas indutivas, entradas compatíveis com TTL/CMOS.

•	ULN2803A - chip, oito transistores darlington com emissores comuns, corrente de saída de 500 mA, tensão de saída de 50 V, diodos de supressão integral, entradas compatíveis com TTL/CMOS.

### Transistores JFet
•	J111 - Tipo n, -35V, 50mA, 625mW, 30 Ohms, sinal.

•	J175 - Tipo p, 30V, 50mA, 350mW, 125 Ohms sinal.

### Transistores MOSFET
•	DMG6968UDM-7 - canal N, 20V 6,5A, 25mhom,  sot23-3 marking code 2N4

•	IRF830 – canal N, 500V 4,5A , 1,5R TO-220  pth

•	8N60 – canal N, 600V 7,5A , 1,2R , TO-220 pth

•	BS170 - canal N, 60V , 500mA, capacitância de entrada 60pf, comutação 4ns.

•	BS250 - canal P, -45 V, -230 mA, 700mW.

•	DMG1012UW-7 - canal N, 20V, 1A, SOT-323, SMD.

•	IRF3205PBF - canal N, Potência MOSFET 150 W, 55V, 110A, 8mOhm, 97.3nC.

### Transistores IGBT
•	STGF5H60DF - 600 V, 5 A, 24 W.

•	STGP7NC60HD - 600 V, 14 A, 25 W.

•	STGP40V60F - 600 V, 40 A, 62.5 W.

•	IHW25N120E1 - 1200 V, 25 A, 231 W.

•	FGH80N60FD2 - 600 V, 40 A, 290 W.

### Tiristores
•	TIC106D – SCR 400V, 6A TO-220 pth

•	P0102DA - SCR, 400 V, 0,8A, TO-92.

•	2N6507G - SCR, 400 V, 25A, TO220-AB.

•	Z0409NF0AA2 - TRIAC, 600V, 4 A.

•	T1620T-8I - TRIAC, 600V, 16A.

### Amplificadores Operacionais 
•	LM358 - Duplo, barato, 3V a 36V, largura de banda 1,2 MHz, Voffset 3mV, figura de ruído 40nV/sqrt Hz, não trilho para trilho.

•	TL072 - Duplo, entradas JFET, barato, baixo THD - Distorção Harmônica Total 0,003%, Baixo ruído 18 nV/sqrt Hz, não trilho para trilho, usado em áudio de alta qualidade.

•	NE5532 - Baixo ruído, barato, fornecimento min +-5V a +-15V, não trilho para trilho, 10 MHz, Voffset 4mV, 5 nV/sqrt Hz, baixo THD - Distorção Harmônica Total, usado em áudio de alta qualidade.

•	MCP6004-I-P - Microchip, quad, barato, rail-to-rail, fonte única 3.3V a 5V, largura de banda 1MHz, tensão offset = 4.5 mV, figura de ruído 28nV/sqrt Hz.

•	MCP6024-E/P - Microchip, quad, rail-to-rail, fonte única 3.3V a 5V, largura de banda 10MHz, tensão offset = +-0.250 mV, temperatura estendida, figura de ruído 8.7nV/sqrt Hz.

•	MCP6072T-E/SN - Microchip, duplo, barato, largura de banda 1,2 MHz, tensão offset = 150 uV, SOIC-8 SMD, 19nV/sqrt Hz.

•	TC7650CPA - único, chopper, de fonte única ou de alimentação dupla 5V, não trilho para trilho + limite inferior de 0,3V - limite superior de 0,3V, amplificador operacional estabilizado com chopper de deslocamento zero, tensão de deslocamento de baixo ruído de entrada 2,0 uV pp largura de banda de 2MHz.

### Comparadores
•	LM2903 - Comparador de tensão smd soic8, atuação rápida para proteção contra curto-circuito.

•	LM393 - Comparador duplo até 38V, 1uS.

•	LM339 - Comparador quádruplo, alimentação simples de 2 V a 36 V, alimentação dupla ± 1 V a ±18 V, corrente de saída de 20 mA.

### Temporizador e gerador de frequências 555
•	NE555 - Temporizador de microssegundos a horas, estável e monoestável, ciclo de trabalho ajustável, saída TTL compatível, pode afundar ou fonte 200 mA.

### Reguladores de tensão
•	LM78xx CIs, 1,5 A, exemplos: 7805 (5 V), 7806 (6 V), 7808 (8 V), 7809 (9 V), 7810 (10 V), 7812 (12 V), 7815 (15 V), 7818 (18 V) e 7824 (24 V).

•	LM79xx CIs tensão negativa, 1,5 A, exemplos: 7905 (-5 V) e 7912 (-12 V).

•	LM2596S-ADJ Regulador de tensão ajustável 1,2V a 37V 3A enc. TO-263 ( Step Down com indutor, diodo schottky e divisor resistivo) . Usado no shield Arduino.

•	LD1117V33 - Regulador de tensão ST, 3,3 V, 0,8A, TO-220-3, a tensão de entrada tem que ser min 1V superior.

•	LD1117V50 - Regulador de tensão ST, 5 V, 0,8A, TO-220-3, a tensão de entrada tem que ser min 1V superior.

•	LD1117 - Regulador de tensão ajustável ST, 0.8A TO-220-3, a tensão de entrada tem que ser min 1V superior.

•	LD1117S33CTR - Regulador de tensão LDO 3.3V, 0.8A, positivo, SMD, pacote SOT-223-3.

•	LM317 - Regulador ajustável, 1,5 A.

•	MC34063 – regulador ajustável 1,5A Boost/Buck/ Inverting 3 a 40Vcc

### PTC- Positive Temperature Current
•	RUEF400 - PolySwitch Resetavel PPTC 4A 30V fab. Littelfuse ( Usado para proteger sobrecorrente, pois aumentam a resistência quando a corrente sobe acima do seu valor nominal. A desvantagem é que são lentos.) 

•	RUEF900 -  PolySwitch Resetavel PPTC 7A 30V fab. Littelfuse

### NTC - Negative Temperature Current
•	5D-11 5R 4A -  Termistor pth modelo NTC ( Usado após o fusível e em série com ele para ajudar no controle de corrente de partida de fontes chaveadas –Inrush current).

### Sensor de temperatura
•	LM35 – varia 10mV a cada 1° Celsius.

•	LM35DZ - Sensor de temperatura, linear + fator de escala de 10 mV/C, precisão garantida de 0,5 C, faixa de -55 C a 150 C.

### Microcontroladores PIC
•	12F1501 - 1K flash, 64 RAM, 8 pinos

•	12F1502 – 3.5K flash, 256 RAM, 8 pinos

•	12F1572 – 2K flash, 256 Ram, 128 HEF flash (substituindo eeprom), 8 pinos

•	16F15324 - 7Kb flash, 512 Ram, 10ADs, XLP@1V8, 14 pinos

•	16F877A- 40 pinos

•	18F24K40 - 16K Flash, 1K Ram, 256 Eeprom, 25 I/Os, 28 Pinos

•	18F45K50 - 32K_flash, 2K Ram, 256 EEprom, 1USB, 1 UART

•	18F46K22 - 64K flash, 3K8 Ram, 1K EEprom, Sem USB, 2 UART, 36 I/Os, 44 pinos

•	18F57Q80 –  128K Flash, 12K5 Ram, 1KEeprom, 5 USART, 44 I/Os, 43 ADCs de 12 bits

### Microcontroladores ST
•	STM32F429ZIT6 – 180Mhz, 32 bits

•	STM8S00SK6T6C – Usado no controle do No-break tipo UPS-Mini

### Cristais
•	32.768 Khz ( Muito usado para gerar a base de 1 segundo para o RTC interno dos microcontroladores ou como oscilador externo dos RTC’s ).

•	4Mhz; 8Mhz; 12Mhz; 16Mhz; 24Mhz; 48 Mhz; 64 Mhz

### Displays:
•	LCD 16x2; 20X2 ; 40x4

•	Display Nextion - Diversos tamanhos em polegadas 3,5” , 4,7”...

### Receivers RS-232 
•	MAX232 - 

### Transceivers RS-485
•	MAX485E – 

•	SP485 –

### Transceiver CAN-BUS
•	SN65HVD230 – Fabricante Texas Instruments (Usado no Shield Arduino)

### RTC – Real Time Calendar
•	PCF85063AT/AY - Circuito Integrado soic-8 smd (Calendário com Data, hora, segundos e pino de saída para alarme).

•	HT1380 – fabricante Holtek

### Memória Eeprom
•	24LC256 - 256Kb (32K x 8)

### Componentes Especiais:
•	L293D - Duas pontes H, fornecimento até 36 V, 600 mA, pico 1.2A.

•	LM386 - Amplificador de áudio classe A-B, ampla faixa de tensão de alimentação 4 V–12 V ou 5 V–18 V, baixa distorção 0,2%, ganhos de tensão de 20 a 200, 20 a 700 mW.

### Os componentes a baixo como fazem parte de um projeto, Edemilso Ilha, pode desenvolvê-lo para uma solução completa e um funcionamento perfeito para sua solução:

• Buzzer 100 db, alimentação 5V até 24Vcc, com oscilador interno, usado para sirenes por exemplo.

• Fototransistor - Par transmissor e receptor de detecção de fumaça com excelente sensibilidade.

• Sensor de temperatura barato e com excelente precisão de -15° a 110° Celcius.

• Buck converter 85 a 240 Vac para saída regulada com valores entre 5V a 16V,  4,2W  até +/- 600mA máximo, com proteção de sobrecorrente, curto circuito na saída, dentre outras proteções. Tudo isso num único CI usando poucos capacitores e resistores ao redor. Solução muito barato para um regulador com diversas proteções. E a grande vantagem deste circuito é não utilizar transformador de entrada, o que reduz muito os custos de fabricação.

• Rede com fio de até 400 dispositivos na mesma rede RS-485 utilizando tranceivers de baixa impedância e 1,2Km de distância máxima, sendo possível ler sensores e acionar saídas através desta rede com resposta de até 10 segundos de todos os dispositivos. Muita programação por de trás de tudo isso para funcionamento correto. Redes de Alarmes de Incêndio Endereçáveis funcionam desta forma por exemplo.

• Driver de brilho constante para iluminação a led de diversas potências.

# Isenção de Responsabilidade
•	Por favor, antes de escolher um componente ou usá-lo, sempre verifique as especificações de cada peça usando a ficha técnica do fabricante. Eu coleciono as características das peças com muita diligência, mas não assumo qualquer responsabilidade por qualquer erro que poderia ter cometido nesta lista ou por um componente se tornar obsoleto.

# Licença
Este documento está sob a licença Creative Commons.


