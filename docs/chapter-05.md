# Capítulo V: Product Implementation, Validation & Deployment

En esta sección se mencionan las decisiones y convenciones las cuales permitirán mantener una consistencia durante el desarrollo del proyecto.

---

## 5.1. Software Configuration Management

---

### 5.1.1. Software Development Environment Configuration

**Project Management:**

La gestión de los proyectos tiene como objetivo mejorar los procesos y su entorno para alcanzar los resultados esperados.

* **Trello:** Es una herramienta visual que permite gestionar cualquier tipo de proyecto y el flujo de trabajo que el equipo desarrollador seguirá para implementar correctamente las tareas de código para el Landing Page y el Web Application.

| **URL:** | https://trello.com/es |
| :--- | :--- |

* **Pivotal Tracker:** Esta herramienta se define como una plataforma en la que se realiza la gestión de user stories, agrupándolos en epics y clasificando su presencia en el programa, por puntaje. Permite que cada miembro del equipo comparta la misma vista en tiempo real de lo que está sucediendo.

| **URL:** | https://www.pivotaltracker.com/ |
| :--- | :--- |

**Product UX/UI Design:**

Nos permite desarrollar el modelo en nuestro producto de manera digital y forme parte de la vida del consumidor. En este caso realizar un modelo de sitio web para computadoras y celulares.

* **Uxpressia:** Es una herramienta en línea para el mapeo de la trayectoria del cliente que crea mapas de impacto y personas. Sus herramientas nos permitieron establecer las bases del modelado de User Persona, Empathy Map y Journey Map.

| **URL:** | https://uxpressia.com/ |
| :--- | :--- |

* **MIRO:** Es una pizarra digital colaborativa en línea, que puede ser usada para la investigación, la ideación, la creación de lluvias de ideas, mapas mentales y una variedad de otras actividades colaborativas.

| **URL:** | https://www.miro.com/ |
| :--- | :--- |

* **Figma:** Es una herramienta de prototipo web y editor de gráficos vectorial alojada en la web, que permite establecer los modelos para las versiones de Web Browser y Landing Page.

| **URL:** | https://www.figma.com/ |
| :--- | :--- |

* **LucidChart:** Es una herramienta de diagramación basada en la web, que permite colaborar en tiempo real creando diseños UML, mapas mentales, prototipos de software, entre otros.

| **URL:** | https://www.lucidchart.com |
| :--- | :--- |

* **Structurizr:** Es una herramienta de diseño que soporta el modelo C4 para visualizar la arquitectura de software de nuestra solución.

| **URL:** | https://structurizr.com/ |
| :--- | :--- |

**Software Development:**

Representa el marco metodológico y técnico empleado para la construcción del producto. Esta estructura define los procesos y actividades específicas que guían el ciclo de vida del desarrollo, asegurando un enfoque organizado para cada etapa de la implementación.

* **GitHub:** Plataforma de alojamiento y gestión de repositorios que facilita el control de versiones y la colaboración técnica entre los integrantes del equipo Animatik.

| **URL:** | https://github.com/ |
| :--- | :--- |

* **WebStorm:** Entorno de desarrollo integrado (IDE) de JetBrains optimizado para el ecosistema web moderno, que agiliza la codificación, el refactorizado y las pruebas de la plataforma.

| **URL:** | https://www.jetbrains.com/webstorm/ |
| :--- | :--- |

* **HTML:** Lenguaje de marcado estándar utilizado para estructurar semánticamente el contenido y los componentes de la interfaz de usuario de Vetalis.

| **URL:** | https://www.jetbrains.com/help/webstorm/editing-html-files.html |
| :--- | :--- |

* **CSS:** Lenguaje de hojas de estilo encargado de la presentación visual, permitiendo implementar la identidad de marca y asegurar una experiencia estética coherente.

| **URL:** | https://www.jetbrains.com/help/webstorm/style-sheets.html#ws_css_completion |
| :--- | :--- |

* **TypeScript:** Lenguaje de programación de código abierto que añade tipado estático opcional a JavaScript, permitiendo un desarrollo más robusto, mantenible y escalable para la lógica de la solución veterinaria.

| **URL:** | https://www.typescriptlang.org/ |
| :--- | :--- |

* **Angular:** Framework de desarrollo para aplicaciones web diseñado por Google, utilizado para construir aplicaciones de una sola página (SPA) altamente eficientes mediante una arquitectura basada en componentes.

| **URL:** | https://angular.io/ |
| :--- | :--- |

* **GitHub Pages:** Servicio de despliegue que permite el alojamiento público de la Landing Page y las versiones preliminares de las aplicaciones web del proyecto.

| **URL:** | https://pages.github.com/ |
| :--- | :--- |

**Software Testing:**

Es el acto de examinar los artefactos y el comportamiento del software bajo prueba mediante validación y verificación.

* **Lenguaje Gherkin:** Es un DSL o Lenguaje Específico de Dominio, es decir, un lenguaje que está creado para resolver un problema. Se pueden agregar los user stories del programa con sus respectivas partes: Feature, Scenario, Example, Scenario Outline, Given, When, Then y And.

