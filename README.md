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
          <a href="#ver-citas">Ver citas</a>
          <ul>
            <li>
              <a href="#ver-citas-de-un-día-en-concreto">Ver citas de un día en concreto</a>
            </li>
            <li>
              <a href="#ver-citas-de-la-semana-anterior-o-posterior">Ver citas de la semana anterior o posterior</a>
            </li>
            <li>
              <a href="#ver-citas-del-mes-anterior-o-posterior">Ver citas del mes anterior o posterior</a>
            </li>
            <li>
              <a href="#ver-citas-de-una-área-determinada">Ver citas de un área determinada</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#crear-cita">Crear cita</a>
        </li>
        <li>
          <a href="#modificar-cita">Modificar cita</a>
        </li>
        <li>
          <a href="#eliminar-cita">Eliminar cita</a>
        </li>
        <li>
          <a href="#copiar-cita">Copiar cita</a>
        </li>
        <li>
          <a href="#buscar-cita">Buscar cita</a>
          <ul>
            <li>
              <a href="#buscar-por-nombre">Buscar por nombre</a>
            </li>
            <li>
              <a href="#buscar-por-apellidos">Buscar por apellidos</a>
            </li>
            <li>
              <a href="#buscar-por-dni">Buscar por DNI</a>
            </li>
            <li>
              <a href="#buscar-por-nie">Buscar por NIE</a>
            </li>
            <li>
              <a href="#buscar-por-pasaporte">Buscar por pasaporte</a>
            </li>
            <li>
              <a href="#buscar-por-teléfono">Buscar por teléfono</a>
            </li>
            <li>
              <a href="#buscar-por-fecha">Buscar por fecha</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#asignar-asistencia">Asignar asistencia</a>
        </li>
        <li>
          <a href="#designar-día">Designar dia</a>
          <ul>
            <li>
              <a href="#designar-día-para-atender-citas">Designar dia para atender citas</a>
            </li>
            <li>
              <a href="#designar-día-como-festivo">Designar dia como festivo</a>
            </li>
            <li>
              <a href="#eliminar-designación">Eliminar designación</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#reservar-hora">Reservar hora</a>
          <ul>
            <li>
              <a href="#crear-reserva">Crear reserva</a>
            </li>
            <li>
              <a href="#ver-reserva">Ver reserva</a>
            </li>
            <li>
              <a href="#modificar-reserva">Modificar reserva</a>
            </li>
            <li>
              <a href="#eliminar-reserva">Eliminar reserva</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#imprimir-ficha-de-gestión-de-citas">Imprimir ficha de gestión de citas</a>
        </li>
      </ul>
    </li>
    <li><a href="#cronología">Cronología</a></li>
    <li><a href="#contribuciones">Contribuciones</a></li>
    <li><a href="#licencia">Licencia</a></li>
    <li><a href="#contacto">Contacto</a></li>
    <li><a href="#conocimientos">Conocimientos</a></li>
    <li><a href="#agradecimientos">Agradecimientos</a></li>
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
### Ver citas

Para poder ver las citas, partimos desde el menú principal de la solución. En él podemos indicar si quieremos ver las citas del turno de manaña o del turno de tarde.

![elegir turno en el menu principal][ver-cita-1]

Al hacer clic, se nos muestra la pantalla desde donde podemos ver las citas registradas para la semana actual.

![ver pantalla de citas][ver-cita-2]

#### Ver citas de un día en concreto

Si se quiere ver las citas de un día en concreto, se puede utilizar el calendario que se encuentra en la parte superior de la izquierda de la pantalla en la que se muestran las citas. Este calendario cuenta tambien con dos controles que permiten seleccionar el mes y el año que se muestran en el calendario.

![ver controles de calendario][ver-cita-3]

Si seleccionamos el mes y el año en los controles descritos anteriormente, el calendario cambiará para mostrar el mes del año indicado. Si hacemos clic en uno de los dias del calendario, se cambiarán las citas que se estaban mostrando para mostrar las citas de la semana al que pertenece el dia en el que se haya hecho clic en el calendario.

![modificar controles de calendario][ver-cita-4]

#### Ver citas de la semana anterior o posterior
Para poder ver las citas de la semana anterior o posterior, se puede hacer uso de los controles de la pantalla de las citas que se marcan en la siguiente imagen. Si se hace clic en el botón de la izquierda, se muestran las citas de la semana anterior y si se hace clic en el botón de la derecha, se muestra las citas de la semana posterior.

