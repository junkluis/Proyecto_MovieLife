![Logo App](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/movielife.png?alt=media&token=8a746ce5-4a89-4dcf-a8e7-cfc7a010f0fc "De 300 x 120 píxeles")


**Proyecto Final Android Studio del Módulo de Programacioón de Oscar Llorenc y Carlos Axel Castex**


DETALLES DEL PROYECTO
------------------------

**APIS utilizadas en la app:**
1. API GMAPS (https://developers.google.com/maps/?hl=es-419) -> Geolocalización de Cines
2. OMDB (www.omdbapi.com) -> API utilizada para la búsqueda de Películas, Series ...ect


IMPLEMENTACIONES DEL PROYECTO
------------------------------

* Implementaciones Carlos:
    * Acoplar distintos módulos a la aplicación base 'RicoPaRico':
        * Geolocate GoogleMaps 
        * CRUD Firebase inicial
        * BookSearch

    * Adaptación de la app para que los datos ofrecidos sean de Cines, Series, etc...
    * Implementación de Home con datos en dummys antes de que funcionase desde API con sus respectivos detalles al pinchar en una.
    * Icono y Baner del menú
    * Guardado y borrado Pelicuas,Series de favoritos en Firebase
    * Entrada de menú 'Cerca de ti' desde la que puedes ver cines cercanos en dummys
    * Details cines con Navigation, Streetview , guardado en favoritos, vista en googlemaps, enlace con un click web del cine y teléfono.
    * Seetings con Seekbar

* Implementaciones Oscar:

* Implementaciones Conjuntas:

FUNCIONALIDAD DEL PROYECTO
------------------------------

Nuestro proyecto es una aplicación de cine. Ofrece información sobre películas y series, extraída desde la API de OMDB.

El menú principal nos ofrece diferentes opciones desde donde podemos movernos dentro de la aplicación

![menu1](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/menu1.jpg?alt=media&token=a52af498-68fb-4376-9cfb-061ae4f99316 "De 520x880 píxeles")

![menu2](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/menu2.jpg?alt=media&token=78c8ecc8-8f3e-4a5d-9c8a-9b4976001fd0 "De 520x880 píxeles")


Desde la entrada de menú 'Registrarse' podemos acceder a nuestra cuenta (si estamos registrados previamente), desde google+, email o twitter.


![logining](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/logining.jpg?alt=media&token=b29170ea-fd98-4d6d-8c2a-e00aeeef7dfb "De 520x880 píxeles")



Desde la entrada Estrenos (main) , nos mostrará las películas en estreno que hemos agregado nosotros al main cómo administrador (mediante un CRUD)


![main](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/main.jpg?alt=media&token=e5b3cb2c-5012-47ea-b1af-5e52aa104d8d "De 520x880 píxeles")



-- CRUD (SQLITE)
**(explicacion de que podemos hacer dependiendo de que user este logeado)**
--

Mediante la entrada de menú 'Sitúate' accederemos a un fragment de GMAps donde estarán pintados los cines disponibles (insertados mediante dummys) geoloalizados y en los cuales mediante un onClickInfo se nos abrirá el details de cada cine.




![detailscines](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/cinesdetails.jpg?alt=media&token=5bf73340-ad48-4c20-9fea-3d8890a450b5 "De 520x880 píxeles")



Desde estos details del cine podremos acceder a una vista de gmaps, pinchando sobre su dirección, abrir la página web del cine seleccionado en nuestro navegador dandole click en la url o, finalmente realizar una llamada telefónica al mismo mediante un click en su número de teléfono. 

Los cines que estarán pintados en la vista de Gmaps a la que accedemos mediante la entrada de menú 'Sitúate', estarán listados dentro de la sección que abriremos al pinchar en la entrada de menú 'Cerca de ti'
Estos cines estarán almacenados cómo dummys en firebase, en una rama sólo accesible por el administrador de la misma.



![listacines](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/cinesfavs.jpg?alt=media&token=ba5a7927-f5bb-44b6-8066-8c24bb9acf58 "De 520x880 píxeles")



Pinchando en uno de ellos, accederemos a los details de los mismos, al igual qe cuando pinchamos en el InfoView de google maps.



Cómo hemos comentado antes, desde nuestro Main, tendremos los estrenos presentados por el administrador, sin embargo, si la película que queremos ver no se encuentra entre ellas, podremos buscarla desde la entrada de menú 'Buscar' o desde el icono de la lupa de nuestro Toolbar, accesible desde cualquier otra vista asociada al toolbar principal.
- Por defecto cada página de la búsqueda nos mostrará 10 resultados (modificables desde la config.)



![busqueda](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/seek.jpg?alt=media&token=3608099d-9ff7-4c87-9bf4-dd96780e9628 "De 520x880 píxeles")



--MIS FAVORITOS--
--



Desde el apartado de configuración podremos modificar , cómo hemos señalado en el apartado de búsqueda, las páginas que queremos cómo resultado de la misma.
Para ello haremos uso de un seekbar que adoptará valores de entre 1 a 100 páginas.



![settings](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/settings.jpg?alt=media&token=de51cb92-4687-4dce-920e-76c8167a47b6 "De 520x880 píxeles")




Finalmente, el apartado de Lang de nuestro menú principal, que consta de dos idiomas Español e Inglés, cambiará en su totalidad el idioma de nuestra app para que el usuario pueda utilizarla en su idioma.Cuando seleccionemos el idioma deseado se relanzará la app en dicho idioma.





![lang](https://firebasestorage.googleapis.com/v0/b/cineapp-b4786.appspot.com/o/lang.jpg?alt=media&token=ffa21179-50d0-4405-86e9-f85dc0f28879 "De 520x880 píxeles")

