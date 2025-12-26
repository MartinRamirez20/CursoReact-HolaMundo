# CURSO REACT POR 'HolaMundo'

## Temario

- Anatomia (¿Que es y de que se trata?)
- Componentes
- Propiedades
- Gestion de estado de componentes
- Herramientas de depuración
- Estilo
- Formularios (Uncontrolled y Controlled)
- Conección a servidores
- React Query
- Gestion global de estado
- React Router

Veremos 3 proyectos y algunos ejercicios

## Requisitos

Este curso cuenta con cierto requisitos, ya se deberia saber HTML, CSS y JavaScript el cual es fundamental.

De JavaScript deberiamos conocer:

- Clases
- Fatarrow functions
- Alcance de las funciones
- Fetch

Usaremos tambien TypeScript.

# Que es React

Es una biblioteca para construir interfaces web y nativas. Podemos usar REACT para crear aplicaciones web o aplicaciones moviles para Android o ios.

El Framework mas popular para la creacion de aplicaciones nativas es React-Native, pero este es para dispositivos moviles.

React es la biblioteca mas popular actualmente en el mercado.

Cada que creamos una aplicacion web tenemos que trabajar con el 'DOM', el cual es un arbol que contiene etiquetas, como 'head', 'body', donde a su vez podemos tener 'div', 'h1' o 'p'. Con JS podemos ir a buscar alguna de estar referencias con 'querySelector' o 'getElementById' con estos metodos podemos mantener las referencias de cada uno de los elementos, ya que le podemos asignar constantes donde podemos actualizar contenido, sin embargo, entre mas grande sea la aplicacion mantener actualizada la pagina unicamente con JS se convierte en algo repetitivo y tedioso, es por eso que se creo React.

React se encargara de actualizar la interfaz del usuario.

Nuestra aplicacion se veria con un componente padre o raiz que se dividiran en componentes como titulo, navegacion, o links. Asi podemos empezar a reutilizar componentes ya creados haciendo que nuestra aplicación sea mas facil de mantener, ya que se reutiliza mucho mas el codigo.

React se compara tambien con 'Angular' y 'Vue', sin embargo estos ultimos son Frameworks, mientras que 'React' es una biblioteca. React solo se encarga de actualizar la vista de las aplicaciones, es decir, lo que ve el usuario. Angular y Vue, tienen mas herramientas como gestión de rutas, gestión de estado y tambien se encargan de actualizar la vista de las aplicaciones.

# Configuración

Para poder usar React debemos tener instalado Node, en especial una version mayor a la 16.
Url de descarga desde la pagina oficial: https://nodejs.org/en/download/current

Adicionalmente si usas Visual Studio Code deberas instalar la extensión de Prettier: https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode

# Creacion APP React

Para la creación de este proyecto se solía usar 'create-react-app' hasta que llego 'vite' la cual es mas rapida y que crea empaquetados mas pequeños, haciendo esta la herramientra predilecta para iniciar nuestros proyectos.

Abriendo la terminal de nuestro VScode vamos a ejecutar el siguiente comando: 'npm create vite @latest-version nombre-proyecto'

Le diremos que si con 'y' despues le colocaremos un nombre a nuestro paquete. Seleccionaremos como Framework 'React' y como variante 'TypeScript'. Ustedes pueden seleccionar diferentes modos para probar tambien. Install with npm and start now?: Yes. Y luego 'ctrl + c' para detener la ejecucion.

## Estructura del proyecto

Ahora miraremos la estructura del proyecto que hemos generado con los pasos anteriores:

- mode_modules: contiene todas las dependencias de nuestro proyecto, como react y typescript, nunca deberiamos tocar ese directorio.
- public: mantiene todos los archivos que son publicos y a los que el usuario deberia poder acceder. Pueden ser imagenes del logo del proyecto o videos y documentos que querramos que el usuario descargue.
- src: Contiene todos los archivos de nuestro codigo fuente, aqui pasaremos el 99.9% del tiempo de nuestro desarrollo.
- index.html: Este archivo contiene nuestro index principal de nuestro proyecto. Podemos ver un 'div' con id 'root'. Un 'script' que se encargara de tomar el codigo fuente de nuestra aplicacion y colocar la app dentro de la etiqueta 'root'.
- package.json: Se guardan las dependencias instaladas y que instalemos despues.
- tsconfig.json y tsconfig.node.json: Estos archivos configuran TypeScript y si comportamiento.

# Componentes

En src abriremos 'App.tsx'.
