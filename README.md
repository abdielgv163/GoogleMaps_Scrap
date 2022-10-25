
### Enlace a mi sitio web 👨‍💻: [abdielgv163.github.io](https://abdielgv163.github.io/)


---

# Google Maps Scrap 🌍

Herramienta que he creado para obtener información de Google Maps a partir de una entrada determinada. Esta información recopilada será utilizada únicamente para proyectos personales de ciencia de datos.

El programa está guardado en un jupyter notebook: `scraping_Google_Maps.ipynb`

---



[![Watch the video](https://i.imgur.com/k7zTCYE.png)](https://i.imgur.com/MWDzBwo.mp4)


---

>En caso de querer darle otro uso hay que tener en cuenta que *enviar consultas automáticas a Google es una violación de sus Términos de Servicio*.

---

## Funcionamiento

1. Comenzamos por crear una clase llamada `googleMapsScraper` la cual contiene la inicialización del driver y las funciones principales para abrir el navegador, realizar la búsqueda, obtener los resultados y scrollear hasta que dejen de aparecer.
    Esto se logra en su mayoría con `selenium` y `parsel` para poder ubicar los elementos de la página e interactuar con ellos (por ejemplo, posicionarse en la barra de búsqueda y ejecutar la acción).

2. Posteriormente le pasamos la URL del sitio web de Google Maps y nuestra entrada de texto que queremos que busque. Esto llamará a nuestra clase anterior y almacenaremos los datos, que hasta este punto sólo incluyen `nombre del lugar` y `url`.

3. Después creamos un DataFrame de nuestra lista para obtener una "tabla" con los nombres de las búsquedas y el link de cada sitio.

4. Posteriormente, se crea la función `completeDataCollect()` que recibe como parámetro las URLs de la tabla anterior.
    Esta ejecutará una búsqueda por cada elemento que tenemos para proceder a buscar datos como: `dirección, estrellas, total de calificaciones, sitio web, número de teléfono y horarios`.

5. Finalmente, guardamos toda esa información en lista para posteriormente crear otro DataFrame y unirlo con el DataFrame anterior; unificando toda la información.

---

<h3> Contacto: </h3> 


[![Twitter: AbdielGuerrero](https://img.shields.io/twitter/follow/AbdielGuerrer20?style=social)](https://twitter.com/AbdielGuerrer20) [![Linkedin:Abdiel Guerrero](https://img.shields.io/badge/-AbdielGuerrero-black?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/abdiel-guerrero-360a39195/)](https://www.linkedin.com/in/abdiel-guerrero-360a39195/) [![GitHub abdielgv163](https://img.shields.io/github/followers/abdielgv163?label=follow&style=social)](https://github.com/abdielgv163)<a href="https://platzi.com/p/abdiel-guerrero/"><img width="50" src="https://upload.wikimedia.org/wikipedia/commons/3/32/Platzi.jpg" />
