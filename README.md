Calculadora_Team
Este es un proyecto de una calculadora que se realizara para la materia de tecnologías de diseño mecatrónico.

	
	#include<stdio.h>
	#include<conio.h>
	#include<math.h>
 

	main()
	{

		int resultado; /* Variable reservada para cada resultado de las operaciones */
		int a;         /* Primer numero que introducimos */
		int b;         /* Segundo numero que introducimos */
		int opcion;    /* Opcion que elegimos */
		do
			{
		
				clrscr();
				printf("\n         ÉÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ»");
				printf("\n         º               :: C A L C U L A D O R A ::                 º");
				printf("\n         ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹");
				printf("\n         º                                                           º");
				printf("\n         º       1.- Suma                     4.- Multiplicacion     º");
				printf("\n         º                                                           º");
				printf("\n         º       2.- Resta                    5.- Division           º");
				printf("\n         º                                                           º");
				printf("\n         º       3.- Raiz Cuadrada            6.- Potencia           º");
				printf("\n         º                                                           º");
				printf("\n         º                        7.- Salir                          º");
				printf("\n         ÈÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¼");
				printf("\n                     Nota: Solo funciona con numeros enteros");
				printf("\n");
				printf("\n                              Elija una opcion: ");
				scanf("%d",&opcion);
		
		switch(opcion)  /* Segun la opcion elegida tendremos los siguientes casos... */
		{
			case 1:     /* Suma */
			printf("\n         -> Introduzca el primer sumando: ");
			scanf("%i",&a);
			printf("\n         -> Introduzca el segundo sumando: ");
			scanf("%i",&b);
			resultado=a+b;
			printf("\n         La SUMA de %i + %i es igual a %i",a,b,resultado);
			break;
 
			case 2:     /* Resta */
			printf("\n         -> Introduzca el primer numero: ");
			scanf("%i",&a);
			printf("\n         -> Introduzca el segundo numero: ");
			scanf("%i",&b);
			resultado=a-b;
			printf("\n         La RESTA de %i - %i es igual a %i",a,b,resultado);
			break;
 
			case 3:     /* Raiz Cuadrada */
			printf("\n         -> Introduzca el numero al que efectuar la raiz: ");
			scanf("%i",&a);
			if (a>0) /* Con este if se pretende que solo haga la raiz de los numeros positivos */
			{
				resultado=sqrt(a);
				printf("\n         La RAIZ CUADRADA de %i es igual a %i",a,resultado);
			}
			else printf("\n         No puede hacer la raiz cuadrada de un numero negativo!!");
			break;
			