| **URL:** | https://cucumber.io/docs/gherkin/ |
| :--- | :--- |

### 5.1.2. Source Code Management

En esta sección se presenta la gestión de código fuente o como es conocido por sus siglas en inglés SCM (Source Code Management). Su función principal es realizar un seguimiento de las modificaciones que el equipo realizará a lo largo del desarrollo de sus proyectos en los repositorios de código fuente. Se emplea como un sistema de control de versiones que permite dar seguimiento a los cambios que cada integrante o desarrollador realice en el proyecto. Asimismo, cabe resaltar que para el sistema de control de versiones emplearemos GitHub.

**GitFlow**

Es el modelo alternativo de creación de ramas en Git que en los últimos años se ha vuelto una herramienta indispensable para muchos desarrolladores. Este flujo de trabajo de control de versiones utiliza ramas y fue publicado y popularizado por Vincent Driessen. Su principal función es ayudar en la organización de la versión de un código, permitiendo la creación de nuevos Features y Hotfixes de manera organizada.

**Main Branches:**

* **main:** es la rama principal, a partir de ella se recorrerán todas las ramas y contendrá la última versión y las anteriores creadas por los desarrolladores.
* **Develop:** Esta rama puede ser creada a partir de la rama main (master) y contará con todos los Features estables. Esto significa que a través de esta rama el equipo podrá integrar las funciones.

**Support Branches:**

* **Feature:** se ramifica de develop y al finalizar debe fusionarse de nuevo en develop. Se emplea para desarrollar nuevas funciones que se integrarán en versiones posteriores.
* **Release:** también se ramifica de develop, es la rama que admite la preparación de una nueva versión de producción.
* **Hotfix:** también está destinado a una nueva versión de producción, pero esta se ramifica de main. Su función es reparar rápidamente las publicaciones de producción.

**Conventional Commits:**

Son una convención para nombrar mensajes de commit en Git de forma estructurada, clara y semántica.

* **feat:** Se añade una nueva funcionalidad.
* **fix:** Se corrige un error.
* **docs:** Cambios en la documentación.
* **style:** Cambios de formato o estilo de código (sin impacto en la lógica).
* **refactor:** Mejoras en el código que no añaden nuevas funcionalidades ni corrigen errores.
* **test:** Añadir o modificar tests.
* **chore:** Cambios menores sin impacto en el código de producción (actualización de dependencias, configuración, etc.).

### 5.1.3. Source Code Style Guide & Conventions

El equipo ha definido un conjunto de reglas y estándares de programación con el objetivo de garantizar la legibilidad, mantenibilidad y coherencia del código en el proyecto Vetalis. Como regla transversal y obligatoria, toda la nomenclatura de los elementos del sistema se realizará en el idioma inglés.

#### General Naming Conventions

Se adoptan las convenciones de capitalización estándar para diferenciar la naturaleza de los componentes:

* **PascalCase:** Utilizado para nombres de clases e interfaces en Java.
* **camelCase:** Utilizado para variables locales, parámetros, nombres de métodos en Java y variables en TypeScript (Angular).
* **kebab-case:** Utilizado para nombres de archivos, selectores CSS (IDs y clases) y selectores de componentes de Angular.

#### HTML & CSS Style Guide

Basado en la Google HTML/CSS Style Guide y las directrices de la W3C:

* **HTML:** Uso obligatorio de etiquetas semánticas para mejorar el SEO y la accesibilidad. Se requiere una indentación de 2 espacios y el uso de comillas dobles para los atributos.
* **CSS:** Se prioriza el uso de selectores de clase. Las propiedades deben agruparse de manera lógica (posicionamiento, luego modelo de caja, luego tipografía). Se prohíbe el uso de estilos en línea (inline styles).

#### TypeScript & Angular Style Guide

Siguiendo la Google TypeScript Style Guide y la Angular Style Guide:

* **Sintaxis:** Uso de TypeScript (Arrow functions, destructuring y template literals). Se prefiere `const` para todas las declaraciones, usando `let` solo cuando sea estrictamente necesario.
* **Angular:** Los nombres de los componentes deben seguir la convención de incluir el tipo en el nombre del archivo (ej. `hero-detail.component.ts`) y los selectores deben usar el prefijo definido para el proyecto seguido de kebab-case.

#### Java & Spring Boot Coding Conventions

Siguiendo las Oracle Java Code Conventions y las guías de Spring Boot:

* **Estructura:** Las interfaces deben ser nombres descriptivos (aunque en Java no es obligatorio el prefijo "I", se mantiene por convención de equipo si se desea). Los campos privados deben utilizar camelCase estándar.
* **Inyección de Dependencias:** Se prefiere la inyección por constructor sobre la anotación `@Autowired` en campos, para facilitar las pruebas unitarias y garantizar la inmutabilidad.

#### Gherkin Conventions for Readable Specifications

Para la redacción de criterios de aceptación y pruebas de comportamiento:

