# Cifrado César

## Índice

* [1. Preámbulo](#1-preámbulo)
* [2. Resumen del proyecto](#2-resumen-del-proyecto)
* [3. Uso de la app](#3-Uso-de-la-App)
* [4. Prototipo de papel](#4-Prototipo-de-papel)
* [5. Prototipo Balsamiq](#5-Prototipo-Balsamiq)

***

## 1. Preámbulo

Cifrar significa codificar. El [cifrado César](https://en.wikipedia.org/wiki/Caesar_cipher)
es uno de los primeros métodos de cifrado conocidos. El emperador romano Julio
César lo usaba para enviar órdenes secretas a sus generales en los campos de
batalla.

![caeser-cipher](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2b/Caesar3.svg/2000px-Caesar3.svg.png)

El cifrado césar es una de las técnicas más simples para cifrar un mensaje. Es
un tipo de cifrado por sustitución, es decir que cada letra del texto original
es reemplazada por otra que se encuentra un número fijo de posiciones
(desplazamiento) más adelante en el mismo alfabeto.

Por ejemplo, si usamos un desplazamiento (_offset_) de 3 posiciones:

* La letra A se cifra como D.
* La palabra CASA se cifra como FDVD.
* Alfabeto sin cifrar: A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
* Alfabeto cifrado: D E F G H I J K L M N O P Q R S T U V W X Y Z A B C

En la actualidad, todos los cifrados de sustitución simple se descifran con
mucha facilidad y, aunque en la práctica no ofrecen mucha seguridad en la
comunicación por sí mismos; el cifrado César sí puede formar parte de sistemas
más complejos de codificación, como el cifrado Vigenère, e incluso tiene
aplicación en el sistema ROT13.

## 2. EL PROYECTO

En este proyecto crearé una aplicación
web que servirá para que el usuario pueda cifrar y descifrar un texto indicando
un desplazamiento específico de caracteres (_offset_).

La temática es kids, una web disfrazada de juego para: 

* Mensajería secreta para niños que sufren cualquier tipo de abuso o maltrato infantil.

![cipher](https://user-images.githubusercontent.com/68177371/99621658-7665aa80-29f6-11eb-8adc-e193328c5ecf.jpeg)

# CRIPTOMANÍA KIDS

En criptografía, el cifrado César, también conocido como cifrado por desplazamiento, código de César o desplazamiento de César, es una de las técnicas decodificación más simples y más usadas. Es un tipo de cifrado por sustitución en el que una letra en el texto original es reemplazada por otra letra que se encuentra un número fijo de posiciones más adelante en el alfabeto.

## 3. ¿Cómo usar la app Criptomanía-Kids

### INSTRUCCIONES DE USO:

*El primer paso es buscar Criptomanía-Kids, una vez encontrada, se procede según lo que el usuario desea a:*

1.PASOS PARA CIFRAR
- Escribe lo que deseas cifar.
- Elige tu número favorito
- Dale click en el botón "JUGAR CIFRAR"
- Verás el mensaje cifrado
- Darle al botón enviar

2.PASOS PARA DESCIFRAR
- Escribe lo que deseas descifar.
- Elige tu número favorito
- Dale click en el botón "JUGAR DESCIFRAR"
- Verás el mensaje descifrado
- Darle al botón enviar
  

El siguiente proyecto ha sido pensado para poner un alto a los actos de violencia, en contra de los niños, la 
idea es que sea lo más parecido a un juego, para evitar ser descubierto. La iniciativa puede ser planteada al 
gobierno, aunque hoy en día el código césar no es tan seguro, se podría implementar al proyecto símbología para 
darle mayor seguridad.

>Los principales usuarios son niñ@s que sufren cualquier tipo de violencia/agresión, tanto para su persona como en sus casas.

>A través de una app, disfrazada de juego infantil, los niños podrán enviar mensajes de ayudar para salvaguardar su bienestar, 
encriptando sus mensajes para evitar ser descubiertos por su agresor.
Ministerio de protección del niño, niña y adolescente)

#### El producto soluciona los problemas/necesidades de dichos usuarios, considerando lo sgte:
- Canalizar mensajes de ayuda.
- Disminuir la violencia en los hogares.
- Brindar ayuda psicológica y evitar futuros actos de violencia.

## 4.PROTOTIPO DE PAPEL
Mi primer prototio en papel, teniendo en cuenta las historias de usuario

![Primerprototipo](https://user-images.githubusercontent.com/68177371/99622018-4a96f480-29f7-11eb-85a3-8c925890ec77.jpeg)


El feedback en cuanto al proyecto: 
* Mis compañeras de squad indican que les agrada la idea y el objetivo del uso de la app cipher.
* Una de las coach: Génesis, opinó que le gusta la idea, y que ella trabaja en proyectos para niños.
* En mi primer demo, las chicas opinaron que les gustó el fondo y los colores.
* En un 2do demo me sugirieron colocar los botones entre el cuadro de inicio de texto y el cuadro de resultados, ya que estaban ubicados en la parte inferior.
Me gustó recibir feedback, siento que ayudó mucho a la mejora del proyecto. 

***En casa testee el proyecto con mi hijo, al cual le gustó y dijo que parecía un juego***

## 5. PROTOTIPO BALSAMIQ

Imagen del prototipo final.
  
Este es el prototipo final de mi proyecto, realizado en balsamiq

![balsamiq](https://user-images.githubusercontent.com/68177371/99621870-ed02a800-29f6-11eb-91b4-1361e5f6d4b1.jpeg)

EL FLUJO DEL PROYECTO

![Diagrama](src/imagen/diagrama.jpeg)

  
  




<!--##### `src/index.html` 

  Este es el punto de entrada a tu aplicación. Este archivo
  debe contener tu _markup_ (HTML) e incluir el CSS y JavaScript necesario.
  
##### `src/cipher.js`
  Acá debes implementar el objeto `cipher`, el cual ya está
  _exportado_ en el _boilerplate_. Este objeto (`cipher`) debe contener dos
  métodos:
  - `cipher.encode(offset, string)`: `offset` es el número de posiciones que
    queremos mover a la derecha en el alfabeto y `string` el mensaje (texto)
    que queremos cifrar.
  - `cipher.decode(offset, string)`: `offset` es el número de posiciones que
    queremos mover a la izquierda en el alfabeto y `string` el mensaje
    (texto) que queremos descifrar.
##### `src/index.js`
  Acá debes escuchar eventos del DOM, invocar `cipher.encode()`
  o `cipher.decode()` según sea necesario y actualizar el resultado en la UI.
##### `test/cipher.spec.js`
  Este archivo contiene algunos tests de ejemplo y acá
  tendrás que implementar los tests para `cipher.encode()` y `cipher.decode()`.

## 6. Hacker edition

Las secciones llamadas _Hacker Edition_ son **opcionales**. Si **terminaste**
con todo lo anterior y te queda tiempo, intenta completarlas. Así podrás
profundizar y/o ejercitar más sobre los objetivos de aprendizaje del proyecto.

La descripción general de este proyecto no menciona qué pasaría con las letras
minúsculas y otros caracteres (como espacios, puntuación, ñ, ...). El
boilerplate incluye algunos tests (comentados en principio) que puedes usar como
punto de partida para implementar el soporte para estos casos.

Tampoco se menciona qué pasaría si el offset fuera negativo. Como parte del
hacker edition te invitamos a explorar también esta caso por tu cuenta.

## 7. Consideraciones técnicas

La lógica del proyecto debe estar implementada completamente en JavaScript. En
este proyecto NO está permitido usar librerías o frameworks, solo JavaScript puro
también conocido como Vanilla JavaScript.

No se debe utilizar la _pseudo-variable_ `this`.

Los tests unitarios deben cubrir un mínimo del 70% de _statements_, _functions_
y _lines_, y un mínimo del 50% de _branches_. El _boilerplate_ ya contiene el
setup y configuración necesaria para ejecutar los tests (pruebas) así como _code
coverage_ para ver el nivel de cobertura de los tests usando el comando `npm
test`.

El _boilerplate_ incluye tests (pruebas) de ejemplo como punto de partida.

Para comenzar este proyecto tendrás que hacer un _fork_ y _clonar_ este
repositorio que contiene el _boilerplate_.

El _boilerplate_ contiene una estructura de archivos como punto de partida así
como toda la configuración de dependencias y tests de ejemplo:

```text
./
├── .babelrc
├── .editorconfig
├── .eslintrc
├── .gitignore
├── README.md
├── package.json
├── src
│   ├── cipher.js
│   ├── index.html
│   ├── index.js
│   └── style.css
└── test
    ├── .eslintrc
    └── cipher.spec.js
```

El _boilerplate_ incluye tareas que ejecutan [eslint](https://eslint.org/) y
[htmlhint](https://github.com/yaniswang/HTMLHint) para verificar el `HTML` y
`JavaScript` con respecto a una guías de estilos. Ambas tareas se ejecutan
automáticamente antes de ejecutar las pruebas (tests) cuando usamos el comando
`npm run test`. En el caso de `JavaScript` estamos usando un archivo de
configuración de `eslint` que se llama `.eslintrc` que contiene un mínimo de
información sobre el parser que usar (qué version de JavaScript/ECMAScript), el
entorno (browser en este caso) y las [reglas recomendadas (`"eslint:recommended"`)](https://eslint.org/docs/rules/).
En cuanto a reglas/guías de estilo en sí,
usaremos las recomendaciones _por defecto_ de tanto `eslint` como `htmlhint`.

***

## 8. Pistas, tips y lecturas complementarias

### Primeros pasos

1. Antes que nada, asegúrate de tener un :pencil: editor de texto en
  condiciones, algo como [Atom](https://atom.io/) o
  [Code](https://code.visualstudio.com/).
2. Para ejecutar los comandos a continuación necesitarás una :shell:
  [UNIX Shell](https://github.com/Laboratoria/bootcamp/tree/master/topics/shell),
  que es un programita que interpreta líneas de comando (command-line
  interpreter) así como tener [git](https://github.com/Laboratoria/bootcamp/tree/master/topics/scm/01-git)
  instalado. Si usas un sistema operativo "UNIX-like", como GNU/Linux o MacOS,
  ya tienes una _shell_ (terminal) instalada por defecto (y probablemente `git`
  también). Si usas Windows puedes usar la versión completa de [Cmder](https://cmder.net/)
  que incluye [Git bash](https://git-scm.com/download/win) y si tienes Windows 10
  o superior puedes usar [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
3. Una de las integrantes del equipo debe realizar un :fork_and_knife:
  [fork](https://help.github.com/articles/fork-a-repo/) del repo de tu cohort,
  tus _coaches_ te compartirán un _link_ a un repo y te darán acceso de lectura
  en ese repo. La otra integrante del equipo deber hacer un fork **del
  repositorio de su compañera** y
  [configurar](https://gist.github.com/BCasal/026e4c7f5c71418485c1) un `remote`
  hacia el mismo.
4. :arrow_down: [Clona](https://help.github.com/articles/cloning-a-repository/)
  tu _fork_ a tu computadora (copia local).
5. 📦 Instala las dependencias del proyecto con el comando `npm install`. Esto
  asume que has instalado [Node.js](https://nodejs.org/) (que incluye [npm](https://docs.npmjs.com/)).
6. Si todo ha ido bien, deberías poder ejecutar las :traffic_light:
  pruebas unitarias (unit tests) con el comando `npm test`.
7. Para ver la interfaz de tu programa en el navegador, usa el comando
  `npm start` para arrancar el servidor web y dirígete a
  `http://localhost:5000` en tu navegador.
8. A codear se ha dicho! :rocket:

### Recursos y temas relacionados

A continuación un video de Michelle que te lleva a través de la fórmula
matemática del Cifrado César y un par de cosas más que debes saber para
resolver este proyecto. ¡Escúchala con detenimiento y sigue sus consejos! :)

[![tips caesar cipher](https://img.youtube.com/vi/zd8eVrXhs7Y/0.jpg)](https://www.youtube.com/watch?v=zd8eVrXhs7Y)

[Link](https://www.youtube.com/watch?v=zd8eVrXhs7Y)

También una metodología para empezar a desarrollar tareas con JavaScript:

[![Resolución de problemas con JavaScript](http://i3.ytimg.com/vi/lYfEmhLmu7A/hqdefault.jpg)](https://www.youtube.com/watch?v=lYfEmhLmu7A)

[Link](https://www.youtube.com/watch?v=lYfEmhLmu7A)

Terminal y shell de UNIX:

[![Playlist de Terminal y shell de UNIX](https://img.youtube.com/vi/GB35Eyb-J4c/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

Control de versiones y trabajo colaborativo con Git y GitHub:

[![Playlist de control de versiones y trabajo colaborativo](https://img.youtube.com/vi/F1EoBbvhaqU/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

Diseño de experiencia de usuario (User Experience Design):

* Ideación
* Prototipado (sketching)
* Testeo e Iteración

Desarrollo Front-end:

* Valores
* Tipos
* Variables
* Control de flujo
* Tests unitarios
* [Aprende más sobre `charCodeAt()`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/String/charCodeAt)
* [Aprende más sobre `String.fromCharCode()`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/String/fromCharCode)
* [Aprende más sobre `ASCII`](http://conceptodefinicion.de/ascii/)
* [Documentación de NPM](https://docs.npmjs.com/)

Organización del Trabajo:

* [Metodologías Ágiles](https://www.youtube.com/watch?v=v3fLx7VHxGM)
* [Scrum en menos de 2 minutos](https://www.youtube.com/watch?v=TRcReyRYIMg)
* [Scrum en Detalle](https://www.youtube.com/watch?v=nOlwF3HRrAY&t=297s). No
  esperamos que hagas todo eso desde este proyecto. Iremos profundizando poco a
  poco a lo largo del -_bootcamp_.
* [Guía para Cifrado César](https://docs.google.com/presentation/d/e/2PACX-1vTQ7-8LZDHrT4Y6AOBN72Nkfz1eJAeseBHpcHX8BSq0aFCFoZmuMjluMeyFNgK9ISKxTz0H03yGfJiT/pub?start=false&loop=false&delayms=60000)

-->
