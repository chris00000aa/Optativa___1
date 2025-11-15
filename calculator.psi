Proceso CalculadoraCompleta


    Definir opcion Como Entero
    Definir n1, n2, r Como Real
    Definir figura Como Entero
    Definir radio, diametro, area Como Real
    Definir cant, i, j, aux Como Entero
    Definir lista Como Entero
    Dimension lista[100]
    Definir suma Como Real
    Definir promedio, mediana Como Real
    Definir moda, repeticionesMax, reps Como Entero
    Definir numeroF, terminos, a, b, c Como Entero
	
    Repetir
		
        Limpiar Pantalla
        Escribir "MENU PRINCIPAL"
        Escribir "1 Operaciones basicas"
        Escribir "2 Calculo de areas radios y diametros"
        Escribir "3 Estadistica media mediana moda"
        Escribir "4 Sucesion de Fibonacci"
        Escribir "0 Salir"
		
        Repetir
            Escribir "Seleccione una opcion:"
            Leer opcion
			
            Si opcion < 0 O opcion > 4 Entonces
                Escribir "Opcion no valida"
            FinSi
        Hasta Que opcion >= 0 Y opcion <= 4
		
        Segun opcion Hacer
			
            1:      // OPERACIONES BASICAS
				
                Escribir "Ingrese numero 1:"
                Leer n1
                Escribir "Ingrese numero 2:"
                Leer n2
				
                Repetir
                    Escribir "Seleccione operacion:"
                    Escribir "1 Suma"
                    Escribir "2 Resta"
                    Escribir "3 Multiplicacion"
                    Escribir "4 Division"
                    Leer figura
					
                    Si figura < 1 O figura > 4 Entonces
                        Escribir "Opcion no valida"
                    FinSi
                Hasta Que figura >= 1 Y figura <= 4
				
                Segun figura Hacer
                    1: r = n1 + n2
                    2: r = n1 - n2
                    3: r = n1 * n2
                    4:
                        Si n2 = 0 Entonces
                            Escribir "No se puede dividir entre cero"
                            r = 0
                        SiNo
                            r = n1 / n2
                        FinSi
                FinSegun
				
                Escribir "Resultado: ", r
                Esperar Tecla
				
				
            2:      // AREAS Y RADIOS
				
                Repetir
                    Escribir "Seleccione figura:"
                    Escribir "1 Circulo"
                    Escribir "2 Cuadrado"
                    Escribir "3 Triangulo"
                    Escribir "4 Trapecio"
                    Leer figura
					
                    Si figura < 1 O figura > 4 Entonces
                        Escribir "Opcion no valida"
                    FinSi
                Hasta Que figura >= 1 Y figura <= 4
				
                Segun figura Hacer
					
                    1:
                        Escribir "Ingrese radio:"
                        Leer radio
                        diametro = radio * 2
                        area = 3.1416 * radio * radio
                        Escribir "Diametro: ", diametro
                        Escribir "Area: ", area
						
                    2:
                        Escribir "Ingrese lado del cuadrado:"
                        Leer n1
                        area = n1 * n1
                        Escribir "Area: ", area
						
                    3:
                        Escribir "Ingrese base:"
                        Leer n1
                        Escribir "Ingrese altura:"
                        Leer n2
                        area = (n1 * n2) / 2
                        Escribir "Area: ", area
						
                    4:
                        Escribir "Base mayor:"
                        Leer n1
                        Escribir "Base menor:"
                        Leer n2
                        Escribir "Altura:"
                        Leer r
                        area = ((n1 + n2) * r) / 2
                        Escribir "Area: ", area
						
                FinSegun
				
                Esperar Tecla
				
				
            3:     // ESTADISTICA
				
                Repetir
                    Escribir "Cuantos numeros desea ingresar (1 a 100):"
                    Leer cant
					
                    Si cant < 1 O cant > 100 Entonces
                        Escribir "Cantidad no valida"
                    FinSi
                Hasta Que cant >= 1 Y cant <= 100
				
                Para i = 1 Hasta cant Con Paso 1 Hacer
                    Escribir "Numero ", i, ":"
                    Leer lista[i]
                FinPara
				
                suma = 0
                Para i = 1 Hasta cant Hacer
                    suma = suma + lista[i]
                FinPara
				
                promedio = suma / cant
				
                // ORDENAR LISTA
                Para i = 1 Hasta cant - 1 Hacer
                    Para j = i + 1 Hasta cant Hacer
                        Si lista[j] < lista[i] Entonces
                            aux = lista[i]
                            lista[i] = lista[j]
                            lista[j] = aux
                        FinSi
                    FinPara
                FinPara
				
                // MEDIANA
                Si cant Mod 2 = 0 Entonces
                    mediana = (lista[cant/2] + lista[cant/2 + 1]) / 2
                SiNo
                    mediana = lista[(cant + 1) / 2]
                FinSi
				
                // MODA
                moda = lista[1]
                repeticionesMax = 1
				
                Para i = 1 Hasta cant Hacer
                    reps = 0
					
                    Para j = 1 Hasta cant Hacer
                        Si lista[i] = lista[j] Entonces
                            reps = reps + 1
                        FinSi
                    FinPara
					
                    Si reps > repeticionesMax Entonces
                        repeticionesMax = reps
                        moda = lista[i]
                    FinSi
                FinPara
				
                Escribir "Media: ", promedio
                Escribir "Mediana: ", mediana
                Escribir "Moda: ", moda
				
                Esperar Tecla
				
				
            4:      // FIBONACCI
				
                Repetir
                    Escribir "Ingrese numero inicial:"
                    Leer numeroF
					
                    Si numeroF < 0 Entonces
                        Escribir "Debe ser numero positivo"
                    FinSi
                Hasta Que numeroF >= 0
				
                Repetir
                    Escribir "Cuantos terminos desea generar:"
                    Leer terminos
					
                    Si terminos < 1 Entonces
                        Escribir "Debe ser mayor a cero"
                    FinSi
                Hasta Que terminos >= 1
				
                a = 0
                b = 1
				
                Mientras b < numeroF Hacer
                    c = a + b
                    a = b
                    b = c
                FinMientras
				
                Escribir "Sucesion desde ", b
				
                Para i = 1 Hasta terminos Hacer
                    Escribir b
                    c = a + b
                    a = b
                    b = c
                FinPara
				
                Esperar Tecla
				
				
            De Otro Modo:
                Escribir "Opcion no valida"
                Esperar Tecla
				
        FinSegun
		
    Hasta Que opcion = 0
	
    Escribir "Programa finalizado"
	
FinProceso