![mostrar controles para ver citas semana anterior o posterior][ver-cita-5]

#### Ver citas del mes anterior o posterior

Si se quiere ver las citas del mes anterior o posterior, se puede utilizar los controles que se encuentran a los lados del calendario de la parte superior derecha de la pantalla en la que se muestran las citas. Si se hace clic en el botón izquierdo, se muestran las citas de la semana a la que pertenece el dia seleccionado del mes anterior y si se hace clic en el botón derecho, se muestran las citas del mes posterior.  

![mostrar controles para ver citas mes anterior o posterior][ver-cita-6]

#### Ver citas de una área determinada

Para ver las citas de un área determinada, se usa el control que acompaña a la etiqueta "Citas para". Al pulsar dicho control, se muestra una lista desplegable con todas las áreas que se gestionan. Si se pincha en en alguna, se cargarán las citas de la misma semana pertenecientes a la nueva área.

![mostrar controles para ver citas de un área][ver-cita-7]

### Crear cita

Si se quiere crear una nueva cita, se parte desde la pantalla en la que se muestran las citas en el que haya un día designado para poner citas. Para empezar a crear la cita, hacemos clic en uno de los recuadros blancos del dia asignado para citas.

![empezar a crear una cita][crear-cita-1]

Al hacer clic aparecerá una venta emergente para poner una nueva cita con la fecha del día seleccionado y la hora escogida. En esta pantalla, introducimos los datos del asistente de la cita. Como mínimo es necesario introducir un nombre, apellidos y un número de teléfono. Si introducimos un DNI o un NIE, no se podrá regitrar la cita hasta que estos tengan el formato correcto. Para poder terminar el proceso, hacemos clic en el botón "Guardar".

![rellenar los datos de una cita][crear-cita-2]

Una vez se ha creado la cita, esta aparecerá en el calendario, ocupando el recuadro en el que hemos hecho clic y mostrando el nombre, los apellidos y el primer número de teléfono que se ha introducido.

![ver cita creada][crear-cita-3]

### Modificar cita

Para modificar una cita, solo es necesario hacer clic en la cita a la que se quiera cambiar los datos desde la pantalla en la que se muestran las citas. Al hacer clic aparace una ventana emergente desde donde se puede realizar la modificación. Para poder guardar los cambios realizados, es necesario que la cita cuente como minimo con nombre, apellidos, un número de teléfono y que los DNI y NIE introducidos tengan un formato correcto. Y por último, hacemos clic en el botón "Actualizar" guardar los cambios.

![modificar los datos de una cita][modificar-cita-1]

### Eliminar cita

Si se quiere eliminar una cita, basta con hacer clic sobre la cita a eliminar desde la pantalla en la que se ven las citas. Al hacerlo, aparece una ventana emergente desde donde se cambia los datos de la cita. Si hacemos clic en el botón "Eliminar cita", saldrá otra ventana emergente donde se nos advierte que si aceptamos los datos se borrarán. Si dentro de esta ventana pulsamos el botón "Aceptar", la cita se eliminará y volveremos a la pantalla en la que se muestran las citas, donde no aparecerá la cita que hemos borrado.

![borrar una cita][borrar-cita-1]

### Copiar cita

Para copiar los datos de una cita y pegarlo en otro dia u hora, se hace clic con el botón derecho del ratón sobre la cita a copiar en la pantalla en la que se ven las citas. Al hacerlo, saldrá un menú contextual en el podemos hacer clic en la opción "Copiar cita". Si lo hacemos cargaremos los datos de la cita y podremos copiarla en cualquier otro lado.

![copiar una cita][copiar-cita-1]

Para pegar la cita que hemos seleccionado anteriormente, elegimos un recuadro en blanco de un dia que esté habilitado para poner cita y hacemos clic en el recuadro con el botón derecho de ratón. Al hacerlo, se mostrará un menú contextual y hacemos clic en la opción "Pegar cita".

![pegar una cita][copiar-cita-2]

Al hacerlo, los datos de la cita que estaban cargados se asignan al dia y la hora del recuadro. De esta forma, se ha creado una cita con los mismos datos que los de la cita que hemos copiado pero en la hora y dia pertencientes al recuadro que hemos seleccionado al pegar.  