* **Formato:** Uso riguroso de la estructura `Given / When / Then`.
* **Lenguaje:** Las especificaciones deben redactarse desde la perspectiva del negocio (usuario de la veterinaria), evitando tecnicismos de implementación en los pasos de Gherkin.

#### Referencias de Estándares Adoptados

| Tecnología | Referencia Principal |
| :--- | :--- |
| HTML / CSS | Google HTML/CSS Style Guide / W3C |
| TypeScript | Google TS Style Guide |
| Java | Oracle Java Code Conventions |
| Spring Boot | Spring Boot Coding Guidelines |
| Angular | Angular Style Guide |
| Gherkin | Gherkin Conventions for Readable Specifications |


### 5.1.4. Software Deployment Configuration

Como se mencionó previamente, la gestión de nuestro código fuente se realizará a través de GitHub. Asimismo, se utilizará GitHub Pages para la publicación y despliegue de la página.

Para el desarrollo del Landing Page de NeuroZen se han usado las siguientes herramientas:

* **HTML:** lenguaje con el cual está estructurado nuestro landing page.
* **CSS:** diseño y formato para el html desarrollado.

El despliegue de nuestro landing page es posible gracias a la herramienta de Github Pages. El cual es un servicio que nos permite alojar nuestro landing directamente desde el repositorio de GitHub.

Para lograr el despliegue seguimos los siguientes pasos:

1. Dirigirnos al repositorio de la página y entrar en la sección de configuración.
2. Ir a la opción de “Pages”, donde se encontrarán todas las opciones de publicación de página.
3. Se debe seleccionar la rama la cual se va a publicar en el vínculo. También se debe seleccionar la carpeta donde se localizara la publicación.
4. Finalmente, el link vínculo de nuestra página aparecerá en la parte superior.

## 5.2. Landing Page, Services & Applications Implementation

La construcción de la página de inicio, junto con los servicios y aplicaciones, es un paso fundamental en nuestro ciclo de desarrollo. Esto nos permite hacer realidad el diseño y las funciones proyectadas, convirtiendo las ideas iniciales en productos tangibles y listos para su uso. En esta fase traducimos los requerimientos y especificaciones a código fuente, estructurando la plataforma web según las necesidades detectadas.
***
### 5.2.1. Sprint 1

La primera iteración constituye un paso fundamental en nuestra metodología de desarrollo ágil. Durante este periodo, enfocaremos nuestra capacidad operativa en la construcción de las funcionalidades críticas y herramientas de alta prioridad establecidas en la fase de planificación. Este proceso consiste en traducir los requisitos técnicos y de negocio en componentes de software operativos, estableciendo los cimientos funcionales de nuestro producto bajo un modelo de mejora continua y entregas incrementales.

#### 5.2.1.1. Sprint Planning 1

| Sprint # | Sprint 1                                                                                                                                                                                                                                                                               |
| :--- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Sprint Planning Background** | Sesión de planificación inicial para establecer las bases del proyecto VetCare, priorizando la presencia web y la documentación técnica del primer hito académico.                                                                                                                     |
| **Date** | 2026-04-17                                                                                                                                                                                                                                                                             |
| **Time** | 07:00 PM                                                                                                                                                                                                                                                                               |
| **Location** | Google Meet (Reunión virtual)                                                                                                                                                                                                                                                          |
| **Prepared By** | Sejuro Medina, Mario Gabriel                                                                                                                                                                                                                                                           |
| **Attendees (to planning meeting)** | Gamero Miranda Lui Mathias/ Roman Zevallos, Sebastian Jared / Romero Vilela, Dario Alberto / Sanchez Benavente, Leonardo Matias / Sejuro Medina, Mario Gabriel                                                                                                                         |
| **Sprint 1 – 1 Review Summary** | Se lograron los hitos de desarrollo para los capítulos iniciales y el despliegue funcional de la Landing Page. No obstante, se identificó como punto de mejora la finalización de los entregables administrativos en formatos PDF y Word para cumplir con la totalidad del hito.       |
| **Sprint 1 – 1 Retrospective Summary** | El desempeño durante el primer ciclo fue aceptable, logrando un producto funcional aunque con oportunidades de optimización en la coordinación interna para futuros entregables de mayor complejidad técnica.                                                                          |
| **Sprint Goal & User Stories** |                                                                                                                                                                                                                                                                                        |
| **Sprint 1 Goal** | Lograr la culminación del reporte técnico y el despliegue exitoso de la Landing Page en el repositorio del equipo. La validación del éxito se mide mediante el flujo de tareas en el Board de Trello, asegurando que todos los ítems de prioridad alta alcancen el estado "Terminado". |
| **Sprint 1 Velocity** | 20                                                                                                                                                                                                                                                                                     |
| **Sum of Story Points** | 20                                                                                                                                                                                                                                                                                     |

