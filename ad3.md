# AD3

Esta es la actividad 3 que consiste en hacer un ejercicio de programación literaria aprovechando el código que hemos usado en programación con phyton donde realizamos *web scraping*.

A continuación pongo el código fuente.


## Código fuente


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
 
resultados = []
 
req = requests.get("https://resultados.elpais.com")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')
 
tags = soup.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')
 
tags = soup2.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')
 
tags = soup3.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')
 
tags = soup4.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')
 
tags = soup5.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')
 
tags = soup6.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')
 
tags = soup7.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')
 
tags = soup8.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')
 
tags = soup9.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')
 
tags = soup10.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')
 
tags = soup11.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')
 
tags = soup12.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')
 
tags = soup13.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')
 
tags = soup14.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')
 
tags = soup15.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req16 = requests.get("https://elpais.com/television/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup16 = BeautifulSoup(req16.text, 'html.parser')
 
tags = soup16.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')
 
tags = soup17.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
 
 
os.system("clear")
 
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
 
print(colored("Igualdad", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))
 
print(colored("Mujeres", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))
 
print(colored("Mujer", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))
 
print(colored("Brecha salarial", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))
 
print(colored("Machismo", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))
 
print(colored("Violencia", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))
 
print(colored("Maltrato", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))
 
print(colored("Homicidio", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))
 
print(colored("Género", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))
 
print(colored("Asesinato", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))
 
print(colored("Sexo", 'green', attrs=['bold']))
 
str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))
```


    ---------------------------------------------------------------------------

    ModuleNotFoundError                       Traceback (most recent call last)

    Input In [1], in <cell line: 1>()
    ----> 1 import requests
          2 import time
          3 import csv
    

    ModuleNotFoundError: No module named 'requests'





# Programación Literaria


## Librerías y módulos


Vamos a importar los siguientes módulos y librerías:
    

## Módulos del sistema
Aquí voy a importar las siguientes librerías: 

-[time](https://docs.python.org/es/3/library/time.html).Destaca funciones relacionada con el tiempo.

-[csv](https://docs.python.org/es/3/library/csv.html)Se utiliza para la lectura y escritura en valores separados por coma, por ejemplo,csv.

-[re](https://docs.python.org/es/3/library/re.html).Proporciona expresiones regulares, similares a las encontradas en perl.

-[os](https://docs.python.org/es/3.10/library/os.html).Permite acceder a funcionalidades dependientes del sistema operativo.

## Librerías Externas

[Requests](https://requests.readthedocs.io/en/latest/). Facilita el trabajo con peticiones HTTP

[bs4](https://www.crummy.com/software/BeautifulSoup/). Permite extraer contenido en formato HTML Y XTML.

[pandas](https://pypi.org/project/pandas/). Facilita el tratamiento de datos.

[termcolor](https://replit.com/talk/learn/How-to-Use-Termcolor-In-Python/24684).Hacer ajuste de color.

## Instalamos librerías

Las librerías que vienen con python no es necesario instalarlas, pero las otras deben ser instaladas.


```python
pip install requests bs4 pandas termcolor
```

    Requirement already satisfied: requests in c:\users\alicia valdés\lib\site-packages (2.28.1)Note: you may need to restart the kernel to use updated packages.
    

    WARNING: You are using pip version 21.2.4; however, version 22.1.2 is available.
    You should consider upgrading via the 'C:\Users\Alicia Valdés\python.exe -m pip install --upgrade pip' command.
    

    
    Requirement already satisfied: bs4 in c:\users\alicia valdés\lib\site-packages (0.0.1)
    Requirement already satisfied: pandas in c:\users\alicia valdés\lib\site-packages (1.4.3)
    Requirement already satisfied: termcolor in c:\users\alicia valdés\lib\site-packages (1.1.0)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\alicia valdés\lib\site-packages (from requests) (2022.6.15)
    Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\alicia valdés\lib\site-packages (from requests) (2.1.0)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\alicia valdés\lib\site-packages (from requests) (1.26.9)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\alicia valdés\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: beautifulsoup4 in c:\users\alicia valdés\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: numpy>=1.21.0 in c:\users\alicia valdés\lib\site-packages (from pandas) (1.23.0)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\alicia valdés\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: pytz>=2020.1 in c:\users\alicia valdés\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: six>=1.5 in c:\users\alicia valdés\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\alicia valdés\lib\site-packages (from beautifulsoup4->bs4) (2.3.2.post1)
    

## Importamos las librerías


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
```

## objetos variables
Vamos a crear una serie de objetos variables

## Resultados
Vamos a crear un objeto vacío denominado resultados, en el que se añadirán los resultados del scraping*.


