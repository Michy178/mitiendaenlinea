# mitiendaenlinea MICHELLE



TECNOLÓGICO NACIONAL DE MÉXICO

INSTITUTO TECNOLÓGICO DE TLÁHUAC

“LA ESENCIA DE LA GRANDEZA RADICA EN SUS RAÍCES”

DEPARTAMENTO DE SISTEMAS Y COMPUTACIONALES
Ingeniería En Sistemas Computacionales


Título
Ensayo de MVC.

P R E S E N T A (N)

Hernández Ramírez Paola Michelle

ASESOR

Martín Cordero-Ocampo



   	 	Tláhuac, CDMX., marzo 2024

Tabla de contenido
Resumen	3
Introducción	4
Desarrollo temático	5
Conclusión	12
Referencias	13





















Resumen

El ensayo abordará el uso del patrón Modelo-Vista-Controlador (MVC) en el desarrollo de aplicaciones web, destacando su capacidad para crear sistemas escalables, mantenibles y fácilmente expandibles al separar las preocupaciones entre el modelo, la vista y el controlador. 
Este enfoque permite que múltiples desarrolladores trabajen simultáneamente en diferentes partes de la aplicación sin interferir entre sí. Se explicará cómo el patrón MVC organiza la lógica de negocio, la presentación de datos y la interacción del usuario en tres componentes principales: el modelo, que gestiona los datos y la lógica de negocio; la vista, que presenta los datos al usuario de manera comprensible; y el controlador, que actúa como intermediario entre el modelo y la vista, coordinando las acciones necesarias.
 Además, se menciona la importancia de las aplicaciones web en la comunicación empresa-cliente, su funcionamiento en un modelo cliente-servidor, su accesibilidad y facilidad de uso para los usuarios, así como su capacidad de crecimiento flexible. Este contexto será relevante para comprender cómo el patrón MVC se aplica en el desarrollo web, ofreciendo una estructura organizada y modular que facilita el mantenimiento, la escalabilidad y la reutilización del código, además de promover buenas prácticas de programación.













Introducción

El enfoque del Modelo-Vista-Controlador (MVC) ha evolucionado significativamente para convertirse en un pilar fundamental en el desarrollo contemporáneo de software. Su amplia aceptación y popularidad se deben en gran medida a los claros beneficios que aporta en términos de estructura, mantenibilidad y escalabilidad de las aplicaciones.
En un entorno donde la complejidad del desarrollo de software sigue en aumento, el patrón MVC proporciona una metodología clara y bien definida para abordar estos desafíos. Al separar de manera distintiva la lógica de negocio, la presentación de datos y la gestión de la interacción del usuario, MVC establece un marco que facilita la comprensión y el mantenimiento del código a lo largo del ciclo de vida del software.
El núcleo de MVC, el modelo, encapsula la lógica de negocio y la manipulación de datos. Esto garantiza una representación precisa y coherente de la información subyacente, independientemente de cómo se presente al usuario final. Definiendo de forma clara las reglas de negocio y la estructura de los datos, el modelo proporciona una base sólida para la construcción y expansión de la aplicación.











Desarrollo temático

 

El patrón MVC se utiliza para desarrollar aplicaciones escalables, mantenibles y fáciles de expandir. Al separar las preocupaciones, permite que varios desarrolladores trabajen simultáneamente en diferentes partes de la aplicación sin interferir entre sí.








Es importante mencionar ¿Que es una aplicación web?:
Es un software que se va a ejecutar en un navegador web y que permite a las empresas comunicarse con los clientes y ofrecer servicios de forma remota. Sus características principales son:
•	Cliente Servidor: una aplicación web funciona en un modelo cliente-servidor. El cliente por así decirlo (un navegador web) solicita información o realiza alguna acción, y el servidor va a procesar esa solicitud y proporciona respuestas.
•	Accesibilidad: Las aplicaciones web están al alcance de todos a través de diversos navegadores y dispositivos personales y empresariales.
•	Eficiencia en el desarrollo: La creación de aplicaciones web es un proceso simple y rentable, con una única versión compatible con todos los navegadores y dispositivos modernos.
•	Facilidad de uso para el usuario: No es necesario descargar las aplicaciones web, lo que las hace fácilmente accesibles para los usuarios. Además, reciben actualizaciones automáticas de software y seguridad.
•	Capacidad de crecimiento: Las empresas pueden ampliar su base de usuarios según sea necesario sin requerir infraestructura adicional.
Es relevante destacar esta parte sobre qué es una aplicación web, ya que el patrón MVC es ampliamente utilizado en el desarrollo web, ofreciendo una estructura organizada y modular que separa los componentes de una aplicación en tres principales: el Modelo, la Vista y el Controlador. Esta separación de preocupaciones facilita el mantenimiento, la escalabilidad y la reutilización del código, además de promover un diseño modular y una buena práctica de programación.
Componentes del MVC:
Modelo:
El Modelo representa la lógica de negocio y los datos de la aplicación. En esta capa se definen las estructuras de datos, las operaciones de acceso y modificación de los datos, así como las reglas de negocio. Es independiente de la interfaz de usuario y no tiene conocimiento sobre cómo se muestran los datos ni cómo se interactúa con ellos. Su función principal es gestionar los datos y proporcionar una interfaz para acceder a ellos.
Vista:
La Vista es la interfaz de usuario que presenta los datos al usuario y recibe las interacciones del usuario. Se encarga de mostrar la información de manera visualmente atractiva y comprensible, pero no realiza ningún cálculo ni manipulación de datos. En MVC, la Vista se mantiene separada del Modelo y del Controlador, lo que permite cambiar la apariencia o el diseño sin afectar la lógica subyacente de la aplicación.
Controlador:
El Controlador actúa como intermediario entre el Modelo y la Vista. Recibe las entradas del usuario a través de la Vista, interpreta esas entradas y coordina las acciones necesarias en el Modelo. También actualiza la Vista en función de los cambios en el Modelo. El Controlador encapsula la lógica de la aplicación y coordina las operaciones, pero no contiene lógica de presentación. Esto facilita la reutilización y la prueba de la lógica de negocio sin depender de la interfaz de usuario.

