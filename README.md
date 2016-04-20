# balance-sheet
A balance sheet report implemented by recursive traversal and summarized of a radix tree chart of accounts with balances

##Example output

| numero | 	nombre	 | tipo | saldo |
| :--- | :--- |:---: | ---: |
| 1 | 	FINANCIACION BASICA	 | debit | 	0 |
| 10 | 	CAPITAL	 | debit | 	0 |
| 100 | 	Capital social	 | debit | 	-2906.06 |
| 1000 | 	Capital social socio 1	 | credit | 	-2906.06 |
| 1001 | 	Capital social socio 2	 | credit | 	0 |
| 101 | 	Fondo social	 | debit | 	0 |
| 102 | 	Capital	 | debit | 	0 |
| 103 | 	Socios por desembolsos no exigidos	 | debit | 	-99 |
| 1030 | 	Socios por desembolsos no exigidos, capital social	 | debit | 	-99 |
| 1034 | 	Socios por desembolsos no exigidos, capital pendiente de inscripción	 | debit | 	0 |
| 104 | 	Socios por aportaciones no dinerarias pendientes	 | debit | 	564 |
| 1040 | 	Socios por aportaciones no dinerarias pendientes, capital social	 | debit | 	564 |
| 1044 | 	Socios por aportaciones no dinerarias pendientes, capital pendiente de insc	 | debit | 	0 |
| 108 | 	Acciones o participaciones propias en situaciones especiales	 | debit | 	0 |
| 109 | 	Acciones o participaciones propias para reducción de capital	 | debit | 	0 |
| 11 | 	RESERVAS Y OTROS INSTRUMENTOS DE PATRIMONIO	 | debit | 	0 |
| 110 | 	Prima de emisión o asunción	 | debit | 	0 |
| 111 | 	Otros instrumentos de patrimonio neto	 | debit | 	0 |
| 1110 | 	Patrimonio neto por emisión de instrumentos financieros compuestos	 | debit | 	0 |
| 1111 | 	Resto de instrumentos de patrimonio neto	 | debit | 	0 |
| 112 | 	Reserva legal	 | debit | 	0 |
| 113 | 	Reservas voluntarias	 | debit | 	0 |
| 114 | 	Reservas especiales	 | debit | 	-564 |
| 1140 | 	Reservas para acciones o participaciones de la sociedad dominante	 | debit | 	-564 |
| 1141 | 	Reservas estatutarias	 | debit | 	0 |
| 1142 | 	Reserva por capital amortizado	 | debit | 	0 |
| 1143 | 	Reserva por fondo de comercio	 | debit | 	0 |
| 1144 | 	Reservas por acciones propias aceptadas en garantía	 | debit | 	0 |
| 115 | 	Reservas por pérdidas y ganancias actuariales y otros ajustes	 | debit | 	0 |
| 116 | 	Reserva de revalorizaciones	 | debit | 	0 |
| 117 | 	Reserva por transacciones con pagos basados en acciones	 | debit | 	0 |
| 118 | 	Aportaciones de socios o propietarios	 | debit | 	0 |
| 119 | 	Diferencias por ajuste del capital a euros	 | debit | 	0 |
| 12 | 	RESULTADOS PENDIENTES DE APLICACIÓN	 | debit | 	0 |
| 120 | 	Remanente	 | debit | 	0 |
| 121 | 	Resultados negativos de ejercicios anteriores	 | debit | 	0 |
| 1210 | 	Resultados negativos ejercicio 1	 | debit | 	0 |
| 129 | 	Resultado del ejercicio	 | debit | 	-32001.71 |
| 1290 | 	Resultado del ejercicio	 | credit | 	-32001.71 |
numero	nombre	tipo	saldo
| 1 | 	FINANCIACION BASICA	 | debit | 	0 |
| 10 | 	CAPITAL	 | debit | 	-2441.06 |
| 100 | 	Capital social	 | debit | 	-2906.06 |
| 1000 | 	Capital social socio 1	 | credit | 	-2906.06 |
| 1001 | 	Capital social socio 2	 | credit | 	0 |
| 101 | 	Fondo social	 | debit | 	0 |
| 102 | 	Capital	 | debit | 	0 |
| 103 | 	Socios por desembolsos no exigidos	 | debit | 	-99 |
| 1030 | 	Socios por desembolsos no exigidos, capital social	 | debit | 	-99 |
| 1034 | 	Socios por desembolsos no exigidos, capital pendiente de inscripción	 | debit | 	0 |
| 104 | 	Socios por aportaciones no dinerarias pendientes	 | debit | 	564 |
| 1040 | 	Socios por aportaciones no dinerarias pendientes, capital social	 | debit | 	564 |
| 1044 | 	Socios por aportaciones no dinerarias pendientes, capital pendiente de insc	 | debit | 	0 |
| 108 | 	Acciones o participaciones propias en situaciones especiales	 | debit | 	0 |
| 109 | 	Acciones o participaciones propias para reducción de capital	 | debit | 	0 |
| 11 | 	RESERVAS Y OTROS INSTRUMENTOS DE PATRIMONIO	 | debit | 	-564 |
| 110 | 	Prima de emisión o asunción	 | debit | 	0 |
| 111 | 	Otros instrumentos de patrimonio neto	 | debit | 	0 |
| 1110 | 	Patrimonio neto por emisión de instrumentos financieros compuestos	 | debit | 	0 |
| 1111 | 	Resto de instrumentos de patrimonio neto	 | debit | 	0 |
| 112 | 	Reserva legal	 | debit | 	0 |
| 113 | 	Reservas voluntarias	 | debit | 	0 |
| 114 | 	Reservas especiales	 | debit | 	-564 |
| 1140 | 	Reservas para acciones o participaciones de la sociedad dominante	 | debit | 	-564 |
| 1141 | 	Reservas estatutarias	 | debit | 	0 |
| 1142 | 	Reserva por capital amortizado	 | debit | 	0 |
| 1143 | 	Reserva por fondo de comercio	 | debit | 	0 |
| 1144 | 	Reservas por acciones propias aceptadas en garantía	 | debit | 	0 |
| 115 | 	Reservas por pérdidas y ganancias actuariales y otros ajustes	 | debit | 	0 |
| 116 | 	Reserva de revalorizaciones	 | debit | 	0 |
| 117 | 	Reserva por transacciones con pagos basados en acciones	 | debit | 	0 |
| 118 | 	Aportaciones de socios o propietarios	 | debit | 	0 |
| 119 | 	Diferencias por ajuste del capital a euros	 | debit | 	0 |
| 12 | 	RESULTADOS PENDIENTES DE APLICACIÓN	 | debit | 	-32001.71 |
| 120 | 	Remanente	 | debit | 	0 |
| 121 | 	Resultados negativos de ejercicios anteriores	 | debit | 	0 |
| 1210 | 	Resultados negativos ejercicio 1	 | debit | 	0 |
| 129 | 	Resultado del ejercicio	 | debit | 	-32001.71 |
| 1290 | 	Resultado del ejercicio	 | credit | 	-32001.71 |
