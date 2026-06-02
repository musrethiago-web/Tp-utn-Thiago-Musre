

Clon de Interfaz: Contador de Caracteres (Character Counter)
1. Propósito del Proyecto
El objetivo de este proyecto consistió en replicar visualmente el diseño de una interfaz web de análisis de texto en tiempo real. La restricción fundamental fue estructurar y estilar la aplicación únicamente con HTML5 y CSS3, dejando de lado en su totalidad de JavaScript.

El desarrollo se enfocó en lograr un maquetado semántico limpio, un flujo de diseño fluido mediante propiedades modernas (como Grid y Flexbox), adaptabilidad en dispositivos móviles y una estilización avanzada utilizando variables de entorno globales.

2. Tecnologías Utilizados
HTML5

CSS3

Google Fonts

Remove.bg

Microsoft Copilot

3. Estructura y Organización del HTML
El archivo index.html cuenta con una división modular limpia gracias a las etiquetas contenedoras de HTML5:

<header class="header">: Barra de navegación superior que encapsula la identidad de la marca (logotipo .logo y el texto Character Counter) junto con el botón funcional interactivo para alternar el esquema cromático (cambiar tema).

<main class="analyze">: Núcleo de la aplicación distribuido de forma secuencial:

Encabezado principal: Etiqueta <h1> estilizada con saltos de línea para el impacto del texto introductorio.

Captura de datos: Elemento <textarea> configurado para la entrada de texto del usuario.

.control-panel: Contenedor de utilidades que agrupa un formulario (.inputs) con dos inputs de tipo checkbox (exclusión de espacios y límites de caracteres) y un elemento <p class="reading-time"> para proyectar el tiempo aproximado de lectura.

.stats: Módulo general de analíticas subdividido en:

.cards: Bloques <article> individuales por clase (.purple-card, .orange-card, .pink-card) para los contadores cuantitativos. (Nota: Los atributos alt de las imágenes se configuraron vacíos intencionalmente al ser recursos decorativos de fondo desde CSS).

.stadistics: Sección dedicada al desglose "Letter Density", construida con bloques estructurales .Letter-density que combinan elementos <span> para los caracteres y porcentajes con barras nativas <progress>. Finaliza con un botón sin bordes para expandir los datos.


. Variables Globales y Reset (:root)
Se centralizó la paleta de colores "tech" (fondos oscuros, textos de alta legibilidad y acentos vibrantes para los componentes destacados) utilizando variables CSS nativas para asegurar un código mantenible y escalable:

Fondos base y contenedores: --bg-main (#12131A), --bg-card (#1C1F2A).

Tipografía: --text-primary y --text-secondary.

Acentos cromáticos de tarjetas: --card-purple, --card-orange, --card-coral y --progress-bar.


4. Desafíos Técnicos

El principal inconveniente durante la estilización con CSS3 se concentró en la sección `.cards`. Específicamente, el problema radicó en la flexibilidad y el comportamiento del contenedor al intentar que las tarjetas ocuparan el espacio proporcional correspondiente en pantalla. 

Las consultas realizadas a la IA para resolver este bug sugerían modificaciones masivas que alteraban la integridad de todo el documento de estilos. Para no perder el control sobre el flujo del trabajo, decidí conservar mi código base. Me gustaria si es posible que me pudieras corregir y explicar esa parte del trabajo para ver donde se encuentra mi error.

Por otro lado, tuvo problemas tambien con la creacion y organizacion de los commits. Me pasó muchas veces que me encontraba escribiendo codigo y me olvidaba de commitearlo, por lo tanto hay saltos grandes de codigo de un commit a otro. Tambien se puede ver que en un commit el codigo esta escrito de una manera y al siguiente commit esta modificado el codigo, ya que con la ayuda de la IA iba corrigiendo errores que iba teniendo.

Adjunto foto de como quedó el maquetado.

![image alt](https://github.com/musrethiago-web/Tp-utn-Thiago-Musre/blob/69dad6999ef5a6904da5468cf864ccd9d2bc815d/image.png)