```python
resultados = []
```

Si pasamos la función type () podemos observar que el objeto es de tipo *lista** de phyton. 



```python
type(resultados)

```


```python
list


```




    list



## Acceso a Datos

Se añade una variable con la que se hace uso de la solicitud req=requests.get("https://resultados.elpais.com") para recoger la información de esa URL.

Se realiza una solictud req = requests.get("https://resultados.elpais.com") para recoger la información de la URL.


```python
req=request.get("https://resultados.elpais.com")

```


```python
Si pasamos la función type() podemos observar que este objeto es de tipo Respuesta de modelo requests.
```


```python
type(req)
```


```python
requests.models.Response
Como está comentado en el propio código, se emplea un condicional if para que cuando el estatus no sea 200 el valor de vuelta no pueda leerse. Este valor 200 significa que la solicitud fue exitosa y el servidor respondió con los datos solicitados. En caso de que no se encuentre un resultado como el indicado se mostrará el mensaje
No se puede hacer Web Scrapping en seguido de la URL errónea.
```




    list




```python
# Si el estatus no es 200 no se puede leer la página
if (req.status_code != 200):
    raise Exception("No se puede hacer Web Scraping en"+ URL)
```

Si pasamos la función type() podemos observar que el objeto req.status_code es de tipo entero, por lo que el resultado será numérico.


```python
type(req.status_code)

```



## Beautiful Soup
Se añade otra variable para aplicar el Web Scrapping.


```python
soup = BeautifulSoup(req.text,'html.parser')
```

Si pasamos la función type() podemos observar que este objeto es de tipo bs4.

type(soup)


bs4.BeautifulSoup
También se añade la variable que sirve para encontrar todas las etiquetas <h2> 
dentro de la página anteriormente especificada.



```python
tags = soup.findAll("h2")
```


```python
Si pasamos la función type() podemos observar que el objeto tags es de tipo Resultado del set de elementos bs4.
```

type(tags)

bs4.element.ResultSet
Se indica a través de un for, que se recorran todos los h2 dentro de la variable anterior y se imprima el texto dentro de la etiqueta. Posteriormente con resultados.append(h2.text),
se añaden todos los textos dentro de las etiquetas a la lista inicial resultados.


```python
for h2 in tags: 
    print(h2.text)
    resultados.append(h2.text)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Input In [6], in <cell line: 1>()
    ----> 1 for h2 in tags: 
          2     print(h2.text)
          3     resultados.append(h2.text)
    

    NameError: name 'tags' is not defined



```python
En el código se añadió una variable para buscar las etiquetas `<h2>`, las cuales significan título, dentro de la página.
```


```python
Input In [9]
    En el código se añadió una variable para buscar las etiquetas `<h2>`, las cuales significan título, dentro de la página.
```


```python
tags = soup.findAll("h2")
```

Se le indicó, a través de un for, que imprima el texto que esta dentro de la etiqueta <h2>.


```python
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
type(resultados.append)
```


```python
builtin_function_or_method

A partir de esta primera acción se repite el mismo proceso para las URLs de las subsecciones de https://elpais.com: internacional, opinión, España,
economía, sociedad, educación, clima y medio ambiente, ciencia, cultura, babelia, deportes, tecnología, gente, televisión y eps.
Por tal motivo,  se realiza el proceso previo de forma similar y se modifican los nombres de las variables poniéndosele números
por ejemplo:req2 para la URL https://elpais.com/internacional y así sucesivamente.
```


```python
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')

tags = soup3.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')

tags = soup14.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
    req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req16 = requests.get("https://elpais.com/television/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup16 = BeautifulSoup(req16.text, 'html.parser')

tags = soup16.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
    
```

## Explicación del ejercicio y errores propios
El ejercicio que realizamos en Phyton con la asignatura de Programación, trataba de un juego en donde cada jugador elegía cómo darle un giro al juego. En este caso, el código de la compañera Iria Santos,nos invitaba mediante el código de web scraping recolectar los titulares de todas las seccciones del periódico **El País**, dichos titulares tenían en común palabras claves, como:igualdad, mujer, machismo, maltrato, homicidio, género. Un juego bastante interesante.

No obstante, no sé qué cuantas cosas hice mal , porque algunas respuestas no me salieron como esperaba. Traté de hacer el mismo procedimiento de la compañera ( por si acaso así me salía), más tampoco pude con el "Out", que tengo entendido es de lista.

Pese a todo  el ejercicio fue interesante, como para seguir practicando y haciendo los ajustes. Considero que aprendí algunos detalles significativos para futuros trabajos ( en comparación cuando inicié), a pesar de los errores y dudas pendientes. 


```python

```
