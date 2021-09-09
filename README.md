[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/mutazen/gestion-citas-access-2007">
    <img src="readme-images/logo.png" alt="Logo" width="500" height="350">
  </a>

  <p align="center">
    <a href="https://https://github.com/mutazen/gestion-citas-access-2007"><strong>Ver documentación»</strong></a>
    <br />
    <br />
    <a href="https://github.com/mutazen/gestion-citas-access-2007/issues">Reportar Bug</a>
    ·
    <a href="https://github.com/mutazen/gestion-citas-access-2007/issues">Solicitar nueva funcionalidad</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Índice</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del proyecto</a>
      <ul>
        <li>
          <a href="#restricciones-iniciales">Restricciones iniciales</a>
        </li>
        <li>
          <a href="#características">Características</a>
        </li>
      </ul>
    </li>
    <li>
      <a href="#preparando-la-aplicación">Preparando la aplicación</a>
      <ul>
        <li>
          <a href="#requisitos">Requisitos</a>
        </li>
        <li>
          <a href="#instalación">Instalación</a>
        </li>
        <li>
          <a href="#configuración">Configuración</a>
        </li>
      </ul>
    </li>
    <li>
      <a href="#guía-de-uso">Guía de uso</a>
      <ul>
        <li>
          <a href="#search-cocktail-by-name">Ver citas</a>
          <ul>
            <li>
              <a href="#installation">Ver citas de un día en concreto</a>
            </li>
            <li>
              <a href="#installation">Ver citas de la semana anterior o posterior</a>
            </li>
            <li>
              <a href="#installation">Ver citas del mes anterior o posterior</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#search-cocktail-by-name">Crear cita</a>
        </li>
        <li>
          <a href="#search-cocktail-by-name">Modificar cita</a>
        </li>
        <li>
          <a href="#search-cocktail-by-type">Eliminar cita</a>
        </li>
        <li>
          <a href="#search-cocktail-by-category">Copiar cita</a>
        </li>
        <li>
          <a href="#search-cocktail-by-ingredient">Buscar cita</a>
          <ul>
            <li>
              <a href="#installation">Buscar por nombre</a>
            </li>
            <li>
              <a href="#installation">Buscar por apellidos</a>
            </li>
            <li>
              <a href="#installation">Buscar por DNI</a>
            </li>
            <li>
              <a href="#installation">Buscar por NIE</a>
            </li>
            <li>
              <a href="#installation">Buscar por pasaporte</a>
            </li>
            <li>
              <a href="#installation">Buscar por teléfono</a>
            </li>
            <li>
              <a href="#installation">Buscar por fecha</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#filter-results-by-type">Asignar asistencia</a>
        </li>
        <li>
          <a href="#filter-results-by-category">Designar dia</a>
          <ul>
            <li>
              <a href="#installation">Designar dia para atender citas</a>
            </li>
            <li>
              <a href="#installation">Designar dia como festivo</a>
            </li>
            <li>
              <a href="#installation">Eliminar designación</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#filter-results-by-ingredient">Reservar hora</a>
          <ul>
            <li>
              <a href="#installation">Crear reserva</a>
            </li>
            <li>
              <a href="#installation">Ver reserva</a>
            </li>
            <li>
              <a href="#installation">Modificar reserva</a>
            </li>
            <li>
              <a href="#installation">Eliminar reserva</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#show-cocktail-information">Imprimir ficha de gestión de citas</a>
        </li>
      </ul>
    </li>
    <li><a href="#roadmap">Cronología</a></li>
    <li><a href="#contributing">Contribuciones</a></li>
    <li><a href="#license">Licencia</a></li>
    <li><a href="#contact">Contacto</a></li>
    <li><a href="#acknowledgements">Conocimientos</a></li>
    <li><a href="#special-thanks">Agradecimientos</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## Acerca del proyecto 

Conforme pasa el tiempo, queda más claro que las empresas deben digitalizar las herramientas que utilizan en el desarrollo de su actividad si quieren mejorar la calidad del servicio que proporcionan. No obstante, para las empresas más pequeñas, el costo de la adquisión del software y de la infraestructura de red que necesitan es inasumible.

Un ejemplo de empresa que se enfrenta a este tipo de problemas son las ONG más pequeñas, las cuales no cuentan con los recursos necesarios para poder digitalizar convenientemente los procesos que realizan en el desarrollo de su actividad. Y que en muchos casos, la infraestructura técnologica con la cuentan está desfasada.

Este proyecto surge para dar respuesta a esta problemática de una ONG en particular, desarrollando una solución para gestionar las citas de los usuarios adaptada al software y a la estructura de red disponible.

![Product Main Screen Shot][product-screenshot]

### Restricciones iniciales.

A la hora de desarrollar este proyecto se contaba con las siguientes restricciones:
* Utilizar software y la infraestructura tecnológica existente. 
 
En este caso, se decidió emplear Microsoft Access 2007 porque estaba presente en todos los equipos de la empresa y su implantación no implicaba excesiva modificación de la configuración de los equipos existente, que consistía en varios equipos de trabajo conectados en la misma red LAN.

* Se debe poder trabajar con la solución desde varios equipos de la red y al mismo tiempo.

Para poder permitir el trabajo simúltaneo, se controlan cuando los usuarios crean o modifican citas. Bloqueándo la hora en la que se asigna una cita durante su creación para que otros usuarios no puedan crear otra nueva. Y bloqueando el acceso a los datos de la cita, cuando otro usuario está modificando sus datos. 

### Características.

Para cumplir con su objectivo, esta solución es capaz de:
* Gestionar los datos de la citas: información personal de los usuarios, datos de contacto y anotaciones.
* Gestionar las horas y los dias en los que se pueden concertar citas y para que áreas.
* Llevar el control de la asistencia de los usuarios a sus respectivas citas.
* Asegurarse que los datos tengan el formato adecuado, controlando la entrada de datos cuando es posible.
* Buscar citas en función de los datos de la cita.

<!-- GETTING STARTED -->
## Preparando la aplicación
### Requisitos
Tener instalado Microsoft Access 2007. No funciona con versiones posteriores de Access.

### Instalación

1. Clona el repositorio.
   ```sh
   git clone https://github.com/mutazen/gestion-citas-access-2007.git
   ```
2. Ejecuta Citas.accdb

### Configuración

Antes de abrir el ejecutable de este proyecto, es preciso añadir al centro de confianza de Access la ubicación desde donde se va ejecutar dicho archivo. Con esto se evita que se muestre cada vez que se acceda a la solución. A continuación se describe como realizar esta configuración.

1. Abrimos Access 2007 directamente o hacemos abrimos un archivo de access mientras pulsamos la tecla "Shift". En pantalla principal de Access, hacemos clic en el logo de Office de la parte superior izquierda de la pantalla y en la nueva pantalla, accemos clic en el botón "Opciones de Access".

![acceder a configuracion de access][configuracion-1]

2. En la nueva pantalla, seleccionamos la opción "Centro de confianza" de la parte izquierda de la pantalla y en la parte derecha, hacemos clic en el botón "Configuración del Centro de Confianza".
 
![acceder a configuracion del centro de confianza][configuracion-2]

3. En este otra pantalla, pinchamos en "Ubicaciones de confiaza" en la columna de la parte izquierda de la pantalla y en la parte derecha, comprobamos si ya está registrada el directorio desde donde ejecutaremos el proyecto. En caso negativo, podemos agregar la el directorio haciendo clic en el botón "Agregar nueva ubicación ...". Si se quiere ejecutar el archivo desde otro ordenador, es necesario marcar la opción "Permitir ubicaciones de confianza que están en red" y después agregar la ubicación del directorio en red. 

![agragar ubicacion del directorio del proyecto][configuracion-3]

<!-- USAGE EXAMPLES -->
## Guía de uso
We have a demo if you want to follow the instructions below. <a href="https://mutazen.github.io/Your-cocktail">View Demo</a>
### Search cocktail by name
<p>
  To search a cocktail by its name, we can introduce its name into the input in the right side of the navbar and press the enter key or click on the 
  magnifying glass button.
</p>
<p>
  In this example, we are going to search for cocktails with the word "smoothie" in their name. So we write "smoothie" in the input and press the enter key. 
</p>

![Screen Shot Seaching by name 1][screenshot-search-name1]

<p>
  In this new screen, we can see all the cocktails that we have in our database that containts the word "smoothie" in their name. In this case, there are 7 cocktails that match the pattern.
</p>

![Screen Shot Seaching by name 2][screenshot-search-name2]

### Search cocktail by type
<p>
  To search a cocktail by its type, we have to click on the "types" button in the left side of the navbar.
</p>

![Screen Shot Seaching by type 1][screenshot-search-type1]

<p>
  In the new screen, we can see the different types of cocktails: "Alcoholic", "Non alcoholic" and "Optional alcohol".
</p>
<p>
  The alcoholic cocktails are cocktails that have some percentage of alcohol, the non alcoholic cocktails don't have alcohol and optional alcohol cocktails could have alcohol or not.
</p>
<p>
  In this example, we are going to show alcoholic cocktails. So we just have to click on the "Alcoholic" option in the type list.
</p>

![Screen Shot Seaching by type 2][screenshot-search-type2]

<p>
  At the next screen, we can see the alcoholic cocktails that we have.
<p>
  If you pay attention to the filters at the left side of the screen, you can see that the "Alcoholic" option in the drink type list is selected. So if you want to see the other drink types options, you just have to click on them.
</p>
<p>
  As result of the search, we have 100 alcoholic cocktails to show.
</p>

![Screen Shot Seaching by type 3][screenshot-search-type3]

### Search cocktail by category
<p>
  To search a cocktail by its category, we have to click on the "category" button in the navbar.
</p>

![Screen Shot Seaching by category 1][screenshot-search-category1]

<p>
  At this new screen, we can see the cocktails category list. There are eleven different categories.
</p>
<p>
  In this example, we want to check the cocktails that belong to the "ordinary drink" category. So we click on the "ordinary drink" option in the categories list.
</p>

![Screen Shot Seaching by category 2][screenshot-search-category2]

<p>
  In this screen, we can see all the ordinary drink cocktails.
<p>
  If you pay attention to the filters at the left side of the screen, you can see that the "Ordinary drink" option in the category list is selected. So if you want to see the other categories options, you just have to click on them.
</p>
<p>
  In this case, we have 100 cocktails that belong to the "ordinary drink" category.
</p>

![Screen Shot Seaching by category 3][screenshot-search-category3]

### Search cocktail by ingredient
<p>
  To start to search a cocktail by its ingredient, we have to click on the "ingredient" button in the navbar.
</p>

![Screen Shot Seaching by ingredient 1][screenshot-search-ingredient1]

<p>
  In this screen, we can see a list of the different ingredient that are been used in the cocktails that we have registered.
</p>
<p>
  In this example, we are going to show cocktails that use "7-Up" as ingredient. So we just have to click on the "7-Up" card in the ingredient list.
</p>

![Screen Shot Seaching by ingredient 2][screenshot-search-ingredient2]


<p>
  At the new screen, we can see all the cocktails that use "7-Up" in their preparation.
<p>
  If you pay attention to the filters at the left side of the screen, you can see that the "7-Up" option in the ingredient list is selected. So if you want to see the other ingredient options, you just have to click on them.
</p>
<p>
  In this case, we just have 4 cocktails that have "7-Up" as one of their ingredients.
</p>

![Screen Shot Seaching by ingredient 3][screenshot-search-ingredient3]

### Filter results by type
<p>
  If we want to filter the results by cocktail type, we have to start searching cocktails using any other parameter.
</p>
<p>
  In this example, we have searched cocktails that have the word "coffee" on their names and we want to see how many of them have alcohol. So in the search result page, at the left controls, we click on the alcoholic option in the drink type list.
</p>

![Screen Shot Filer Results by type 1][screenshot-filter-type1]

<p>
  At the time that we clicked the option, we can observe that the cocktails displayed have changed. That is because it is showing cocktails that have "coffee" on their name and are alcoholic cocktails.
</p>
<p>
  As result of this filter, we have found 9 coffees that have alcohol. 
</p>

![Screen Shot Filer Results by type 2][screenshot-filter-type2]

### Filter results by category
<p>
  If we want to filter the results by cocktail category, we have to start searching cocktails using any other parameter.
</p>
<p>
  In this example, we have searched cocktails that have the word "coffee" on their names and we want to see how many of them belong to the "ordinary drink" category. So in the search result page, at the left controls, we click on the "ordinary drink" option in the category type list.
</p>

![Screen Shot Filer Results by category 1][screenshot-filter-category1]

<p>
  Once we have clicked the option, we can observe that the cocktails displayed have changed. That is because it is showing cocktails that have "coffee" on their name and that belongs to the "ordinary drink" category.
</p>
<p>
  We can observe that only one coffee that belong to the "ordinary drink" category. 
</p>

![Screen Shot Filer Results by category 2][screenshot-filter-category2]

### Filter results by ingredient
<p>
  To filter the search results by their ingredient, we have to start searching cocktails using any other parameter.
</p>
<p>
  In this example, we have searched cocktails that have 'alcoholic' on their type and we want to see how many of them use "amaretto" as ingredient in their preparation. So in the search result page, at the left controls, we click on the "amaretto" option in the ingredient type list.
</p>

![Screen Shot Filer Results by ingredient 1][screenshot-filter-ingredient1]

<p>
  At time that we have clicked the option, we can observe that the cocktails displayed have changed. That is because it is showing alcoholic cocktails that have "amaretto" as one of their ingredients.
</p>

![Screen Shot Filer Results by ingredient 2][screenshot-filter-ingredient2]

### Show cocktail information
<p>
  If we want more information about any cocktail, we only have to click on it in the seach cocktail page.
</p>
<p>
  In this example, we want to see more information about the cocktail named "110 in the shade". So we click on it.
</p>

![Screen Shot Cocktail Information 1][screenshot-show-cocktail-info1]

<p>
 In this new screen, we can see more information about the cocktail. Their name, category, type, type of glass used to serve it, preparation instruction and a list of ingredients with their measure
</p>

![Screen Shot Cocktail Information 2][screenshot-show-cocktail-info2]

### Show ingredient information
<p>
  If we want more information about certain ingredient, we only have to click on it in the cocktail detail page.
</p>
<p>
  In this example, we are in the cocktail which name is "110 in the shade" information page. In this page, we want more information about an ingredient called "Lager". So we click on it in the ingredient list. 
</p>

![Screen Shot Ingredient Information 1][screenshot-show-ingredient-info1]

<p>
 In this new screen, we can see more information about the ingredient "Lager". Their name, category, if it has alcohol, their alcohol by volume and description. Also we have a button to search cocktails that use this ingredient on their preparation. 
</p>

![Screen Shot Ingredient Information 2][screenshot-show-ingredient-info2]

### Adapted to small devices
<p>
 One of the fundamental goals of this website is to be able to be displayed on any device. So we started its design having in mind the mobile first concept.
</p>
<p>
 In order to that, we designed our home page to be very simple. So as it increases its width, we add more elements and we adapted them as long the width increase.
</p>
<p align="center">
  <img src="readme-images/mobilefirst-1.JPG" alt="Logo" width="500" height="450">
</p>
<p>
  To save more space we hide navbar button within a collapse element that can be open using a toggle button. Thank to this method the user can access to this controls when they need them or hide them when they aren´t useful. 
</p>
<p align="center">
  <img src="readme-images/mobilefirst-2.JPG" alt="Logo" width="500" height="450">
</p>
<p>
  In the search result page, we have the same problem that we have in the navbar. To solve it, we hide the filters controls to give all the space to show the search results in a better way. But we left a toggle button so the users are able to access to the filter controls if need them.
</p>
<p align="center">
  <img src="readme-images/mobilefirst-3.JPG" alt="Logo" width="500" height="450">
</p>
<p>
  We use a offcanvas element to show the filter controls. Thank to this technique, the user can see the control properly and make of them without any problem. 
</p>
<p align="center">
  <img src="readme-images/mobilefirst-4.JPG" alt="Logo" width="500" height="450">
</p>
<p>
 The pages that show information about cocktails and ingredients are ready to show all the information that they have in a proper way. Independently of user's device.
</p>
<p align="center">
  <img src="readme-images/mobilefirst-5.JPG" alt="Logo" width="325" height="470">
</p>

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/mutazen/Your-cocktail/issues) for a list of proposed features (and known issues).


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact
<p>
  Daniel Saavedra - https://www.linkedin.com/in/danielsavgem/