La sesión de Sprint Planning es clave dentro de la metodología ágil, ya que en ella el equipo organiza con detalle las actividades de la siguiente iteración. Aquí se determinan las tareas a realizar, los tiempos estimados y los responsables. Su objetivo principal es trazar una hoja de ruta definida y realista, promoviendo el trabajo en equipo y garantizando que todos compartan la misma visión sobre las metas trazadas.

#### 5.2.1.2. Aspect Leaders and Collaborators

Durante la ejecución de la primera iteración, el equipo focalizó sus capacidades en el desarrollo integral de la presencia digital de *Vetalis, abordando los requerimientos priorizados dentro del **Epic 1: Landing Page (Static Web Site)*. La finalidad de este ciclo fue consolidar el canal de comunicación externa y habilitar los mecanismos de conversión para prospectos interesados en la plataforma.

*Historias de Usuario Abordadas*

| ID | Título | Descripción | Story Points | Asignado a | Estado |
| :--- | :--- | :--- |:------------------:| :--- | :---: |
| *US001* | View Value Proposition | Visualización de la propuesta de valor centrada en el ecosistema IoT y gestión integral en la home page. | 3 | Gamero Miranda, Lui Mathias | Done |
| *US002* | Select Veterinarian Segment | Implementación de la sección especializada para el perfil médico, detallando funciones de EHR y control nutricional. | 3 | Roman Zevallos, Sebastian Jared | Done |
| *US003* | Request Software Demo | Desarrollo del formulario de contacto para la captación de leads y registro de interés en dispositivos IoT. | 5 | Romero Vilela, Dario Alberto | Done |
| *US004* | View Pricing Plans | Maquetación de la tabla comparativa de planes de suscripción (Basic, Pro, Enterprise) y sus costos. | 3 | Sanchez Benavente, Leonardo Matias | Done |
| *US006* | Read Client Testimonials | Despliegue de la sección de prueba social con reseñas verificadas de administradores y médicos veterinarios. | 3 | Sejuro Medina, Mario Gabriel | Done |
| *US008* | View Mobile Menu | Implementación del sistema de navegación responsiva (menú hamburguesa) para optimizar la experiencia en smartphones. | 5 | Sanchez Benavente, Leonardo Matias | Done |

Evidencia del avance en Trello:

<img src="../assets/Sprint_01_Trello.png" alt="Foto Sprint 01 en Trello"/>

*URL:* https://trello.com/invite/b/69ea5e4e6743746b9259cdec/ATTI07c5209f0d55628672b1d547ef9c38243661ADA5/vetalis-user-stories

Este primer ciclo de trabajo concluyó con la entrega funcional de la Landing Page de Vetalis, ofreciendo a los usuarios un acercamiento inicial a la propuesta de valor integral. El sitio permite explorar las herramientas de gestión administrativa, las funcionalidades diseñadas para el sector clínico veterinario y la automatización IoT, integrando además testimonios de la industria y datos generales sobre el ecosistema de la aplicación.

#### 5.2.1.3. Sprint Backlog 1

| Sprint # | Sprint 1 |
| :--- | :--- |

| User Story / Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- |:------------------:| :--- | :---: |
| *WK01* | Configuración del entorno de desarrollo | Establecimiento de la organización en GitHub, definición de la estrategia de ramas (GitFlow) y configuración del tablero en Trello. | 2 | Todos los miembros del equipo | Done |
| *WK02* | Finalización del Capítulo 01 | Elaboración de la descripción de la startup Animatik, perfiles de los integrantes y definición estratégica de la solución. | 4 | Todos los miembros del equipo | Done |
| *WK03* | Finalización del Capítulo 02 | Documentación de User Personas, Empathy Maps, análisis competitivo y diseño de entrevistas para el needfinding. | 6 | Todos los miembros del equipo | Done |
| *WK04* | Finalización del Capítulo 03 | Redacción de User Stories detalladas, elaboración del Impact Mapping y organización del Product Backlog prioritario. | 6 | Todos los miembros del equipo | Done |
| *WK05* | Finalización del Capítulo 04 | *Fase de Diseño Detallado:* Definición de lineamientos de estilo, arquitectura de información y creación de Wireframes y Mockups de alta fidelidad. | 9 | Todos los miembros del equipo | Done |
| *WK06* | Finalización del Capítulo 05 | *Configuración de Implementación:* Documentación de la gestión de configuración de software, convenciones de código y evidencia de despliegue. | 8 | Todos los miembros del equipo | Done |
| *US001* | View Value Proposition | Implementación en la home page de la propuesta de valor enfocada en la automatización de alimentación IoT y gestión clínica. | 3 | Lui Mathias Gamero Miranda | Done |
| *US002* | Select Veterinarian Segment | Desarrollo de la sección detallada para el perfil médico sobre EHR, prescripciones y control nutricional remoto. | 3 | Roman Zevallos, Sebastian Jared | Done |
| *US003* | Request Software Demo | Creación del formulario de contacto para la captación de leads y registro del interés en la integración IoT en la base de datos. | 5 | Romero Vilela, Dario Alberto | Done |
| *US004* | View Pricing Plans | Maquetación de la tabla comparativa de los niveles de suscripción (Basic, Pro y Enterprise) y sus beneficios financieros. | 3 | Sanchez Benavente, Leonardo Matias | Done |
| *US006* | Read Client Testimonials | Implementación del carrusel de testimonios verificados de administradores y veterinarios para fortalecer la confianza en el producto. | 3 | Sejuro Medina, Mario Gabriel | Done |
| *US008* | View Mobile Menu | Desarrollo y adaptación del menú hamburguesa responsivo para garantizar la navegación fluida en dispositivos móviles. | 5 | Sanchez Benavente, Leonardo Matias | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

