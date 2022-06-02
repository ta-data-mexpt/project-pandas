# Project: Data Cleaning and Manipulation with Pandas

## Overview

The goal of this project is to combine everything you have learned about data wrangling, cleaning, and manipulation with Pandas so you can see how it all works together. For this project, you will start with this messy data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). You will need to import it, use your data wrangling skills to clean it up, prepare it to be analyzed, and then export it as a clean CSV data file.

**You will be working individually for this project**, but we'll be guiding you along the process and helping you as you go. Show us what you've got!

---

## Realización de este proyecto

Para la realización de este proyecto se consideraron diferentes pasos, no se tomó un orden específico de acción, cosa que se podria mejorar en futuros proyectos. El archivo CSV de shark attacks se encontraba terriblemente sucio, constando de mas de 20,000 renglones de los cuales una buena cantidad estaban totalmente vacios. Lo primero que se realizó fue eliminar estos renglones hasta quedarnos con al rededor de 6,000 renglones con imformación relativamente completa. Despues de esto se eliminaron columnas que tuvieran ionformación repetida o que bien tuvieran una gran cantidad de datos faltantes incluso después de eliminar renglones vacios. Se llenaron valores nulos que se pudieran obtener de alguna forma o bien haciendo inferencias sobre los datos mismos y en caso de que no se encontrara ninguna forma de llenarlos, con la leyenda 'No Data'. Se cambió el tipo de datos de la fecha a tipo fecha en los elementos que se pudiera. Finalmente se guardó un nuevo archivo limpio como CSV.

## Dificultados

Al no tener un objetivo claro, las manipulaciones de datos que se podian hacer quedan enteramente a nuestra decisión por lo que la insertidumbre de si la forma en que estamos limpiando los datos o no es correcta siempre se encuentra además de no tener total confienza en eliminar columnas ya que al no tener objetivo, no podiamos evaluar la importancia de los datos que encontrabamos eliminando. Me parece que esta fué la mayor dificultad de este proyecto ya que hacer la manipulación de datos una vez decidido que se haría es bastante directo.

## Resultados

El resultado es un archivo CSV de menor tamaño y con datos más estandarizados.