Una estructura básica de cómo se realiza el ordenamiento de carpetas de una app web en MVC es:











La carpeta app/ contiene la lógica de la aplicación.
controllers/: Contiene los controladores que manejan las solicitudes HTTP.
models/: Contiene los modelos que interactúan con la base de datos u otras fuentes de datos.
database.php: Configuración de la conexión a la base de datos.
views/: Contiene las plantillas HTML para renderizar la interfaz de usuario. Están organizadas por controlador para mantener la estructura limpia.
La carpeta public/ es la carpeta raíz del servidor web.
assets/: Contiene archivos estáticos como CSS, JavaScript e imágenes.
index.php: Punto de entrada de la aplicación que dirige las solicitudes a los controladores.
La carpeta config/ contiene archivos de configuración.
routes.php: Define las rutas de la aplicación, asociando URLs con controladores y acciones.
 Un ejemplo de la programación con php utilizando este modelo de negocio cada parte de cada carpeta queda así:
Controlador:
 
Modelo:
 

Vista:
 
Index:
  
Ventajas del MVC:
Separación de preocupaciones:
MVC divide la aplicación en componentes ya que ocupan de aspectos específicos, lo que facilita la comprensión y el mantenimiento del código. Cada componente tiene una responsabilidad clara y definida, lo que facilita la colaboración en equipos de desarrollo.
Reutilización de código:
Al separar la lógica de negocio de la presentación, es más fácil reutilizar componentes en diferentes partes de la aplicación o en diferentes aplicaciones. Por ejemplo, el mismo Modelo puede ser utilizado por diferentes Vistas con distintas interfaces de usuario.

Facilita las pruebas:
La separación de la lógica de negocio del código de presentación hace que sea más fácil probar cada componente por separado. Los modelos pueden ser probados independientemente de las vistas y los controladores, lo que facilita la escritura de pruebas unitarias y la detección de errores.
Flexibilidad y escalabilidad:
MVC facilita la evolución y la expansión de una aplicación a medida que los requisitos cambian o crecen. Los cambios en la interfaz de usuario no afectan al modelo subyacente, lo que permite realizar modificaciones con menor impacto en el resto del sistema.
En este diagrama contiene tres clases, controlador, modelo y vista con las relaciones de uso que existen entre ellas. El controlador usa los modelos y las vistas y las vistas usan los modelos. Generalmente el controlador trabajará con los modelos de la aplicación, seleccionando aquellos datos que requiere la vista. Entonces el controlador usa la vista para generar la salida, enviando los modelos adecuados a la vista para que pinte los datos que necesite en la salida al usuario.


	




 










Conclusión

En conclusión, el patrón Modelo-Vista-Controlador (MVC) es una herramienta importante en el desarrollo de software, brindando un enfoque sólido y adaptable para la creación de aplicaciones que perduren en el tiempo. Al estructurar las áreas de preocupación relacionadas con la lógica de negocio, la presentación de datos y la interacción del usuario, MVC establece un estándar de calidad que sigue siendo relevante en el cambiante paisaje tecnológico actual.
MVC ofrece una estructura organizada y modular para la construcción de aplicaciones, fomentando la separación de responsabilidades y simplificando tanto el mantenimiento como la evolución del software. Al descomponer la aplicación en tres componentes discretos, este patrón optimiza la claridad del código, promueve la reutilización de componentes y potencia la escalabilidad del sistema. Su adopción es ampliamente recomendada en el ámbito del desarrollo de aplicaciones web y de escritorio, contribuyendo así a la creación de una arquitectura resistente y fácil de gestionar.
Otro aspecto importante del MVC es su capacidad para adaptarse a diferentes tecnologías y plataformas. Aunque el patrón se originó en el contexto del desarrollo web, su filosofía de separación de preocupaciones y su enfoque en el modularidad lo hacen igualmente aplicable al desarrollo de aplicaciones de escritorio, móviles o incluso embebidas. Esto lo convierte en una opción versátil y duradera para una amplia gama de proyectos de software.











Referencias  

Qué es MVC. (s. f.). DesarrolloWeb.com.https://desarrolloweb.com/articulos/quees-
García, M. (2017, 5 octubre). MVC (Modelo-Vista-Controlador): ¿qué es y para qué sirve? https://codingornot.com/mvc-modelo-vista-controlador-que-es-y-para-que-sirve
Guía MVC (Model, View, Controller). (2023, 19 noviembre). DevCode Tutoriales. https://devcode.la/blog/guia-mvc-model-view-controller/
Rick-Anderson. (2023, 13 julio). ASP.NET introducción MVC. Microsoft Learn. https://learn.microsoft.com/es-es/aspnet/mvc/overview/getting-started/
Hernandez, R. D. (2021, 28 junio). El patrón modelo-vista-controlador:  Arquitectura y frameworks explicados. freeCodeCamp.org. https://www.freecodecamp.org/espanol/news/el-modelo-de-arquitectura-view-controller-pattern/
colaboradores de Wikipedia. (2023, 14 noviembre). Modelo–Vista–Controlador. Wikipedia, la Enciclopedia Libre. https://es.wikipedia.org/wiki/Modelo%E2%80%93vista%E2%80%93controlador