En este apartado se detallan los progresos realizados en la fase de implementación de los componentes de la solución vinculados al alcance del presente Sprint: Landing Page y la base documental del proyecto.

Inicialmente, se exponen los commits más significativos realizados en el repositorio del Informe, los cuales evidencian la evolución de la estructura estratégica y técnica de *Vetalis*:

| Repository | Branch | Commit Message | Commit ID |
| :--- | :---: | :--- | :---: |
| /Report | main | docs: chapter 1 structure and startup profile finalized | 50c76ce |
| /Report | develop | feat: chapter 3 user stories and impact mapping | 32f741a |
| /Report | develop | docs: update style guidelines and information architecture | 6940803 |

*Registro de Commits de Documentación y Diseño*

A continuación, se presenta el registro detallado de las contribuciones destinadas a la estructuración de los primeros capítulos y el diseño de la experiencia de usuario:

| Autor | Fecha | Commit Message | Commit ID |
| :--- | :---: | :--- | :---: |
| Sanchez Benavente, Leonardo Matias | 16/04/2026 | docs: añade segmentos objetivo en chapter-01 | f052994 |
| Roman Zevallos, Sebastian Jared | 16/04/2026 | docs(chapter-03): refine user story descriptions | 948f654 |
| Lui Mathias Gamero Miranda | 17/04/2026 | Update chapter-04.md assets and color palette | 33c063c |
| Sejuro Medina, Mario Gabriel | 17/04/2026 | docs(chapter-02): update customer journey maps | f0197b2 |
| Romero Vilela, Dario Alberto | 17/04/2026 | docs: add empathy maps for veterinarian segment | 96423a6 |
| Sejuro Medina, Mario Gabriel | 20/04/2026 | docs(chapter-05): finalize sprint backlog 1 | 9367375 |
| Roman Zevallos, Sebastian Jared | 20/04/2026 | docs: software development environment setup | 6479f15 |
| Romero Vilela, Dario Alberto | 20/04/2026 | docs(chapter-02): add event storming diagrams | cdf0e31 |
| Lui Mathias Gamero Miranda | 19/04/2026 | docs: update high-fidelity mockups for landing page | de62be9 |

#### 5.2.1.5. Execution Evidence for Sprint Review

En esta entrega, el equipo de desarrolladores de Vetalis ha completado con éxito la implementación y el lanzamiento de la página de la Landing Page. Esta página presenta diferentes secciones que brindan información detallada sobre nuestro producto.

<img src="../assets/vetalis_landing_1.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_2.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_3.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_4.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_5.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_6.jpeg" alt="Vetalis landing"/>
<img src="../assets/vetalis_landing_7.jpeg" alt="Vetalis landing"/>

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1, se llevó a cabo la publicación de la Landing Page de Vetalis empleando GitHub Pages como servicio de hosting. A continuación, se detallan las acciones realizadas para lograr su despliegue exitoso.

Se creó el repositorio denominado Vetalis-Landing-Page dentro de la organización 1ASI0729-2610-10177-Animatik-Vetalis en GitHub.

El desarrollo de la Landing Page se realizó en la rama develop, siguiendo el modelo de trabajo GitFlow, donde se implementaron secciones como hero, problemática, beneficios, startup, planes y footer.

Tras validar el contenido, se efectuó la fusión de la rama develop hacia main mediante un Pull Request, lo que permitió activar automáticamente el despliegue del sitio a través de GitHub Pages.

Se verificó el despliegue exitoso accediendo a la URL pública: https://1asi0729-2610-10177-animatik-vetalis.github.io/Vetalis-Landing/

---
#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Se desplegó la landing page usando el servicio de GitHub Pages. Se configuró para utilizar la rama main como base del proyecto a desplegar.

<img src="../assets/Landing-deploy.jpeg" alt="Vetalis landing deploy"/>

URL de Landing Page Desplegada: https://1asi0729-2610-10177-animatik-vetalis.github.io/Vetalis-Landing/


---
#### 5.2.1.8. Team Collaboration Insights during Sprint
A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 1:
<img src="../assets/team_Insights.png" alt="Vetalis landing"/>

### 5.2.2. Sprint 2

