
# Proyecto: Data Cleaning and Manipulation with Pandas

## Procesos seguidos

### Importación y exportación de data

Para importar la data simplemente decargué el csv y lo importé usando "pd.read_csv"
Para exportar la data utilicé la fórmula pd.csv_write

## Limpieza de la base 

Métodos utilizados:
  - df.shape()
  - df.replace()
  - list comprenhesion
  - .lower()
  - .isnull()
  - .nunique()
  - re.sub()
  - np.where()
  - .value_counts()

El principal reto con esta base es que en muchas de sus variables cuenta con muchos valores únicos que muchas veces son repetición de lo mismo pero expresado de diferentes formas o también expresiones que se refieren a cosas muy diversas como ocurre con la variable "activity". 

En el caso de la variable date el reto es que contiene con fechas en muchos formatos diferentes o con datos inexactos, mezclan palabras con números, etc.

La variable de nombres incluye valores que no son nombres además de que en algunos casos trae varios nombres, así como nombres muy diversos, algunos incluyen guión intermedio, puntos, entre otros.