![ver cita pegada][copiar-cita-3]

### Buscar cita

Para empezar a buscar citas, partimos desde la pantalla del menú principal, en ella pulsamos el botón de "Buscar citas".

![empezando a buscar citas][buscar-cita-1]

Al haber hecho clic, se mostrará una nueva venta en la que podremos buscar citas según diversos parámetros, ver sus resultados, ver los datos de la cita seleccionada o verla en el calendario.

![ver pantalla de buscar cita][buscar-cita-2]

#### Buscar por nombre

Para poder buscar una cita por nombre, partimos de la pantalla de buscar cita. En ella, escribimos el nombre del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "Nombre" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por nombre][buscar-cita-3]

#### Buscar por apellidos

Si queremos buscar una cita por apellidos, partimos de la pantalla de buscar cita. En ella, escribimos el nombre del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "Apellidos" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por apellidos][buscar-cita-4]

#### Buscar por DNI

Si queremos buscar una cita por DNI, partimos de la pantalla de buscar cita. En ella, escribimos el dni del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "DNI" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por dni][buscar-cita-5]

#### Buscar por NIE

Si queremos buscar una cita por NIE, partimos de la pantalla de buscar cita. En ella, escribimos el nie del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "NIE" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por nie][buscar-cita-6]

#### Buscar por pasaporte

Si queremos buscar una cita por pasaporte, partimos de la pantalla de buscar cita. En ella, escribimos el pasaporte del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "Pasaporte" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por pasaporte][buscar-cita-7]

#### Buscar por teléfono

Si queremos buscar una cita por teléfono, partimos de la pantalla de buscar cita. En ella, escribimos el teléfono del usuario cuya citas estamos buscando en el recuadro que acompaña a la etiqueta de "Teléfono" y pulsamos el botón "Buscar. Una vez hecho esto, aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por teléfono][buscar-cita-8]

#### Buscar por fecha

Si queremos buscar una cita por fecha, partimos de la pantalla de buscar cita. En ella, podemos seleccionar una fecha en el recuadro que acompaña a la etiqueta "Desde", haciendo uso de un control de calendario o escribiendo la fecha directamente. También es posible acortar la búsqueda, indicando la fecha hasta donde quiere que se deje de buscar. Una vez introducidos los parámetros, hacemos clic en el botón "Buscar" y aparecerá los resultados en la lista de la parte derecha de la pantalla.

![buscar cita por fecha][buscar-cita-9]

### Asignar asistencia

### Designar día

#### Designar día para atender citas

#### Designar día como festivo

#### Eliminar designación

### Reservar hora

#### Crear reserva

#### Ver reserva

#### Modificar reserva

#### Eliminar reserva

### Imprimir ficha de gestión de citas

<!-- ROADMAP -->
## Cronología

Vea [open issues](https://github.com/mutazen/gestion-citas-access-2007/issues) para ver una lista de las características propuestas y de los bugs conocidos.


<!-- CONTRIBUTING -->
## Contribuciones

Las contribuciones son lo que hace que la comunidad de "open source" sea un lugar increíble para aprender, inspirarse y crear. Cualquier contribución que se haga se **aprecia mucho**

1. Fork el proyecto.
2. Crear una nueva rama para la funcionalidad a añadir (`git checkout -b feature/AmazingFeature`)
3. Haz "commit" de los cambios realizados (`git commit -m 'Add some AmazingFeature'`)
4. Actualiza la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request



<!-- LICENSE -->
## Licencia

Distrubuido bajo la licencia  MIT. Vea `LICENCIA` para más información.

<!-- CONTACT -->
## Contacto
<p>
  Jeremy Camacho - https://www.linkedin.com/in/jeremycamacholugo/
</p>
<p>
  Project Link: https://github.com/mutazen/gestion-citas-access-2007
</p>


<!-- ACKNOWLEDGEMENTS -->
## Conocimientos
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)

## Agradecimientos

Quiero agredecer a @othneildrew por compartir la plantilla que se usó como base de este readme.

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
[ver-cita-1]: readme-images/ver-citas/ver-cita-1.png
[ver-cita-2]: readme-images/ver-citas/ver-cita-2.png
[ver-cita-3]: readme-images/ver-citas/ver-cita-3.png
[ver-cita-4]: readme-images/ver-citas/ver-cita-4.png