La segunda iteración representa un avance consecuente en nuestra metodología de desarrollo ágil. Durante este periodo, enfocaremos nuestra capacidad operativa en la construcción y despliegue de la aplicación web frontend, priorizando las interfaces interactivas de gestión clínica establecidas en la fase de planificación. Este proceso consiste en traducir los requisitos de experiencia de usuario y lógica de negocio en componentes visuales operativos, expandiendo los cimientos funcionales de nuestro producto hacia una solución de software interactiva bajo un modelo de mejora continua y entregas incrementales.

### 5.2.2.1. Sprint Planning 2

| Sprint # | Sprint 2                                                                                                                                                                                                                                         |
| :--- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Sprint Planning Background** |                                                                                                                                                                                                                                                  |
| Date | 2026-05-11                                                                                                                                                                                                                                       |
| Time | 05:00 PM                                                                                                                                                                                                                                         |
| Location | Google Meet (Reunión virtual)                                                                                                                                                                                                                         |
| Prepared By | Gamero Miranda, Lui Mathias                                                                                                                                                                                                                      |
| Attendees (to planning meeting) | Gamero Miranda, Lui Mathias / Roman Zevallos, Sebastian Jared / Romero Vilela, Dario Alberto / Sanchez Benavente, Leonardo Matias / Sejuro Medina, Mario Gabriel                                                                                 |
| **Sprint 1 Review Summary** | Se logró implementar y desplegar exitosamente la primera versión del Landing Page estático con HTML5, CSS3 y JavaScript. Se validó correctamente la presentación de la propuesta de valor y los planes de precios ante el Product Owner.         |
| **Sprint 1 Retrospective Summary** | El equipo identificó que la comunicación durante el control de versiones fue fluida gracias a GitFlow, pero se acordó mejorar la estimación de tiempos en el diseño responsivo para evitar sobrecargas de tareas en los últimos días del sprint. |
| **Sprint Goal & User Stories** |                                                                                                                                                                                                                                                  |
| Sprint 2 Goal | Nuestro enfoque es desplegar el frontend de gestión clínica. Creemos que facilitará a los veterinarios el manejo de triajes e historiales. Se confirmará cuando los usuarios naveguen por la aplicación Angular y sus módulos básicos.           |
| Sprint 2 Velocity | 34                                                                                                                                                                                                                                               |
| Sum of Story Points | 34                                                                                                                                                                                                                                               |

La sesión de Sprint Planning es clave dentro de nuestra metodología ágil, ya que nos permitió organizar con detalle las actividades de esta segunda iteración. Durante la reunión, determinamos las tareas específicas para la configuración y desarrollo del frontend, asignamos los tiempos estimados y definimos a los responsables de cada módulo clínico. El objetivo principal fue trazar una hoja de ruta definida y realista para la implementación de las interfaces de usuario, promoviendo el trabajo en equipo y garantizando que todos compartamos la misma visión sobre las metas trazadas para el despliegue de la aplicación web.

### 5.2.2.2. Aspect Leaders and Collaborators

Durante la ejecución de la segunda iteración, el equipo focalizó sus capacidades en el desarrollo y estructuración de la aplicación web frontend, abordando los requerimientos priorizados dentro del Epic 2: Clinical Management - EHR (Veterinarian). La finalidad de este ciclo fue consolidar las interfaces operativas de la plataforma y habilitar los módulos interactivos de triaje, prescripción e historial médico para optimizar el flujo de trabajo diario de los profesionales veterinarios.

| Team Member (Last Name, First Name) | GitHub Username   | Configuración y Despliegue Frontend Leader (L) / Collaborator (C) | Módulo de Búsqueda y Alertas Leader (L) / Collaborator (C) | Módulo de Historial y Recetas Leader (L) / Collaborator (C) | Módulo de Triaje Leader (L) / Collaborator (C) |
| :--- |:------------------| :---: | :---: | :---: | :---: |
| Gamero Miranda, Lui Mathias | lug07m            | L | C | C | C |
| Roman Zevallos, Sebastian Jared | Chebas19          | C | C | L | C |
| Romero Vilela, Dario Alberto | patatitis9-alt    | C | C | L | C |
| Sanchez Benavente, Leonardo Matias | Matiassb06        | C | C | C | L |
| Sejuro Medina, Mario Gabriel | maghetthi         | C | L | C | C |

### 5.2.2.3.Sprint Backlog 2.
| Sprint # | Sprint 2 |
| :--- | :--- |

| User Story / Task Id | Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- |:------------------:| :--- | :---: |
| *WK07* | Configuración y Despliegue del Frontend | Configuración del entorno de desarrollo en Angular y despliegue de la primera versión de la Web Application en la nube, generando la URL pública. | 5 | Todos los miembros del equipo | To Do |
| *US011* | Search Patient Profile | Desarrollo de la barra de búsqueda y vista de resultados para localizar rápidamente los perfiles y el historial médico de los pacientes. | 6 | Sejuro Medina, Mario Gabriel | To Do |
| *US012* | Record Vital Signs | Maquetación e implementación del formulario para el registro de los signos vitales (peso y temperatura) durante el proceso de triaje. | 5 | Sanchez Benavente, Leonardo Matias | To Do |
| *US013* | View Allergy Alerts | Implementación visual de alertas de alta prioridad (banners) en la vista del historial clínico para notificar alergias del paciente. | 4 | Gamero Miranda, Lui Mathias | To Do |
| *US014* | Create Digital Prescription | Desarrollo del módulo de recetas médicas para la generación de prescripciones digitales y planes nutricionales estandarizados. | 8 | Romero Vilela, Dario Alberto | To Do |
| *US019* | View Medical History Timeline | Maquetación de la línea de tiempo cronológica para visualizar de forma ordenada el historial de consultas pasadas del paciente. | 6 | Roman Zevallos, Sebastian Jared | To Do |

