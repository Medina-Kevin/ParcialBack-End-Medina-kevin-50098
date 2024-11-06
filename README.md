# ParcialBack-End-Medina-Kevin-50098

## Instrucciones para Ejecutar la API en REMOTO

### Paso 1: Abrir Postman  
### Paso 2: En postman, primero crear un POST, luego poner el siguiente URL y enviarle el adn que se va a verificar:  
https://mutantesrender.onrender.com/mutant/  
### Paso 3: En postman, primero crear un GET, luego poner el siguiente URL para obtener las estadisticas de la cantidad de adns humanos y mutantes que se probaron: 
https://mutantesrender.onrender.com/stats  
### Aca dejo algunos ejemplos que se pueden usar para probar
**Ejemplo de ADN mutante válido**:
  ```json
	{
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	}
```

**Ejemplo de un mutante:**  
  ```json
	{  
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	}  
```
**Ejemplo de un NO mutante:**  
  ```json
	{  
	"dna": ["ATGCGA", "CAGTGC", "TTATTT", "AGACGG", "GCGTCA", "TCACTG"]
	}   
```





## Instrucciones para Ejecutar la API en LOCAL

### Paso 1: Descargar el Repositorio

Una vez descargado el repositorio desplayaremos la carpeta "MutantePrueba" en este orden  

- a) MutantePrueba  
- b) src  
- c) main  
- d) java  

### Paso 2: Ejecutar la JavaClass Principal

Una vez hayamos desplayado las carpetas en el orden anteriormente dicho podremos observar la JavaClass "MutantePruebaApplication", la cual debemos ejecutar

### Paso 3: Confirmar Ejecución

 Una vez la ejecución esté en proceso se abrirá la consola, la cual nos debería mostrar el siguiente mensaje si todo se ha ejecutado correctamente    
`Started MutantePruebaApplication in X (Tiempo que tardó) seconds`

## Configuración en Postman

### Paso 4: Crear una Nueva Colección en Postman

Luego abriremos el Postman y crearemos una nueva colección.

### Paso 5: Agregar Requests a la Colección

En esta nueva colección agregaremos los siguientes Request:

- **"GET ALL"** de tipo `GET`
- **"CREATE"** de tipo `POST`

### Paso 6: Configurar el Request "CREATE"  
Nos dirigiremos a la Request "CREATE" y escribiremos la siguiente URL:  
`http://localhost:8080/mutant/`  y daremos "Send" 

### Paso 7- Luego pondremos "Save"  
### Paso 8:    
Una vez coloquemos la URL tendremos que configurarlo colocando lo siguiente:  
	a) Seleccionaremos "Body"  
 	b) Marcamos "raw"  
	c) Elegimos JSON  
 ### Paso 9:  
Ahora podremos corroborar si el DNA de nuestro humano es mutante o no,
para averiguarlo tendremos que ingresar el DNA con la siguiente estructura (recuerda que el `dna` debe ser escrito entre comillas, aqui te dejo unos ejemplos)      

**Ejemplo de ADN mutante válido**:
  ```json
	{
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	}
```

**Ejemplo de un mutante:**  
  ```json
	{  
	"dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"]
	}  
```
**Ejemplo de un NO mutante:**  
  ```json
	{  
	"dna": ["ATGCGA", "CAGTGC", "TTATTT", "AGACGG", "GCGTCA", "TCACTG"]
	}   
```





### Paso 10:  
Una vez ingresemos el DNA tendremos que apretar "send", una vez escaneado el DNA, nos mostrará un mensaje el cual nos dirá si es Mutante o es Humano.  

