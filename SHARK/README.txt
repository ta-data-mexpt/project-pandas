Primero el tema fue el leer el cvs, requería de una decodificación especifica. El cual se buscó por google.
•	Posterior se realizó el análisis de las columnas con mayor null.
•	Revisamos el total de nulos de cada columna y eliminamos los que tiene un porcentaje mayor al 60%
•	antes de continuar, vamos a limpiar los nombres de las columnas, para poder trabajar con ellas
•	De los países donde ha habido ataques, voy a eliminar todos los ataques aislados, y solo con los países que tiene el mayor registro de ataques
•	Realizamos un análisis de los nulos que aún me aparecen en las columnas
•	Vamos a unificar las columnas y rellenar los nulos de sex
•	Revisaremos activity
•	Revisaremos fatal_(y/n)
•	Rellenaremos las columnas que tiene pocos null, con un string o valor de acuerdo a lo que solicita
•	En el programa que viene vamos a cargar los links de la lista de links que difiere, y vamos a realizar un request para ver si el link es funcional o no, vamos a guardar los links funciones en ambas tablas para que ahora si sean iguales
•	Pero en el caso de que los links estén caídos, los vamos a guardar con una comentario de link caído, esto lo guardaremos en ambas columnas y para después solo quedarnos con una de ellas.
•	Como aun tenemos varios nullos, se les realizara un filtro , en donde eliminaremos las filas donde Age, time y species tengan null
•	La tabla de edad, se revisará dato por dato, en donde se pueda guardar como entero, en donde no se guardara como 0.
•	Vamos a remplazar los horarios de 11hr00 a 11:00:00, para el caso de querer cambiarlo a time, sin embargo, no sería conveniente debido a que solo cuenta con hora
•	En el caso de spacies, se agregará como sin identificar en la tabla para los casos null
•	Vamos a limpiar las tablas case_number para solo quedarnos con una
•	Guardamos la tabla limpia como cvs