Evidencia del avance en Trello:

<img src="../assets/Sprint_02_Trello.png" alt="Foto Sprint 02 en Trello"/>

*URL:* https://trello.com/invite/b/69ea5e4e6743746b9259cdec/ATTI07c5209f0d55628672b1d547ef9c38243661ADA5/vetalis-user-stories

Este segundo ciclo de trabajo concluyó con la entrega funcional de la aplicación web frontend de Animatik, permitiendo a los médicos veterinarios interactuar directamente con los módulos de gestión clínica. La plataforma ahora facilita la búsqueda ágil de pacientes, el registro de signos vitales durante el triaje y la gestión de historiales médicos digitales, integrando una interfaz responsiva desplegada en la nube que optimiza la operatividad y la atención diaria en la clínica.

### 5.2.2.4.Development Evidence for Sprint Review.

En este apartado se detallan los commits más significativos realizados en el repositorio durante el Sprint 2:

| Repository | Branch | Commit id | Commit message | Commited on (Date) |
| :--- | :---: | :---: | :--- | :---: |
| Vetalis-Frontend | main | bef77e0 | feat(main): add schedule.html, schedule.css, and schedule.ts | 12/05/2026 |
| Vetalis-Frontend | main | da539b3 | feat(main): add dashboard.html and profile.css | 12/05/2026 |
| Vetalis-Frontend | main | 3c2d25e | feat(main): add profile html and ts files | 12/05/2026 |
| Vetalis-Frontend | main | 7e66bba | feat(main): add comunication | 12/05/2026 |
| Vetalis-Frontend | main | cd62339 | Vetalis-Frontend | 12/05/2026 |

### 5.2.2.5.Execution Evidence for Sprint Review.

Durante este segundo Sprint, el equipo avanzó en la implementación de la aplicación web frontend, logrando una interfaz interactiva, visualmente coherente y adaptable a diferentes dispositivos para los módulos de gestión clínica. A continuación se muestra la evidencia visual de las secciones desplegadas, mostrando la navegación de la plataforma.

1. Dashboard - Panel Principal:

<img src="../assets/Frontend-01.png" alt="Vetalis Frontend - Vista 1"/>

2. Perfil de Usuario (Profile):

<img src="../assets/Frontend-02.png" alt="Vetalis Frontend - Vista 2"/>

3. Calendario/Agenda (Schedule):

<img src="../assets/Frontend-03.png" alt="Vetalis Frontend - Vista 3"/>

4. Comunicación (Comunication):

<img src="../assets/Frontend-04.png" alt="Vetalis Frontend - Vista 4"/>

5. Otras vistas de gestión:

<img src="../assets/Frontend-05.png" alt="Vetalis Frontend - Vista 5"/>

### 5.2.2.6.Services Documentation Evidence for Sprint Review.

A continuación, se presentan los commits que evidencian la construcción e integración de servicios y componentes para el Frontend:

