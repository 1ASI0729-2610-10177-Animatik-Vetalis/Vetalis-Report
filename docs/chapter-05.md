# Capítulo V: Product Implementation, Validation & Deployment

En esta sección se mencionan las decisiones y convenciones las cuales permitirán mantener una consistencia durante el desarrollo del proyecto.

---

## 5.1. Software Configuration Management

---

### 5.1.1. Software Development Environment Configuration

**Project Management:**

La gestión de los proyectos tiene como objetivo mejorar los procesos y su entorno para alcanzar los resultados esperados.

* **Trello:** Es una herramienta visual que permite gestionar cualquier tipo de proyecto y el flujo de trabajo que el equipo desarrollador seguirá para implementar correctamente las tareas de código para el Landing Page y el Web Application.

| **Link de referencia:** | https://trello.com/es |
| :--- | :--- |

* **Pivotal Tracker:** Esta herramienta se define como una plataforma en la que se realiza la gestión de user stories, agrupándolos en epics y clasificando su presencia en el programa, por puntaje. Permite que cada miembro del equipo comparta la misma vista en tiempo real de lo que está sucediendo.

| **Link de referencia:** | https://www.pivotaltracker.com/ |
| :--- | :--- |

**Product UX/UI Design:**

Nos permite desarrollar el modelo en nuestro producto de manera digital y forme parte de la vida del consumidor. En este caso realizar un modelo de sitio web para computadoras y celulares.

* **Uxpressia:** Es una herramienta en línea para el mapeo de la trayectoria del cliente que crea mapas de impacto y personas. Sus herramientas nos permitieron establecer las bases del modelado de User Persona, Empathy Map y Journey Map.

| **Link de referencia:** | https://uxpressia.com/ |
| :--- | :--- |

* **MIRO:** Es una pizarra digital colaborativa en línea, que puede ser usada para la investigación, la ideación, la creación de lluvias de ideas, mapas mentales y una variedad de otras actividades colaborativas.

| **Link de referencia:** | https://www.miro.com/ |
| :--- | :--- |

* **Figma:** Es una herramienta de prototipo web y editor de gráficos vectorial alojada en la web, que permite establecer los modelos para las versiones de Web Browser y Landing Page.

| **Link de referencia:** | https://www.figma.com/ |
| :--- | :--- |

* **LucidChart:** Es una herramienta de diagramación basada en la web, que permite colaborar en tiempo real creando diseños UML, mapas mentales, prototipos de software, entre otros.

| **Link de referencia:** | https://www.lucidchart.com |
| :--- | :--- |

* **Structurizr:** Es una herramienta de diseño que soporta el modelo C4 para visualizar la arquitectura de software de nuestra solución.

| **Link de referencia:** | https://structurizr.com/ |
| :--- | :--- |

**Software Development:**

Es una estructura aplicada al desarrollo de un producto de software. Se utiliza para el establecimiento de un proceso para el desarrollo de software, cada uno de los cuales describe un enfoque diferente para diferentes actividades que tienen lugar durante el proceso.

* **GitHub:** Es un repositorio comunitario cuya función es almacenar los avances de un proyecto elaborado por un grupo de personas.

| **Link de referencia:** | https://github.com/ |
| :--- | :--- |

* **WebStorm:** Es un entorno de JetBrains. Este nos ofrece facilidad en probar nuestro entorno web en navegadores web.

| **Link de referencia:** | https://www.jetbrains.com/webstorm/ |
| :--- | :--- |

* **HTML:** Es un lenguaje que sirve como desarrollador de plataformas web que trabaja con hipertextos.

| **Link de referencia:** | https://www.jetbrains.com/help/webstorm/editing-html-files.html |
| :--- | :--- |

* **CSS:** Es un lenguaje de diseño para el entorno web. Permite elaborar la interfaz de usuario diseñada anteriormente.

| **Link de referencia:** | https://www.jetbrains.com/help/webstorm/style-sheets.html#ws_css_completion |
| :--- | :--- |

* **JavaScript:** Es un lenguaje de programación ligero, interpretado o compilado justo a tiempo (JIT) con funciones de primera clase, esencial para el desarrollo de aplicaciones web interactivas.

| **Link de referencia:** | https://developer.mozilla.org/es/docs/Web/JavaScript |
| :--- | :--- |

* **Vue.js:** Framework progresivo de JavaScript utilizado para construir interfaces de usuario y aplicaciones de una sola página (SPA).

| **Link de referencia:** | https://vuejs.org/ |
| :--- | :--- |

* **GitHub Pages:** Servicio de Github que nos permitió alojar nuestra landing page y nos permitirá alojar nuestras web applications.

| **Link de referencia:** | https://pages.github.com/ |
| :--- | :--- |

**Software Testing:**

Es el acto de examinar los artefactos y el comportamiento del software bajo prueba mediante validación y verificación.

* **Lenguaje Gherkin:** Es un DSL o Lenguaje Específico de Dominio, es decir, un lenguaje que está creado para resolver un problema. Se pueden agregar los user stories del programa con sus respectivas partes: Feature, Scenario, Example, Scenario Outline, Given, When, Then y And.

| **Link de referencia:** | https://cucumber.io/docs/gherkin/ |
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

*Enlace de Trello:* https://trello.com/invite/b/69ea5e4e6743746b9259cdec/ATTI07c5209f0d55628672b1d547ef9c38243661ADA5/vetalis-user-stories

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

#### 5.2.1.5. Execution Evidence for Sprint Review
#### 5.2.1.6. Services Documentation Evidence for Sprint Review
#### 5.2.1.7. Software Deployment Evidence for Sprint Review
#### 5.2.1.8. Team Collaboration Insights during Sprint


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

### Video About-the-Team

---

## Bibliografía

Beyer, K., Chomiak-Orsa, I., Pietrzykowski, Z., & Rozkrut, D. (2025). *Digital transformation and business process improvement in veterinary clinics*. (pp. 201-213). https://doi.org/10.18276/978-83-8419-028-9-15

Mallikarjun, A., Charendoff, I., Moore, M. B., Wilson, C., Nguyen, E., Hendrzak, A. J., Poulson, J., Gibison, M., & Otto, C. M. (2024). Assessing Different Chronic Wasting Disease Training Aids for Use with Detection Dogs. *Animals*, *14*(2), 300. https://doi.org/10.3390/ani14020300

Soltani, Z., & Siadati, S. (2019). *The impact of business intelligence on increasing the efficiency and health quality of surgical centers*. (Research on Health Management and Efficiency).

---