</p>
<p>
  Jeremy Camacho - https://www.linkedin.com/in/jeremycamacholugo/
</p>
<p>
  Project Link: https://github.com/mutazen/Your-cocktail
</p>


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)

## Special thanks

This website initially was a result of an exercise of Reboot Academy's bootcamp (ed. May-Jul 2021) but we keep working on it, giving it more functionalities and making it better because we loved the idea and we used it to test the skills that we learned. So we want to thank our instructors for their support and their patience. Thank you guys, you are the best!

We want to thank to @othneildrew for share their template for this readme. 

<p align="center">
  https://github.com/othneildrew/Best-README-Template
</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/mutazen/gestion-citas-access-2007.svg?style=for-the-badge
[contributors-url]: https://github.com/mutazen/gestion-citas-access-2007/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/mutazen/gestion-citas-access-2007.svg?style=for-the-badge
[forks-url]: https://github.com/mutazen/gestion-citas-access-2007/network/members
[stars-shield]: https://img.shields.io/github/stars/mutazen/gestion-citas-access-2007.svg?style=for-the-badge
[stars-url]: https://github.com/mutazen/gestion-citas-access-2007/stargazers
[issues-shield]: https://img.shields.io/github/issues/mutazen/gestion-citas-access-2007.svg?style=for-the-badge
[issues-url]: https://github.com/mutazen/gestion-citas-access-2007/issues
[license-shield]: https://img.shields.io/github/license/mutazen/gestion-citas-access-2007.svg?style=for-the-badge&
[license-url]: https://github.com/mutazen/gestion-citas-access-2007/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/jeremycamacholugo/
[product-screenshot]: readme-images/image-1.png
[configuracion-1]: readme-images/configuracion/configuracion-1.png
[configuracion-2]: readme-images/configuracion/configuracion-2.png
[configuracion-3]: readme-images/configuracion/configuracion-3.png
[screenshot-search-type1]: readme-images/screenshot-search-type1.jpg
[screenshot-search-type2]: readme-images/screenshot-search-type2.jpg
[screenshot-search-type3]: readme-images/screenshot-search-type3.jpg
[screenshot-search-category1]: readme-images/screenshot-search-category1.jpg
[screenshot-search-category2]: readme-images/screenshot-search-category2.jpg
[screenshot-search-category3]: readme-images/screenshot-search-category3.jpg
[screenshot-search-ingredient1]: readme-images/screenshot-search-ingredient1.jpg
[screenshot-search-ingredient2]: readme-images/screenshot-search-ingredient2.jpg
[screenshot-search-ingredient3]: readme-images/screenshot-search-ingredient3.jpg
[screenshot-filter-type1]: readme-images/screenshot-filter-type1.jpg
[screenshot-filter-type2]: readme-images/screenshot-filter-type2.jpg
[screenshot-filter-category1]: readme-images/screenshot-filter-category1.jpg
[screenshot-filter-category2]: readme-images/screenshot-filter-category2.jpg
[screenshot-filter-ingredient1]: readme-images/screenshot-filter-ingredient1.jpg
[screenshot-filter-ingredient2]: readme-images/screenshot-filter-ingredient2.jpg
[screenshot-show-cocktail-info1]: readme-images/screenshot-show-cocktail-info1.jpg
[screenshot-show-cocktail-info2]: readme-images/screenshot-show-cocktail-info2.jpg
[screenshot-show-ingredient-info1]: readme-images/screenshot-show-ingredient-info1.jpg
[screenshot-show-ingredient-info2]: readme-images/screenshot-show-ingredient-info2.jpg