<table>
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit ID</th>
      <th>Commit message</th>
      <th>Commit Message body</th>
      <th>Commit on (date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="5" align="center" valign="middle">Vetalis-<br>Frontend</td>
      <td align="center">main</td>
      <td align="center">cd62339</td>
      <td>Vetalis-Frontend</td>
      <td>Configuración base inicial del repositorio del frontend.</td>
      <td align="center">12/05/2026</td>
    </tr>
    <tr>
      <td align="center">main</td>
      <td align="center">7e66bba</td>
      <td>feat(main): add comunication</td>
      <td>Desarrollo e integración del módulo de comunicación.</td>
      <td align="center">12/05/2026</td>
    </tr>
    <tr>
      <td align="center">main</td>
      <td align="center">3c2d25e</td>
      <td>feat(main): add profile html and ts files</td>
      <td>Agregada la estructura HTML y la lógica en TypeScript para el perfil.</td>
      <td align="center">12/05/2026</td>
    </tr>
    <tr>
      <td align="center">main</td>
      <td align="center">da539b3</td>
      <td>feat(main): add dashboard.html and profile.css</td>
      <td>Creación de la vista del dashboard y estilos asociados al perfil.</td>
      <td align="center">12/05/2026</td>
    </tr>
    <tr>
      <td align="center">main</td>
      <td align="center">bef77e0</td>
      <td>feat(main): add schedule.html, schedule.css, and schedule.ts</td>
      <td>Implementación de las vistas y estilos para el módulo de agenda (schedule).</td>
      <td align="center">12/05/2026</td>
    </tr>
  </tbody>
</table>

### 5.2.2.7.Software Deployment Evidence for Sprint Review.

El despliegue de la aplicación web frontend se realizó utilizando GitHub Pages, aprovechando la integración directa con el repositorio del proyecto. Esta configuración permite que el sitio sea accesible públicamente y se actualice automáticamente con cada cambio en la rama principal.

<img src="../assets/Deployment.png" alt="Vetalis Frontend Deployment"/>

**URL:** https://1asi0729-2610-10177-animatik-vetalis.github.io/Vetalis-Frontend/

### 5.2.2.8.Team Collaboration Insights during Sprint.

Durante el Sprint 2, nuestra colaboración se centró principalmente en la estructuración y desarrollo de la aplicación web frontend, así como en la actualización de la base documental. El equipo utilizó Trello y GitFlow para la gestión de tareas y control de versiones, asegurando que cada módulo (Dashboard, Perfil, Agenda) fuera implementado correctamente y a tiempo.

**Gráfico de Contribuciones del equipo**

**Contribuciones al desarrollo del Frontend:**

<img src="../assets/Team Collaboration- Frontend.png" alt="Team Collaboration Frontend"/>

**Contribuciones al desarrollo del Documento:**

<img src="../assets/Team Collaboration.png" alt="Team Collaboration Documento"/>

## 5.3. Validation Interviews
***
### 5.3.1. Diseño de Entrevistas
### 5.3.2. Registro de Entrevistas
### 5.3.3. Evaluaciones según heurísticas
## 5.4. Video About-the-Product

---
## Conclusiones

---

### Conclusiones y recomendaciones

**Conclusiones:**
1. **Adopción exitosa de Metodologías Ágiles:** El uso de Sprints y herramientas como Trello y Pivotal Tracker ha permitido al equipo de Animatik mantener un flujo de trabajo organizado y estructurado. Esto se evidenció en la entrega oportuna de la Landing Page en el Sprint 1 y del Frontend de la aplicación web en el Sprint 2, cumpliendo con los objetivos y la velocidad estimada.
2. **Eficiencia en la Gestión de Configuración y Control de Versiones:** La estricta implementación de GitFlow en GitHub, apoyada con Convenciones de Commits (Conventional Commits), facilitó la colaboración fluida entre los desarrolladores, mitigando conflictos de integración y asegurando la estabilidad de las ramas `main` y `develop`.
3. **Calidad y Estandarización de Código:** La definición y seguimiento de guías de estilo para HTML, CSS, TypeScript y Angular ha garantizado que el código base de Vetalis sea escalable, legible y fácilmente mantenible.
4. **Despliegue Continuo con Github Pages:** La automatización básica implementada a través de GitHub Pages ha demostrado ser una solución efectiva y ágil para el despliegue tanto de la Landing Page como del Frontend, permitiendo la validación continua del producto por parte de los stakeholders.
5. **Enfoque Centrado en el Usuario (Veterinarios):** La correcta maquetación de funcionalidades clave, como el Electronic Health Record (EHR), el registro de signos vitales (Triaje) y el módulo de recetas médicas, demuestra que la solución Vetalis está profundamente alineada con las necesidades operativas de la gestión clínica veterinaria y el control de dispositivos IoT.

**Recomendaciones:**
1. **Mejora en la Estimación de Tareas:** Se recomienda refinar la asignación de Story Points y la estimación de tiempos, especialmente para módulos con alta complejidad en diseño responsivo y lógica de componentes, evitando la sobrecarga técnica al final de cada Sprint.
2. **Integración Continua Avanzada:** A medida que el proyecto escale hacia el desarrollo del Backend (Spring Boot/Java) y los servicios IoT, será recomendable implementar pipelines o flujos de CI/CD (GitHub Actions) más robustos que incluyan pruebas automatizadas antes del despliegue.
3. **Validación Temprana con Usuarios Finales:** Se sugiere ejecutar rondas de Usability Testing con veterinarios y administradores utilizando el Frontend actual, para aplicar ajustes de experiencia de usuario (UX) antes de completar la integración con la base de datos y la API.

### Video About-the-Team

---

## Bibliografía

Beyer, K., Chomiak-Orsa, I., Pietrzykowski, Z., & Rozkrut, D. (2025). *Digital transformation and business process improvement in veterinary clinics*. (pp. 201-213). https://doi.org/10.18276/978-83-8419-028-9-15

Mallikarjun, A., Charendoff, I., Moore, M. B., Wilson, C., Nguyen, E., Hendrzak, A. J., Poulson, J., Gibison, M., & Otto, C. M. (2024). Assessing Different Chronic Wasting Disease Training Aids for Use with Detection Dogs. *Animals*, *14*(2), 300. https://doi.org/10.3390/ani14020300

Soltani, Z., & Siadati, S. (2019). *The impact of business intelligence on increasing the efficiency and health quality of surgical centers*. (Research on Health Management and Efficiency).

---

