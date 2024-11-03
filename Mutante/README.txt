Instrucciones para ejecutar la API

1- Una vez descargado el repositorio desplayaremos la carpeta "MutantePrueba" en este orden
	a)MutantePrueba
	b)src
	c)main
	d)java
2- Una vez hayamos desplayado las carpetas en el orden anteriormente dicho podremos
observar la JavaClass "MutantePruebaApplication", la cual debemos ejecutar
3- Una vez la ejecución esté en proceso se abrirá la consola, la cual nos debería mostrar el
siguiente mensaje si todo se ha ejecutado correctamente 
"Started MutantePruebaApplication in X (Tiempo que tardó ) seconds
4- Luego abriremos el Postman y crearemos una nueva colección.
5- En esta nueva colección agregaremos los siguientes Request
	a) "GET ALL" de tipo GET
	b) "CREATE" de tipo POST
	c) "UPDATE" de tipo PUT
	d) "DELETE" de tipo DEL
6- Nos dirigiremos a la Request "CREATE" y escribiremos la siguiente URL
"http://localhost:8080/mutant/" y daremos "Send"
7- Luego pondremos "Save"
8- Una vez coloquemos la URL tendremos que configurarlo colocando lo siguiente:
	a) Seleccionaremos "Body"	
	b) Marcamos "raw"
	c) Elegimos JSON
9)Ahora podremos corroborar si el DNA de nuestro humano es mutante o no,
para averiguarlo tendremos que ingresar el DNA con la siguiente estructura
" 	{
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	} 
".
Recuerda que el DNA debe ser escrito entre comillas, aqui te dejo unos ejemplos

	*EJEMPLO MUTANTE*
"
	{
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	}
"
	*EJEMPLO NO MUTANTE*	
"
	{
	"dna": ["ATGCGA", "CAGTGC", "TTATTT", "AGACGG", "GCGTCA", "TCACTG"]
	}
"
10) Una vez ingresemos el DNA tendremos que apretar "send", una vez escaneado
 el DNA, nos mostrará un mensaje el cual nos dirá si es Mutante o es Humano.











