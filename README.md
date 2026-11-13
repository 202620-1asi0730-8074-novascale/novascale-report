# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management


### 5.1.1. Software Development Environment Configuration

**Project Management:**

La gestión de los proyectos tiene como objetivo mejorar los procesos y su entorno para alcanzar los resultados esperados, facilitando la colaboración continua del equipo.

* **WhatsApp:** Canal de mensajería instantánea empleado para la comunicación síncrona, permitiendo consultas rápidas, toma de decisiones ágiles y una interacción constante entre los miembros del equipo de desarrollo.
* **Google Meet:** Plataforma de videoconferencia elegida como el espacio principal para llevar a cabo las reuniones periódicas (como los Daily Stand-ups), compartir pantalla en tiempo real y solucionar bloqueos técnicos de forma conjunta.

**Product UX/UI Design & Architecture:**

Nos permite desarrollar el modelo de nuestro producto de manera digital para que forme parte de la vida del consumidor. En este caso, realizar esquemas, diagramas de arquitectura y el diseño visual para computadoras y celulares.

* **UXPressia:** Herramienta en línea especializada en la gestión de requerimientos y diseño centrado en el usuario. Sus funcionalidades nos permitieron establecer las bases analíticas mediante la creación de User Personas, Empathy Maps y Journey Maps.
* **Figma:** Plataforma colaborativa de diseño de interfaces web, empleada para elaborar los esquemas estructurales (wireframes), las maquetas visuales (mock-ups) y los prototipos interactivos de alta fidelidad para el Landing Page y las aplicaciones.
* **Miro:** Es una pizarra digital interactiva en línea, utilizada para la investigación temprana, la ideación y la creación de lluvias de ideas.
* **PlantUML:** Herramienta de modelado bajo el enfoque *Diagram-as-Code*, utilizada para estructurar y documentar de manera programática la arquitectura del sistema y los diagramas de clases.
* **Trello:** Herramienta de gestión visual basada en tableros Kanban. Se ha adaptado en este contexto para organizar y hacer un seguimiento detallado de las tareas específicas correspondientes al diseño de experiencia de usuario y arquitectura.

**Software Development:**

Representa el marco metodológico y técnico empleado para la construcción del producto. Esta estructura define los procesos y actividades específicas que guían el ciclo de vida del desarrollo, asegurando un enfoque organizado para cada etapa de la implementación técnica.

* **GitHub:** Plataforma central de alojamiento que facilita el control de versiones distribuido y la gestión colaborativa de todo el código fuente del proyecto.
* **HTML:** Lenguaje de marcado estándar utilizado para definir la estructura semántica y el esqueleto del contenido de nuestras páginas web.
* **CSS:** Lenguaje de hojas de estilo encargado de la presentación visual, garantizando la estética, la adaptación responsiva en múltiples dispositivos y las animaciones de la interfaz.
* **JavaScript:** Lenguaje de programación empleado para dotar de interactividad dinámica al lado del cliente, gestionar eventos y aplicar la lógica de internacionalización en las vistas.
* **Vue.js:** Framework progresivo de JavaScript, seleccionado para la construcción robusta, ágil y basada en componentes de la aplicación web Frontend.
* **ASP.NET Core (C#):** Framework utilizado para el desarrollo del RESTful API y la gestión centralizada de la lógica de negocio, conexiones y servicios en el Backend.
* **MySQL Workbench:** Herramienta de software visual enfocada en el diseño, modelado y administración directa de las bases de datos relacionales requeridas por el sistema.

**Software Testing:**

Es el acto de examinar los artefactos y el comportamiento del software bajo prueba mediante procesos sistemáticos de validación y verificación.

* **Lenguaje Gherkin:** Es un DSL o Lenguaje Específico de Dominio creado para describir comportamientos del sistema de manera comprensible. Se utiliza para estructurar las historias de usuario y sus criterios de aceptación mediante la sintaxis: Feature, Scenario, Given, When, Then y And.


### 5.1.2. Source Code Management

En esta sección se presenta la gestión de código fuente o como es conocido por sus siglas en inglés SCM (Source Code Management). Su función principal es realizar un seguimiento de las modificaciones que el equipo realizará a lo largo del desarrollo de sus proyectos en los repositorios de código fuente. Se emplea como un sistema de control de versiones que permite dar seguimiento a los cambios que cada integrante o desarrollador realice en el proyecto. Asimismo, cabe resaltar que para el sistema de control de versiones emplearemos GitHub.

**Organización de Repositorios**

Para mantener la modularidad, el proyecto está dividido en repositorios independientes gestionados por la organización principal en GitHub.

* **Organización en GitHub (NovaScale):**

| **URL:** | https://github.com/202620-1asi0730-8074-novascale |
| :--- | :--- |

* **Repositorio del Landing Page:**

| **URL:** | https://github.com/202620-1asi0730-8074-novascale/novascale-website |
| :--- | :--- |

* **Repositorio del Frontend:**

| **URL:** | https://github.com/202620-1asi0730-8074-novascale/novascale-webapp |
| :--- | :--- |

* **Repositorio del Backend:**

| **URL:** | https://github.com/202620-1asi0730-8074-novascale/novascale-platform |
| :--- | :--- |

**GitFlow**

Es el modelo alternativo de creación de ramas en Git que en los últimos años se ha vuelto una herramienta indispensable para muchos desarrolladores. Este flujo de trabajo de control de versiones utiliza ramas y fue publicado y popularizado por Vincent Driessen. Su principal función es ayudar en la organización de la versión de un código, permitiendo la creación de nuevos Features y Hotfixes de manera organizada.

**Main Branches:**

* **main:** Es la rama principal de producción. A partir de ella se recorrerán todas las ramas y contendrá la última versión de código estable y las anteriores versiones definitivas creadas por los desarrolladores.
* **develop:** Esta rama de integración se crea a partir de la rama main y contará con todos los Features estables. Esto significa que a través de esta rama el equipo podrá integrar y probar las nuevas funciones de manera unificada.

**Support Branches:**

* **feature:** Se ramifica de develop y al finalizar el desarrollo debe fusionarse de nuevo obligatoriamente en develop. Se emplea para desarrollar historias de usuario individuales o nuevas funciones que se integrarán en versiones posteriores.
* **release:** También se ramifica de develop. Es la rama que admite la preparación, revisión final y estabilización de una nueva versión antes de su salida a producción.
* **hotfix:** Está destinada a corregir fallos en una nueva versión de producción, pero esta se ramifica directamente de main. Su función es reparar rápidamente emergencias o publicaciones de producción críticas sin alterar el trabajo en progreso.

**Conventional Commits:**

Son una convención estándar y obligatoria para nombrar los mensajes de commit en Git de forma estructurada, clara y semántica, facilitando la lectura del historial.

* **feat:** Se añade una nueva funcionalidad al software.
* **fix:** Se corrige un error de código o fallo en el sistema.
* **docs:** Cambios o agregados realizados exclusivamente en la documentación del proyecto.
* **style:** Cambios de formato o estilo de código (como puntos y comas, indentaciones) sin impacto en la lógica.
* **refactor:** Mejoras en la estructura del código que no añaden nuevas funcionalidades ni corrigen errores, pero optimizan el rendimiento o la lectura.
* **test:** Añadir nuevos escenarios de prueba o modificar tests existentes.
* **chore:** Cambios menores sin impacto en el código de producción (por ejemplo, actualización de dependencias, configuración de entornos, etc.).

### 5.1.3. Source Code Style Guide & Conventions

Para asegurar un código fácil de mantener, escalable y que favorezca el trabajo en equipo dentro del proyecto **NovaLeads** (nuestro CRM diseñado para pymes y startups), en NovaScale hemos establecido normativas de programación basadas en estándares globales. Una regla inquebrantable de este proyecto es que **todos los elementos del código fuente** (como nombres de variables, clases, métodos, ramas y comentarios) deben escribirse exclusivamente en **inglés**.

#### A. HTML5, CSS3 & JavaScript (Landing Page)
Para la creación de nuestra página web promocional, la cual se encuentra en el repositorio `novascale-website`, seguimos los lineamientos de la *Google HTML/CSS Style Guide* y las normativas de la *W3C*:

*   **HTML5:** Uso riguroso de etiquetas con valor semántico (`<header>`, `<section>`, `<article>`) para organizar visualmente los beneficios del CRM, aplicando siempre una indentación de 2 espacios.
*   **CSS3:** Adopción del patrón **BEM** (Block Element Modifier) utilizando la escritura en *kebab-case* para nombrar las clases de estilo (ej. `.pricing-card__button--active`).
*   **JavaScript:** Las interacciones del lado del cliente se rigen por las *MDN JavaScript Guidelines*, declarando funciones y variables en formato `camelCase`.

#### B. Vue.js & PrimeVue (Frontend Web Application)
El desarrollo de la plataforma web principal, enfocada en la gestión de los equipos de ventas y alojada en `novascale-webapp`, obedece al *Vue Style Guide* y se apoya en el sistema visual *Material Design* provisto por **PrimeVue**:

*   **Componentes (SFC):** Todo *Single-File Component* (`.vue`) debe nombrarse usando `PascalCase` y su título debe reflejar claramente su propósito en el sistema (ej. `LeadKanbanBoard.vue`, `SalesDashboard.vue`).
*   **Lógica y Variables:** Las propiedades reactivas y los métodos de JavaScript se redactan obligatoriamente en `camelCase`.
*   **Directivas:** Es imperativo usar la sintaxis abreviada de Vue (ej. `:` en lugar de `v-bind` y `@` en lugar de `v-on`) para garantizar que las plantillas sean fáciles de leer.

#### C. C# & ASP.NET Core (Backend - Iteraciones Futuras)
La arquitectura de nuestros Web Services RESTful, ubicados en el repositorio `novascale-platform`, se rige por las *Microsoft C# Coding Conventions* y las mejores prácticas de *ASP.NET Core*:

*   **Clases y Métodos:** Se exige el formato `PascalCase` para su declaración (ej. `LeadManagementController`).
*   **Interfaces:** Toda interfaz de dominio o técnica debe iniciar con la letra "I" mayúscula (ej. `IConversationService`).
*   **Variables Locales y Parámetros:** Se declaran utilizando `camelCase`.
*   **Estructura:** Implementamos *Entity Framework Core* como ORM para sincronizar con la base de datos previamente modelada en **MySQL Workbench**, y utilizamos XML Documentation (`///`) para describir el comportamiento de los endpoints.

#### D. Gherkin (Readable Specifications)
Los criterios de aceptación de nuestras Historias de Usuario se redactan bajo la estructura de **Gherkin** (`Given-When-Then`). Esta práctica certifica que el comportamiento esperado de la plataforma sea perfectamente comprensible para cualquier *stakeholder*, asegurando que cada función desarrollada mitigue los problemas de organización del equipo comercial.


### 5.1.4. Software Deployment Configuration

El ciclo de integración y entrega continua (CI/CD) de **NovaLeads** está completamente gestionado mediante **GitHub Actions**. Este mecanismo nos permite automatizar las validaciones y la publicación de código nuevo en la rama `main` (respetando nuestra metodología GitFlow), asegurando entregas rápidas y seguras.

Puesto que la meta principal de nuestra iteración actual (Sprint 1) fue cimentar la presencia operativa del producto a través de la Landing Page, nuestro pipeline de despliegue automatiza actualmente la salida a producción de las interfaces de usuario. Esto deja el terreno y la infraestructura en la nube preparados para conectar la lógica del backend en las fases posteriores.

#### Ecosistema de Despliegue

| Componente | Entorno de Hosting | Tecnologías y Estrategia de Despliegue |
| :--- | :--- | :--- |
| **Landing Page** | GitHub Pages | Servicio de alojamiento de sitios estáticos para el repositorio `novascale-website`. Se apoya en la CDN global de GitHub para brindar tiempos de respuesta óptimos, habiéndose desplegado de forma exitosa en el Sprint 1. |
| **Frontend Web App** | Amazon S3 & CloudFront | Distribución de los archivos compilados (`dist/`) de nuestra aplicación Vue alojada en `novascale-webapp`. CloudFront funciona como red de distribución de contenido (CDN) para el almacenamiento en caché y la administración de los certificados SSL. |
| **Web Services (Próximos Sprints)** | AWS Elastic Beanstalk | Plataforma como Servicio (PaaS) encargada de hospedar nuestra API RESTful programada en C# (`novascale-platform`), la cual cuenta con balanceo dinámico de carga. |
| **Database (Próximos Sprints)** | Amazon RDS | Motor de base de datos relacional MySQL (estructurado desde MySQL Workbench) y administrado en la nube de AWS. Cuenta con backups automatizados para proteger la información comercial. |

#### Pipeline de Despliegue (Pasos del CI/CD)

1. **Desarrollo y Testing Local:** Los programadores comprueban el correcto funcionamiento de los componentes en Vue y el diseño de la Landing Page directamente en sus equipos locales, verificando que el código cumpla con las directrices de estilo.
2. **Control de Versiones (GitFlow):** El código nuevo se envía (`git push`) a una rama de trabajo específica (`feature/*`). Posteriormente, se abre un *Pull Request* hacia la rama de integración `develop`, redactando los mensajes bajo la norma de *Conventional Commits*.
3. **Integración Continua (CI):** La creación de un *Pull Request* activa inmediatamente un *workflow* de GitHub Actions encargado de descargar las dependencias (`npm install`) y compilar la aplicación. Cualquier fallo en este proceso bloquea automáticamente la fusión del código.
4. **Despliegue Continuo (Frontend):** Una vez que el PR es revisado y fusionado hasta la rama `main`, GitHub Actions mueve los archivos finales de la Landing Page hacia la rama `gh-pages`. Al mismo tiempo, los binarios de la aplicación Web se cargan en el *bucket* de Amazon S3 y se ejecuta una invalidación de caché en CloudFront.
5. **Despliegue Backend (Futuro):** En los próximos sprints, el pipeline empaquetará la solución en C# (`dotnet publish`) y mandará los ejecutables hacia AWS Elastic Beanstalk, estableciendo finalmente la conexión con la base de datos Amazon RDS.

## 5.2. Landing Page, Services & Applications Implementation
En esta sección se detalla y evidencia el proceso continuo de implementación, pruebas de software, documentación técnica y despliegue en la nube de los componentes de la solución: Landing Page, RESTful Web Services y Frontend Web Applications. 
A partir de la priorización establecida en el Product Backlog, el desarrollo se ha estructurado mediante iteraciones ágiles, garantizando que tanto los procesos *core* del negocio como los procesos de soporte sean construidos y desplegados progresivamente aplicando principios de *Responsive Web Design*.

### 5.2.1. Sprint 1
En esta sección se registra y explica el avance obtenido durante el primer ciclo de desarrollo (Sprint 1), abarcando tanto la construcción de los productos de software iniciales como el trabajo colaborativo del equipo. Se incluyen los detalles de planificación, los líderes de cada aspecto, el backlog comprometido y las evidencias de ejecución, documentación y despliegue del trabajo completado.

#### 5.2.1.1. Sprint Planning 1
El Sprint Planning Meeting marcó el inicio formal del desarrollo. Durante esta sesión, se seleccionaron las Historias de Usuario más prioritarias del Product Backlog para definir el objetivo central de la iteración. A continuación, se presenta el cuadro resumen con los detalles y acuerdos de esta reunión:

| **Sprint #** | Sprint 1 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2026-08-26 |
| **Time** | 21:00 PM |
| **Location** | Reunión virtual (Google Meet) |
| **Prepared By** | Bottger Salazar, Johan Karl |
| **Attendees (to planning meeting)** | Johan, Renzo, Sergio, Lui, Dario |
| **Sprint n – 1 Review Summary** | - |
| **Sprint n – 1 Retrospective Summary** | - |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | **Contexto:** El equipo decidió enfocar el primer esfuerzo de codificación en sentar las bases operativas de la plataforma, desarrollando la Landing Page para presentar el producto. <br><br> **Sprint Goal:**<br>*"Our focus is on offering a reliable body of knowledge for future users of our CRM system, while establishing the product's digital presence through a responsive Landing Page.*<br>*We believe it delivers a trustworthy onboarding experience to administrators and clear product value proposition to prospective customers.*<br>*This will be confirmed when administrators and visitors can navigate the Landing Page features without errors."* |
| **Sprint 1 Velocity** | 67 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos). |
| **Sum of Story Points** | 67 Story Points. |

#### 5.2.1.2. Aspect Leaders and Collaborators

En esta sección se presenta la **Leadership-and-Collaboration Matrix (LACX)**. Esta matriz detalla los líderes (L) y colaboradores (C) para cada aspecto clave del Sprint, asegurando una comunicación clara y una distribución de responsabilidades eficiente para el proyecto. La organización está directamente relacionada con la selección de tareas (*tasks*) que se desarrollarán durante el Sprint.

| Team Member (First Name, Last Name) | GitHub Username | Arquitectura & DB | Backend API & Seguridad | Frontend (Landing & Web App) | QA & Deployment |
| :--- | :--- | :---: | :---: | :---: | :---: |
| Lui Mathias Gamero Miranda | lug07m | L | C | C | C |
| Dario Alberto Romero Vilela | patatitis9-alt | C | L | C | C |
| Johan Karl Bottger Salazar | Deskjobo | C | C | L | C |
| Sergio Ruben Caldas Garcia | Sergiocaldas10 | C | C | C | L |
| Renzo Paul Retuerto Zapata | Renzoocf | C | C | C | C |

#### 5.2.1.3. Sprint Backlog 1
Durante el primer sprint, el equipo se centró en desarrollar una landing page que fuera tanto atractiva como funcional, organizando y distribuyendo tareas en el tablero de Sprint de acuerdo con las habilidades de cada integrante.

##### **Sprint 1 - Tareas Asignadas**

| **User Story** |  | **Work-Item / Task** |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Id** | **Título** | **Id** | **Título** | **Descripción** | **Est. (Hrs)** | **Asignado** | **Status** |
| US-21 | Visualización de información del negocio | T-01 | Diseñar estructura de la Landing Page | Definir la estructura de las secciones principales y organizar la información de NovaLeads. | 3 | Lui | To Do |
| US-21 | Visualización de información del negocio | T-02 | Implementar información del negocio | Implementar las secciones principales con la propuesta de valor, funcionalidades y beneficios de NovaLeads. | 5 | Lui | To Do |
| US-22 | Información para dueños de pymes y startups | T-03 | Diseñar sección para dueños | Definir la estructura y contenido de la sección dirigida a dueños de pymes y startups. | 3 | Dario | To Do |
| US-22 | Información para dueños de pymes y startups | T-04 | Implementar contenido para dueños | Implementar la información relacionada con la gestión de leads, clientes, conversaciones y resultados de ventas. | 4 | Dario | To Do |
| US-23 | Información para equipos de ventas | T-05 | Diseñar sección para equipos de ventas | Definir la estructura y contenido de la sección dirigida a equipos de ventas. | 3 | Johan | To Do |
| US-23 | Información para equipos de ventas | T-06 | Implementar contenido para equipos de ventas | Implementar la información relacionada con leads, conversaciones y rendimiento del equipo. | 4 | Johan | To Do |
| US-24 | Navegación entre secciones | T-07 | Implementar menú de navegación | Crear el menú de navegación con enlaces hacia las principales secciones de la Landing Page. | 3 | Sergio | To Do |
| US-24 | Navegación entre secciones | T-08 | Implementar navegación interna | Configurar y validar el desplazamiento hacia las secciones correspondientes. | 3 | Sergio | To Do |
| US-25 | Call to Action para dueños | T-09 | Diseñar Call to Action para dueños | Diseñar el Call to Action dirigido a dueños de pymes y startups. | 2 | Renzo | To Do |
| US-25 | Call to Action para dueños | T-10 | Implementar flujo del Call to Action | Implementar y validar la acción que permita al visitante iniciar el flujo correspondiente. | 3 | Renzo | To Do |
| US-26 | Call to Action para equipos de ventas | T-11 | Diseñar Call to Action para equipos de ventas | Diseñar el Call to Action dirigido a equipos de ventas. | 2 | Lui | To Do |
| US-26 | Call to Action para equipos de ventas | T-12 | Implementar flujo del Call to Action | Implementar y validar la acción que permita al visitante iniciar el flujo correspondiente. | 3 | Lui | To Do |
| US-27 | Visualización responsive | T-13 | Adaptar Landing Page a dispositivos | Adaptar la estructura y los componentes de la Landing Page para desktop, tablet y dispositivos móviles. | 5 | Johan | To Do |
| US-27 | Visualización responsive | T-14 | Validar comportamiento responsive | Verificar la correcta visualización y funcionamiento de la Landing Page en diferentes tamaños de pantalla. | 3 | Johan | To Do |
| TS-02 | Autenticación de usuarios | T-15 | Implementar servicio de autenticación | Configurar la comunicación del frontend con el endpoint de autenticación y procesar sus respuestas. | 5 | Renzo | To Do |
| TS-02 | Autenticación de usuarios | T-16 | Validar autenticación | Verificar el comportamiento del frontend ante credenciales válidas, inválidas y respuestas HTTP de error. | 3 | Renzo | To Do |
| — | — | T-17 | Configurar estructura base del frontend | Configurar la estructura inicial del proyecto frontend y los recursos necesarios para el desarrollo del Sprint. | 3 | Sergio | To Do |
| — | — | T-18 | Configurar dependencias del proyecto | Instalar y configurar las dependencias requeridas según las tecnologías definidas para el proyecto. | 2 | Sergio | To Do |
| — | — | T-19 | Configurar control de versiones | Configurar la estructura de ramas y realizar la integración del trabajo del Sprint en el repositorio. | 2 | Sergio | To Do |
| — | — | T-20 | Aplicar lineamientos visuales generales | Aplicar los lineamientos definidos en el Web Style Guide relacionados con espaciado, dimensiones, tipografía y comunicación. | 3 | Dario | To Do |
| — | — | T-21 | Realizar integración de componentes | Integrar las secciones, navegación y Call to Action desarrollados durante el Sprint en una única Landing Page funcional. | 2 | Sergio | To Do |



#### 5.2.1.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 1 fue el desarrollo de la Landing Page institucional del producto. 
A continuación, se presentan los commits más importantes del Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo del Landing Page.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| novaleads-website | main | 2cba00275bc03d34bcf17822454a79e95efd4182 | feat: Landing Page initial commit | - | 17-09-2026 |
| novaleads-website | main | b3cc5e18a42399f9cd1ca8f89190f2ab0d602d5c | feat: Add pricing and footer styles | - | 17-09-2026 |
| novaleads-website | main | 5cc2120d85e1037a4508f406159024d4a27752ef | feat: add app.js | - | 17-09-2026 |


#### 5.2.1.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución de la Landing Page de la aplicación como evidencia. La Landing Page es compuesta por varias secciones que se presentan en las capturas a continuación.

<img src="Resources/Chapter5/sprint1/execution1.png"/>
<img src="Resources/Chapter5/sprint1/execution2.png"/>

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
No aplica a primer sprint y desarrollo de Landing Page.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.
El despliegue de la Landing Page se realizó en el servicio de Github Pages, se seleccionó esta alternativa debido a la rapidez de despliegue y su sencillez, apropiada para una página estática.
Se incluye la evidencia de despliegue del Landing Page en la plataforma Github Pages: [https://202620-1asi0730-8074-novascale.github.io/novascale-website/](https://202620-1asi0730-8074-novascale.github.io/novascale-website/)

<img src="Resources/Chapter5/sprint1/deployment1.png"/>
<img src="Resources/Chapter5/sprint1/deployment2.png"/>

#### 5.2.1.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 1:

<img src="Resources/Chapter5/sprint1/collab1.png"/>


____


### 5.2.2. Sprint 2
En esta sección se registra y explica el avance obtenido durante el segundo ciclo de desarrollo (Sprint 2), abarcando la construcción de los productos de software intermedios y el trabajo colaborativo del equipo. Se incluyen los detalles de planificación, los líderes de cada aspecto, el backlog comprometido y las evidencias de ejecución, documentación y despliegue del trabajo completado.

#### 5.2.2.1. Sprint Planning 2
Durante esta sesión, se seleccionaron las Historias de Usuario más prioritarias del Product Backlog para definir el objetivo central de la iteración. A continuación, se presenta el cuadro resumen con los detalles y acuerdos de esta reunión:

| **Sprint #** | Sprint 2 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2026-09-21 |
| **Time** | 21:00 PM |
| **Location** | Reunión virtual (Google Meet) |
| **Prepared By** | Bottger Salazar, Johan Karl |
| **Attendees (to planning meeting)** | Johan, Renzo, Sergio, Lui, Dario |
| **Sprint 1 Review Summary** | Durante el Sprint 1 el equipo logró completar la primera versión funcional de la Landing Page. Se cumplió el objetivo principal del sprint de habilitar la presencia digital del producto y redactar el tronco del conocimiento relacionado a la solución. |
| **Sprint 1 Retrospective Summary** | La comunicación entre integrantes fue constante y facilitó la integración temprana. Mantener documentación y estándares técnicos actualizados durante el sprint. |
| **Sprint Goal & User Stories** | |
| **Sprint 2 Goal** | **Contexto:** El equipo decidió enfocar el trabajo en el desarrollo del Frontend Web Application. <br><br> **Sprint Goal:**<br>*"Our focus is on delivering the first operational version of the NovaLeads Web Application while improving the quality, usability, and stability of artifacts created during Sprint 1.
We believe this delivers a more complete digital experience to administrators and prospective customers by providing the first functional version of the Frontend Web Application.
This will be confirmed when users can access the deployed web application, navigate the improved Landing Page without usability issues, and interact successfully with the first administrative frontend modules in a production-like environment."* |
| **Sprint 2 Velocity** | XX Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos). |
| **Sum of Story Points** | XX Story Points. |

#### 5.2.2.2. Aspect Leaders and Collaborators

En esta sección se presenta la **Leadership-and-Collaboration Matrix (LACX)**. Esta matriz detalla los líderes (L) y colaboradores (C) para cada aspecto clave del Sprint, asegurando una comunicación clara y una distribución de responsabilidades eficiente para el proyecto. La organización está directamente relacionada con la selección de tareas (*tasks*) que se desarrollarán durante el Sprint.

| Team Member (First Name, Last Name) | GitHub Username | Dashboard | Conversations | Authentication | Leads | QA & Deployment |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| Lui Mathias Gamero Miranda | lug07m | C | L | C | C | C |
| Dario Alberto Romero Vilela | patatitis9-alt | C | C | L | C | C |
| Johan Karl Bottger Salazar | Deskjobo | C | C | C | C | L |
| Sergio Ruben Caldas Garcia | Sergiocaldas10 | L | C | C | C | C |
| Renzo Paul Retuerto Zapata | Renzoocf | C | C | C | L | C |

#### 5.2.2.3. Sprint Backlog 2
Durante el segundo sprint, el equipo se centró en desarrollar la primera versión del Web Application funcional, organizando y distribuyendo tareas en el tablero de Sprint de acuerdo con las habilidades de cada integrante.

##### Sprint 2 - Tareas Asignadas

| User Story | Título | Work-Item / Task | Título | Descripción | Est. (Hrs) | Asignado | Status |
| :--- | :--- | :--- | :--- | :--- | ---: | :--- | :--- |
| US-01 | Inicio de sesión | T-01 | Implementar inicio de sesión y manejo de sesión | Implementar el formulario de autenticación, integrarlo con el servicio correspondiente y gestionar la respuesta y sesión del usuario. | 8 | Renzo | To Do |
| US-02 | Gestión de usuarios y permisos | T-02 | Implementar gestión de usuarios y permisos | Implementar la consulta de usuarios vendedores y la modificación y validación de los permisos asignados. | 8 | Dario | To Do |
| US-03 | Dashboard del dueño | T-03 | Implementar dashboard e indicadores del negocio | Implementar la consulta y presentación de los indicadores generales de leads y ventas mediante los gráficos correspondientes. | 8 | Lui | To Do |
| US-04 | Dashboard del vendedor | T-04 | Implementar dashboard y validación de indicadores personales | Implementar la consulta y presentación de los indicadores del vendedor autenticado y validar que únicamente pueda consultar sus propios resultados. | 7 | Johan | To Do |
| US-05 | Visualización de ventas por vendedor | T-05 | Implementar visualización de ventas por vendedor | Implementar la consulta y presentación de las ventas asociadas a cada vendedor para usuarios con permisos de dueño. | 7 | Sergio | To Do |
| US-06 | Registro de leads | T-06 | Implementar registro y validación de leads | Implementar el formulario de registro de leads, integrarlo con el servicio de creación y validar la información requerida. | 8 | Dario | To Do |
| US-07 | Filtrado de leads | T-07 | Implementar consulta y filtrado de leads | Implementar la obtención de leads disponibles y su filtrado mediante criterios como estado, vendedor y etiqueta. | 7 | Lui | To Do |
| US-08 | Cambio de estado de un lead | T-08 | Implementar actualización y validación de estados | Implementar la modificación del estado de un lead y validar los valores permitidos y las respuestas ante valores no válidos. | 7 | Johan | To Do |
| US-09 | Etiquetado de leads por producto | T-09 | Implementar etiquetado de leads por producto | Implementar la consulta de etiquetas disponibles y la asignación de una o más etiquetas de producto a un lead. | 7 | Sergio | To Do |
| US-10 | Gestión de etiquetas | T-10 | Implementar gestión de etiquetas | Implementar la creación y edición de etiquetas de productos para usuarios con permisos de gestión, incluyendo la gestión de sus asociaciones con leads. | 8 | Dario | To Do |
| US-11 | Visualización de contactos | T-11 | Implementar visualización de contactos | Implementar la consulta y presentación de los contactos disponibles según los permisos del usuario. | 6 | Lui | To Do |
| US-12 | Clasificación de contacto | T-12 | Implementar clasificación de contactos | Implementar la consulta y presentación de la clasificación de cada contacto como lead o cliente. | 5 | Sergio | To Do |
| US-13 | Edición de información de contacto | T-13 | Implementar edición y validación de contactos | Implementar la modificación de información de contactos autorizados, integrarla con la API y gestionar las validaciones y restricciones de permisos. | 7 | Renzo | To Do |
| US-14 | Creación automática de contactos | T-14 | Implementar sincronización automática de contactos | Integrar el frontend con la información de contactos generada automáticamente a partir de conversaciones y verificar la correcta sincronización de contactos nuevos y existentes. | 8 | Johan | To Do |
| US-15 | Visualización de conversaciones | T-15 | Implementar visualización e historial de conversaciones | Implementar la consulta y presentación de las conversaciones disponibles y del historial de mensajes de una conversación seleccionada. | 9 | Lui | To Do |
| US-16 | Notificación de nuevos mensajes | T-16 | Implementar notificaciones y actualización de conversaciones | Integrar la recepción de notificaciones de nuevos mensajes y actualizar la información de las conversaciones correspondientes. | 7 | Sergio | To Do |
| US-17 | Temporizador de conversaciones | T-17 | Implementar temporizador de conversaciones | Implementar el cálculo y actualización del tiempo transcurrido desde la recepción de un mensaje pendiente de respuesta. | 6 | Dario | To Do |
| US-18 | Prioridad automática de conversaciones | T-18 | Implementar prioridad automática de conversaciones | Integrar la información de prioridad calculada y actualizar las conversaciones cuando la prioridad cambia según el umbral definido. | 7 | Johan | To Do |
| US-19 | Ordenamiento y filtrado de conversaciones | T-19 | Implementar ordenamiento y filtrado de conversaciones | Implementar el ordenamiento y filtrado de conversaciones utilizando criterios de prioridad, etiquetas y vendedor según los permisos disponibles. | 8 | Renzo | To Do |
| US-20 | Perfil del vendedor | T-20 | Implementar consulta y edición del perfil | Implementar la consulta y modificación de la información autorizada del perfil del vendedor autenticado, incluyendo sus validaciones. | 7 | Sergio | To Do |
| TS-01 | Documentación OpenAPI | T-21 | Configurar y validar documentación OpenAPI | Configurar la documentación automática de los endpoints mediante OpenAPI/Swagger y verificar que recursos, métodos, respuestas y esquemas estén documentados correctamente. | 4 | Renzo | To Do |
| TS-02 | Autenticación de usuarios | T-22 | Implementar y validar API de autenticación | Implementar el endpoint RESTful para autenticar usuarios y generar el token de acceso, validando credenciales, respuestas y códigos HTTP correspondientes. | 8 | Renzo | To Do |
| TS-03 | API de gestión de Leads | T-23 | Implementar y validar API de Leads | Implementar los endpoints RESTful para registrar y consultar leads, incluyendo las validaciones de datos y respuestas HTTP correspondientes. | 10 | Dario | To Do |
| TS-04 | API de gestión de Contactos | T-24 | Implementar y validar API de Contactos | Implementar los endpoints RESTful para consultar y actualizar contactos, incluyendo las validaciones de permisos y respuestas HTTP correspondientes. | 9 | Lui | To Do |
| TS-05 | API de conversaciones | T-25 | Implementar y validar API de conversaciones | Implementar los endpoints RESTful para consultar y gestionar conversaciones e historial de mensajes, incluyendo autorización y respuestas para recursos existentes, inexistentes o no autorizados. | 9 | Johan | To Do |
| TS-06 | API de Dashboard y métricas | T-26 | Implementar y validar API de métricas | Implementar los endpoints RESTful para obtener indicadores de ventas y leads según el rol, validando datos, permisos y períodos sin información. | 9 | Sergio | To Do |
| TS-07 | Manejo de errores y respuestas HTTP | T-27 | Implementar y validar manejo estandarizado de errores | Implementar un mecanismo común para gestionar errores y generar respuestas HTTP consistentes, verificando solicitudes inválidas, recursos inexistentes, accesos no autorizados y errores internos. | 7 | Dario | To Do |


#### 5.2.2.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 2 fue el desarrollo del Frontend Web Application del producto. 
A continuación, se presentan los commits más importantes del Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| novaleads-webapp | main | 7232b642decc898fccb61cf8274f89b5b18eb295 | feat: Initial frontend commit | - | 6-10-2026 |
| novaleads-webapp | feature/authentication | 62472074af1f6030186ed13777b84aab05444b79 | feat(authentication): add frontend authentication module layers | - | 6-10-2026 |
| novaleads-webapp | feature/conversations | e8bab0c9d6f1303c0d14eaa13a6034dd19201494 | feat(conversations): add frontend conversations | - | 6-10-2026 |
| novaleads-webapp | feature/dashboard | 537b42fda98eafb6f8c599e15c4f4e345b57165a | feat(dashboard): add dashboards and reports | - | 6-10-2026 |
| novaleads-webapp | feature/leads | ed2da282fe144471657364868c7d9519e88ef20c | feat(leads): add frontend leads module | - | 7-10-2026 |



#### 5.2.2.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución del Frontend Web Application como evidencia.

<img src="Resources/Chapter5/sprint2/execution1.png"/>
<img src="Resources/Chapter5/sprint2/execution2.png"/>
<img src="Resources/Chapter5/sprint2/execution3.png"/>

#### 5.2.2.6. Services Documentation Evidence for Sprint Review.
Se incluyen capturas detalladas de los servicios utilizados por el Frontend Web Application, correspondientes a un fakeapi bajo el alcance del sprint.

<img src="Resources/Chapter5/sprint2/services1.png"/>

URL de la fake api: https://novaleads-api.onrender.com/users

#### 5.2.2.7. Software Deployment Evidence for Sprint Review.

El despliegue del Frontend Web Application se realizó en el servicio de , se seleccionó esta alternativa debido a su rapidez de despliegue y accesibilidad.

Se incluye la evidencia de despliegue: []()

<img src="Resources/Chapter5/sprint2/deployment1.png"/>
<img src="Resources/Chapter5/sprint2/deployment2.png"/>
<img src="Resources/Chapter5/sprint2/deployment3.png"/>

URL: https://novaleads.onrender.com

#### 5.2.2.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 2:

<img src="Resources/Chapter5/sprint2/collab1.png"/>
<img src="Resources/Chapter5/sprint2/collab2.png"/>



____


### 5.2.3. Sprint 3
En esta sección se registra y explica el avance obtenido durante el tercer ciclo de desarrollo (Sprint 3), abarcando la construcción de los productos de software finales, la validación y el trabajo colaborativo del equipo. Se incluyen los detalles de planificación, los líderes de cada aspecto, el backlog comprometido y las evidencias de ejecución, documentación y despliegue del trabajo completado.

#### 5.2.3.1. Sprint Planning 3
Durante esta sesión, se seleccionaron las Historias de Usuario más prioritarias del Product Backlog para definir el objetivo central de la iteración. A continuación, se presenta el cuadro resumen con los detalles y acuerdos de esta reunión:

| **Sprint #** | Sprint 3 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2026-11-01 |
| **Time** | 21:00 PM |
| **Location** | Reunión virtual (Google Meet) |
| **Prepared By** | Bottger Salazar, Johan Karl |
| **Attendees (to planning meeting)** | Johan, Renzo, Sergio, Lui, Dario |
| **Sprint 2 Review Summary** | Durante el Sprint 2 el equipo logró completar la primera versión funcional del frontend web application y una nueva versión del Landing Page. Se cumplió el objetivo principal del sprint de la primera versión operacional de NovaLeads. |
| **Sprint 2 Retrospective Summary** | La comunicación entre integrantes fue constante y facilitó la integración temprana. Mantener documentación y estándares técnicos actualizados durante el sprint. |
| **Sprint Goal & User Stories** | |
| **Sprint 3 Goal** | **Contexto:** El equipo decidió enfocar el trabajo en el desarrollo del Backend Web Services. <br><br> **Sprint Goal:**<br>*"Our focus is on delivering the first operational version of the NovaLeads backend web services while improving the quality, usability, and stability of artifacts created during previous sprints.
We believe this delivers a more complete digital experience to administrators and prospective customers by providing the first functional version of the Backend Web Service.
This will be confirmed when users can access the deployed service through our frontend, navigate the improved Landing Page and frontend web application without usability issues, and interact successfully over the first backend modules in a production-like environment."* |
| **Sprint 3 Velocity** | 216 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos). |
| **Sum of Story Points** | 216 Story Points. |

#### 5.2.3.2. Aspect Leaders and Collaborators

En esta sección se presenta la **Leadership-and-Collaboration Matrix (LACX)**. Esta matriz detalla los líderes (L) y colaboradores (C) para cada aspecto clave del Sprint, asegurando una comunicación clara y una distribución de responsabilidades eficiente para el proyecto. La organización está directamente relacionada con la selección de tareas (*tasks*) que se desarrollarán durante el Sprint.

| Team Member (First Name, Last Name) | GitHub Username | IdentityAccess | LeadManagement| SalesManagement | ConversationManagement | QA & Deployment |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| Lui Mathias Gamero Miranda | lug07m | C | C | C | C | L |
| Dario Alberto Romero Vilela | patatitis9-alt | L | C | C | C | C |
| Johan Karl Bottger Salazar | Deskjobo | C | C | C | L | C |
| Sergio Ruben Caldas Garcia | Sergiocaldas10 | C | C | L | C | C |
| Renzo Paul Retuerto Zapata | Renzoocf | C | L | C | C | C |

#### 5.2.3.3. Sprint Backlog 3
Durante el tercer sprint, el equipo se centró en desarrollar la primera versión de los Web Services funcionales, organizando y distribuyendo tareas en el tablero de Sprint de acuerdo con las habilidades de cada integrante.

##### Sprint 3 - Tareas Asignadas


| User Story | Título | Work-Item / Task | Título | Descripción | Est. (Hrs) | Asignado | Status |
| :--- | :--- | :--- | :--- | :--- | ---: | :--- | :--- |
| US-01 | Inicio de sesión | T-01 | Implementar servicio de autenticación | Implementar la lógica de autenticación de usuarios, verificando las credenciales registradas en la base de datos. | 5 | Renzo | To Do |
| US-01 | Inicio de sesión | T-02 | Implementar generación y validación de tokens | Implementar la generación de tokens de acceso y los mecanismos necesarios para validar la identidad del usuario autenticado. | 4 | Renzo | To Do |
| US-02 | Gestión de usuarios y permisos | T-03 | Implementar consulta de usuarios y permisos | Implementar las consultas a la base de datos para obtener usuarios vendedores y sus permisos asociados. | 5 | Renzo | To Do |
| US-02 | Gestión de usuarios y permisos | T-04 | Implementar actualización de permisos | Implementar la lógica de actualización de permisos, verificando las autorizaciones del usuario que realiza la operación. | 4 | Renzo | To Do |
| US-03 | Dashboard del dueño | T-05 | Implementar consultas de métricas generales | Implementar las consultas a la base de datos para obtener indicadores generales de leads y ventas del negocio. | 5 | Lui | To Do |
| US-03 | Dashboard del dueño | T-06 | Implementar servicio de métricas del negocio | Implementar el servicio que procesa y proporciona los indicadores generales correspondientes al usuario con permisos de dueño. | 4 | Lui | To Do |
| US-04 | Dashboard del vendedor | T-07 | Implementar consultas de métricas personales | Implementar las consultas necesarias para obtener los indicadores de ventas asociados al vendedor autenticado. | 4 | Sergio | To Do |
| US-04 | Dashboard del vendedor | T-08 | Implementar validación de acceso a métricas | Implementar las restricciones de acceso para garantizar que cada vendedor consulte únicamente sus propios resultados. | 4 | Sergio | To Do |
| US-05 | Visualización de ventas por vendedor | T-09 | Implementar consulta de ventas por vendedor | Implementar las consultas a la base de datos para obtener las ventas agrupadas según el vendedor responsable. | 4 | Sergio | To Do |
| US-05 | Visualización de ventas por vendedor | T-10 | Implementar servicio de ventas por vendedor | Implementar el servicio que procesa y proporciona la información de ventas individuales al usuario con permisos de dueño. | 4 | Sergio | To Do |
| US-06 | Registro de leads | T-11 | Implementar persistencia de leads | Implementar la lógica de creación y almacenamiento de nuevos leads en la base de datos. | 5 | Dario | To Do |
| US-06 | Registro de leads | T-12 | Implementar validación de registro de leads | Implementar las validaciones de información requerida y las restricciones correspondientes antes de registrar un lead. | 4 | Dario | To Do |
| US-07 | Filtrado de leads | T-13 | Implementar consultas de leads | Implementar las consultas a la base de datos para obtener los leads disponibles según los permisos del usuario. | 4 | Dario | To Do |
| US-07 | Filtrado de leads | T-14 | Implementar filtros de leads en API | Implementar los parámetros de filtrado por estado, vendedor y etiqueta en los servicios de consulta de leads. | 4 | Dario | To Do |
| US-08 | Cambio de estado de un lead | T-15 | Implementar actualización de estado de leads | Implementar la lógica de modificación del estado de un lead y persistir los cambios en la base de datos. | 4 | Dario | To Do |
| US-08 | Cambio de estado de un lead | T-16 | Implementar validación de estados permitidos | Implementar las validaciones de estados disponibles y gestionar las respuestas ante modificaciones no válidas. | 3 | Dario | To Do |
| US-09 | Etiquetado de leads por producto | T-17 | Implementar consulta de etiquetas de productos | Implementar las consultas para obtener las etiquetas de productos disponibles en la base de datos. | 4 | Dario | To Do |
| US-09 | Etiquetado de leads por producto | T-18 | Implementar asociación de etiquetas a leads | Implementar la lógica de asociación y almacenamiento de una o más etiquetas de productos vinculadas a un lead. | 4 | Dario | To Do |
| US-10 | Gestión de etiquetas | T-19 | Implementar creación de etiquetas | Implementar la lógica de creación y persistencia de nuevas etiquetas de productos, verificando los permisos correspondientes. | 4 | Lui | To Do |
| US-10 | Gestión de etiquetas | T-20 | Implementar actualización de etiquetas | Implementar la modificación de etiquetas existentes y gestionar la consistencia de sus asociaciones con los leads. | 4 | Lui | To Do |
| US-11 | Visualización de contactos | T-21 | Implementar consultas de contactos | Implementar las consultas a la base de datos para obtener los contactos registrados según los permisos del usuario. | 4 | Lui | To Do |
| US-11 | Visualización de contactos | T-22 | Implementar servicio de consulta de contactos | Implementar el servicio RESTful para proporcionar la información de contactos solicitada. | 3 | Lui | To Do |
| US-12 | Clasificación de contacto | T-23 | Implementar clasificación de contactos | Implementar la lógica para identificar y obtener la clasificación de cada contacto como lead o cliente. | 3 | Lui | To Do |
| US-12 | Clasificación de contacto | T-24 | Implementar persistencia de clasificación | Implementar el almacenamiento y consulta de la clasificación correspondiente a cada contacto. | 3 | Lui | To Do |
| US-13 | Edición de información de contacto | T-25 | Implementar actualización de contactos | Implementar la lógica de modificación y persistencia de la información de contactos existentes. | 4 | Sergio | To Do |
| US-13 | Edición de información de contacto | T-26 | Implementar validación de actualización de contactos | Implementar las validaciones de información y permisos necesarios para actualizar los datos de un contacto. | 4 | Sergio | To Do |
| US-14 | Creación automática de contactos | T-27 | Implementar recepción de mensajes de WhatsApp | Implementar el procesamiento de los eventos recibidos mediante la integración de WhatsApp para identificar nuevos contactos. | 5 | Johan | To Do |
| US-14 | Creación automática de contactos | T-28 | Implementar creación y sincronización de contactos | Implementar la lógica para registrar automáticamente contactos nuevos y conservar los existentes cuando reciben nuevos mensajes. | 4 | Johan | To Do |
| US-15 | Visualización de conversaciones | T-29 | Implementar consultas de conversaciones | Implementar las consultas a la base de datos para obtener las conversaciones asociadas a los contactos y vendedores. | 5 | Johan | To Do |
| US-15 | Visualización de conversaciones | T-30 | Implementar consulta de historial de mensajes | Implementar el servicio para obtener el historial de mensajes asociado a una conversación seleccionada. | 4 | Johan | To Do |
| US-16 | Notificación de nuevos mensajes | T-31 | Implementar procesamiento de nuevos mensajes | Implementar el procesamiento de mensajes entrantes y su asociación con las conversaciones correspondientes. | 5 | Johan | To Do |
| US-16 | Notificación de nuevos mensajes | T-32 | Implementar generación de notificaciones | Implementar el mecanismo backend para generar y distribuir notificaciones cuando se reciben nuevos mensajes. | 4 | Johan | To Do |
| US-17 | Temporizador de conversaciones | T-33 | Implementar cálculo de tiempo pendiente | Implementar la lógica para calcular el tiempo transcurrido desde la recepción de un mensaje pendiente de respuesta. | 3 | Johan | To Do |
| US-17 | Temporizador de conversaciones | T-34 | Implementar servicio de tiempo de conversación | Implementar el servicio para proporcionar el tiempo pendiente de respuesta correspondiente a cada conversación activa. | 3 | Johan | To Do |
| US-18 | Prioridad automática de conversaciones | T-35 | Implementar cálculo de prioridad de conversaciones | Implementar la lógica de asignación automática de prioridad según el tiempo transcurrido sin respuesta y el umbral definido. | 4 | Sergio | To Do |
| US-18 | Prioridad automática de conversaciones | T-36 | Implementar actualización de prioridades | Implementar el mecanismo de actualización de prioridades y persistencia de los cambios en las conversaciones correspondientes. | 4 | Sergio | To Do |
| US-19 | Ordenamiento y filtrado de conversaciones | T-37 | Implementar consultas y ordenamiento de conversaciones | Implementar las consultas necesarias para ordenar las conversaciones según los criterios disponibles. | 4 | Renzo | To Do |
| US-19 | Ordenamiento y filtrado de conversaciones | T-38 | Implementar filtros de conversaciones | Implementar los filtros por prioridad, etiquetas y vendedor, considerando los permisos del usuario autenticado. | 4 | Renzo | To Do |
| US-20 | Perfil del vendedor | T-39 | Implementar consulta de perfil de usuario | Implementar el servicio para obtener la información del perfil del vendedor autenticado desde la base de datos. | 4 | Renzo | To Do |
| US-20 | Perfil del vendedor | T-40 | Implementar actualización de perfil | Implementar la modificación y persistencia de la información autorizada del perfil del vendedor, incluyendo sus validaciones. | 3 | Renzo | To Do |
| TS-01 | Documentación OpenAPI | T-41 | Configurar documentación OpenAPI | Configurar Swagger/OpenAPI para documentar automáticamente los endpoints, modelos y esquemas disponibles en el backend. | 2 | Renzo | To Do |
| TS-01 | Documentación OpenAPI | T-42 | Validar documentación de API | Verificar que los recursos, métodos HTTP, parámetros, esquemas y respuestas de los servicios estén documentados correctamente. | 2 | Renzo | To Do |
| TS-02 | Autenticación de usuarios | T-43 | Implementar endpoint RESTful de autenticación | Implementar el endpoint POST de autenticación para validar credenciales y generar el token de acceso correspondiente. | 5 | Renzo | To Do |
| TS-02 | Autenticación de usuarios | T-44 | Validar respuestas de autenticación | Verificar las respuestas HTTP para credenciales válidas e inválidas, incluyendo los códigos 200 OK y 401 Unauthorized. | 3 | Renzo | To Do |
| TS-03 | API de gestión de Leads | T-45 | Implementar endpoints RESTful de leads | Implementar los endpoints necesarios para registrar y consultar leads mediante los métodos HTTP correspondientes. | 6 | Dario | To Do |
| TS-03 | API de gestión de Leads | T-46 | Validar datos y respuestas de API de leads | Verificar las validaciones de datos, persistencia y respuestas HTTP de las operaciones de creación y consulta de leads. | 4 | Dario | To Do |
| TS-04 | API de gestión de Contactos | T-47 | Implementar endpoints RESTful de contactos | Implementar los endpoints para consultar y actualizar contactos mediante los recursos correspondientes de la API. | 5 | Lui | To Do |
| TS-04 | API de gestión de Contactos | T-48 | Validar permisos y respuestas de API de contactos | Verificar las restricciones de acceso, validaciones y respuestas HTTP para las operaciones sobre contactos. | 4 | Lui | To Do |
| TS-05 | API de conversaciones | T-49 | Implementar endpoints RESTful de conversaciones | Implementar los endpoints para consultar conversaciones e historiales de mensajes asociados a los contactos. | 5 | Johan | To Do |
| TS-05 | API de conversaciones | T-50 | Validar autorización y respuestas de API de conversaciones | Verificar los permisos de acceso y las respuestas HTTP para conversaciones existentes, inexistentes o no autorizadas. | 4 | Johan | To Do |
| TS-06 | API de Dashboard y métricas | T-51 | Implementar endpoints RESTful de métricas | Implementar los endpoints para obtener indicadores de ventas y leads según el rol y permisos del usuario autenticado. | 5 | Sergio | To Do |
| TS-06 | API de Dashboard y métricas | T-52 | Validar métricas y permisos | Verificar los resultados de las consultas, restricciones de acceso y respuestas para períodos sin información. | 4 | Sergio | To Do |
| TS-07 | Manejo de errores y respuestas HTTP | T-53 | Implementar manejo estandarizado de errores | Implementar un mecanismo centralizado para gestionar excepciones y generar respuestas HTTP consistentes en los servicios backend. | 4 | Dario | To Do |
| TS-07 | Manejo de errores y respuestas HTTP | T-54 | Validar respuestas de error | Verificar las respuestas para solicitudes inválidas, recursos inexistentes, accesos no autorizados y errores internos del servidor. | 3 | Dario | To Do |
| **Total** | **216** |


#### 5.2.3.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 3 fue el desarrollo del Backend Web Services del producto. 
A continuación, se presentan los commits más importantes del Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| novascale-platform | feature/platform-foundation | bb5627787e8e6eb542350e6b8299e1df38f96fd0 | feat: add shared backend foundation | - | 12-11-2026 |
| novascale-platform | feature/conversation-management | edc4ceeb4dba3095cf2213a8d4a0376fc8359c62 | feat(ConversationManagement): Bounded Context completed | - | 12-11-2026 |
| novascale-platform | feature/identity-access | 52e6a8df9f1dc4d8499d35f8207d6a8d99a53d4c | feat(IdentityAccess): add full bounded context | - | 12-11-2026 |
| novascale-platform | feature/lead-management | b3004b3fca47da9be6d19e4421dcb76da1e1491f | feat(LeadManagement): add full bounded context | - | 12-11-2026 |
| novascale-platform | feature/sales-management | ab1b84a40eb70a24e03563f25abcfd327dc6e48c | feat(LeadManagement): add full bounded context | - | 12-11-2026 |



#### 5.2.3.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución del Backend Web Services como evidencia.

<img src="Resources/Chapter5/sprint3/execution1.png"/>
<img src="Resources/Chapter5/sprint3/execution2.png"/>
<img src="Resources/Chapter5/sprint3/execution3.png"/>

#### 5.2.3.6. Services Documentation Evidence for Sprint Review.
Se incluyen capturas detalladas de la documentación del Backend Web Services.

<img src="Resources/Chapter5/sprint3/services1.png"/>


#### 5.2.3.7. Software Deployment Evidence for Sprint Review.

El despliegue del Backend Web Service se realizó en el servicio de , se seleccionó esta alternativa debido a su rapidez de despliegue y accesibilidad.

Se incluye la evidencia de despliegue:

<img src="Resources/Chapter5/sprint3/deployment1.png"/>
<img src="Resources/Chapter5/sprint3/deployment2.png"/>
<img src="Resources/Chapter5/sprint3/deployment3.png"/>

URL: 

#### 5.2.3.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 2:

<img src="Resources/Chapter5/sprint3/collab1.png"/>
<img src="Resources/Chapter5/sprint3/collab2.png"/>






---
# 5.3. Validation Interviews

## 5.3.1. Diseño de Entrevistas

Con el objetivo de validar la usabilidad, funcionalidad y eficiencia de NovaLeads, se diseñaron entrevistas dirigidas a los dos segmentos objetivo de la plataforma. Estas entrevistas permitirán recopilar las experiencias de los usuarios durante la interacción con el sistema, identificando posibles dificultades y oportunidades de mejora en los procesos de gestión comercial.

### Segmento 1: Dueños de Startups y Pymes

1. Al iniciar sesión en la plataforma, ¿qué tan rápido e intuitivo le resultó el proceso de autenticación?
2. Al ingresar al Dashboard principal, ¿considera que los indicadores y datos comerciales se presentan de manera clara y comprensible?
3. Al revisar el listado de leads y clientes, ¿le resultó sencillo identificar la información y el estado de las oportunidades de venta?
4. ¿Considera que la visualización del pipeline de ventas facilita la identificación de oportunidades pendientes, en proceso y concretadas?
5. Al consultar los reportes de ventas y ganancias, ¿la información presentada le resultó útil para evaluar el rendimiento comercial de su negocio?
6. ¿Le resultó sencillo navegar entre las diferentes secciones de la plataforma y encontrar las funcionalidades necesarias para supervisar las actividades comerciales?
7. En términos generales, ¿considera que NovaLeads le permitiría mejorar la organización de sus procesos comerciales y tomar decisiones de manera más rápida y efectiva?

### Segmento 2: Equipos de Ventas

1. Al iniciar sesión en la plataforma, ¿qué tan sencillo e intuitivo le resultó acceder a las funcionalidades disponibles para su rol?
2. Durante el registro de un nuevo lead, ¿le resultó fácil ingresar y guardar correctamente la información del potencial cliente?
3. Al consultar el listado de leads asignados, ¿considera que la información presentada le permite identificar rápidamente a los clientes que requieren atención?
4. Al actualizar el estado de una oportunidad dentro del pipeline de ventas, ¿le resultó sencillo comprender y realizar el proceso?
5. Al revisar el historial de conversaciones con un cliente, ¿considera que la información se encuentra organizada de manera clara y facilita la continuidad del seguimiento comercial?
6. ¿Le resultó sencillo identificar las oportunidades de venta pendientes y reconocer cuáles requieren un seguimiento prioritario?
7. En términos generales, ¿considera que el uso de NovaLeads agilizaría sus actividades diarias de seguimiento de clientes y gestión de oportunidades en comparación con las herramientas que utiliza actualmente?

## 5.3.2. Registro de Entrevistas

A continuación, se presenta el registro de las entrevistas de validación realizadas con usuarios de ambos segmentos objetivo interactuando en vivo con la plataforma NovaLeads, junto con sus respectivos enlaces alojados en Microsoft Stream.

### Segmento 1: Dueños de Startups y Pymes

#### Entrevista 1 – Segmento 1
- **Nombres y Apellidos:** Angie Moné Vásquez
- **Edad:** 31 años
- **Distrito:** Santiago de Surco, Lima
- **Fecha:** 13 de noviembre de 2026
- **Enlace del video:** [Ver video de la Entrevista 1](https://drive.google.com/file/d/1vijFBkCROYGYsBUbqvPtduEBpG0Al7Ne/view?usp=sharing) — Inicio: `00:00` | Duración: `05:20`
- **Evidencia visual:** ![Entrevista 1 - Segmento 1](Resources/Chapter5/entrevistas/1.png)
- **Resumen de la entrevista:** Angie Moné Vásquez (Gerente General) interactuó con NovaLeads y destacó que la propuesta de valor se comprende rápidamente gracias a las muestras visuales del tablero comercial y que tanto el formulario de registro como el acceso son breves y fluidos. Sin embargo, señaló oportunidades de mejora concretas en experiencia de usuario e internacionalización: indicó que la combinación de distintos matices en los fondos de las secciones puede cansar la vista tras jornadas largas, que los botones de *Registrarse* e *Iniciar sesión* tienen un diseño muy similar que puede generar confusión inicial, que la sección de soporte o preguntas frecuentes se encuentra muy abajo en el pie de página y que, al cambiar el idioma a español, aún permanecen algunos términos o etiquetas secundarias en inglés.

#### Entrevista 2 – Segmento 1
- **Nombres y Apellidos:** Flor Velázquez
- **Edad:** 29 años
- **Distrito:** Miraflores, Lima
- **Fecha:** 13 de noviembre de 2026
- **Enlace del video:** [Ver video de la Entrevista 2](https://drive.google.com/file/d/1i3FKSDKPjATFDNwPwGrUgVSYZbRqdpie/view?usp=sharing) — Inicio: `00:00` | Duración: `06:30`
- **Evidencia visual:** ![Entrevista 2 - Segmento 1](Resources/Chapter5/entrevistas/2.png)
- **Resumen de la entrevista:** Flor Velázquez (Directora Comercial en *Flora & Suelo*) evaluó la plataforma e indicó que la propuesta de valor se entiende desde el primer vistazo como una solución orientada a reemplazar hojas de cálculo tradicionales. Valoró positivamente la legibilidad de la tipografía, la fluidez de la navegación sin recargas bruscas y la estructura lógica de las secciones. Como oportunidades de mejora, sugirió ampliar la vista previa del sistema en la portada, otorgar un tono de acento más vivo a los botones principales e iconos para guiar mejor la mirada, añadir un enlace explícito para regresar al inicio desde el formulario de acceso (sin depender únicamente del logotipo), incorporar un icono para mostrar u ocultar la contraseña durante el registro y agregar textos descriptivos (*tooltips*) al pasar el cursor sobre los iconos decorativos.

#### Entrevista 3 – Segmento 1
- **Nombres y Apellidos:** Brenda More Vázquez
- **Edad:** 27 años
- **Distrito:** San Borja, Lima
- **Fecha:** 13 de noviembre de 2026
- **Enlace del video:** [Ver video de la Entrevista 3](https://drive.google.com/file/d/1J42g26O0tRrzP23BzxxzYP-5Dd8pCN4n/view?usp=sharing) — Inicio: `00:00` | Duración: `07:10`
- **Evidencia visual:** ![Entrevista 3 - Segmento 1](Resources/Chapter5/entrevistas/3.png)
- **Resumen de la entrevista:** Brenda More Vázquez (Fundadora de una startup) participó en la prueba interactiva completando el registro de cuenta, el inicio de sesión y la revisión del Dashboard y los leads. Señaló que la interfaz se percibe moderna y que el mensaje principal explica con claridad el propósito de ordenar ventas y clientes potenciales, aunque observó que el bloque inicial presenta demasiado texto concentrado. Como mejoras específicas, recomendó incrementar el contraste de los textos secundarios grises sobre tarjetas claras, mostrar de forma preventiva los requisitos de seguridad de la contraseña antes de enviar el formulario de registro, hacer más visible el selector de idioma (`ES / EN`) en la barra superior, redirigir el botón principal directamente al registro y añadir un botón rápido de retorno al inicio en la parte inferior.
### Segmento 2: Equipos de Ventas


#### Entrevista 1 – Segmento 2
- **Nombres y Apellidos:** Sebastián Herrera
- **Edad:** 24 años
- **Distrito:** Surquillo
- **Fecha:** 13 de noviembre de 2026
- **Enlace del video:** [Ver video de la Entrevista 4](https://drive.google.com/file/d/1ln4vHPm9JEiD3Evv5d1MgPGwO8RPYmJ2/view?usp=drive_link) — Inicio: `00:00` | Duración: `02:43`
- **Evidencia visual:** ![Entrevista 4 - Segmento 2](Resources/Chapter5/entrevistas/4.png)
- **Resumen de la entrevista:** Sebastián evaluó su experiencia de uso de NovaLeads e indicó que el inicio de sesión fue rápido y que encontró fácilmente las opciones necesarias para trabajar. Señaló que el registro de leads fue fácil de entender, con campos bien organizados que permitieron ingresar la información sin complicaciones. Asimismo, manifestó que la organización de los datos de los clientes ayuda a identificar con quién debe comunicarse. Respecto al pipeline de ventas, consideró intuitivo identificar las etapas y actualizar el estado de las oportunidades. También valoró la utilidad del historial de conversaciones para recordar lo tratado con cada cliente antes de volver a contactarlo. Como oportunidad de mejora, propuso destacar más las oportunidades que necesitan atención urgente. Finalmente, expresó que centralizar la información de clientes y ventas en un solo lugar facilitaría el trabajo y ayudaría a ahorrar tiempo.


#### Entrevista 2 – Segmento 2
- **Nombres y Apellidos:** Giuseppe Chavez.
- **Edad:** 19 años.
- **Distrito:** Comas.
- **Fecha:** 12 de noviembre de 2026.
- **Perfil:** Estudiante y emprendedor encargado de atender consultas, contactar a potenciales clientes y realizar seguimiento de ventas.
- **Entrevistador:** Lui Mathias Gamero Miranda.
- **Enlace del video (Google Drive):** [Ver video de la Entrevista 5](https://drive.google.com/file/d/1WSy_STwC9aSqxFdmnXYCMDD_3-cUkKkh/view?usp=sharing) — Inicio: `00:00` | Duración: `04:23`.
- **Evidencia visual:** ![Entrevista 5 - Segmento 2: Giuseppe Chavez y Lui Mathias Gamero Miranda durante la sesión de validación](Resources/Chapter5/entrevistas/5.png)
- **Resumen de la entrevista:** Giuseppe describió su experiencia de uso de NovaLeads desde sus actividades de atención comercial y seguimiento de clientes, que actualmente organiza con Excel y WhatsApp. Manifestó que el menú y los nombres de las secciones le permitieron ubicar las funcionalidades con pocas indicaciones, y valoró la claridad de los campos y la centralización de los datos de los contactos. Asimismo, consideró comprensibles las etapas del pipeline y útil consultar el historial de conversaciones junto con la información de cada cliente para retomar el seguimiento con mayor contexto. Respecto a la priorización, explicó que también necesita considerar la situación de cada oportunidad, la última conversación, el tiempo de espera y los compromisos pendientes, como el envío de una cotización. Finalmente, señaló que la plataforma podría ayudarle a organizar la información y reducir el tiempo de búsqueda, aunque manifestó su interés en utilizarla durante varios días con sus actividades habituales para valorar mejor su utilidad. Estas apreciaciones corresponden a lo declarado por el participante; la grabación muestra una presentación compartida del dashboard y no documenta paso a paso la ejecución autónoma de todos los flujos mencionados.

#### Entrevista 3 – Segmento 2
- **Nombres y Apellidos:** `[Nombre y Apellido Entrevistado 3 - Seg. 2]`
- **Edad:** 26 años
- **Distrito:** Magdalena del Mar, Lima
- **Fecha:** 13 de noviembre de 2026
- **Enlace del video (Microsoft Stream):** `[PEGAR_LINK_STREAM_S2_E3]` — Inicio: `00:00` | Duración: `[04:15]`
- **Evidencia visual:** `![Entrevista 3 - Segmento 2](ruta/captura_s2_entrevista_3.png)`
- **Resumen de la entrevista:** El entrevistado recorrió los flujos diarios de trabajo entre Dashboard, *Leads*, *Pipeline* y *Conversaciones*, destacando la fluidez de la interfaz y la utilidad del buscador superior para ubicar clientes específicos. Concluyó que NovaLeads agiliza significativamente el seguimiento comercial frente a herramientas tradicionales, recomendando añadir alertas visuales para oportunidades pendientes sin actividad reciente.

## 5.3.3. Evaluaciones según heurísticas

La evaluación heurística de NovaLeads tiene como finalidad identificar dificultades de interacción y oportunidades de mejora en la experiencia de los usuarios. Se consideran principios de **usabilidad, arquitectura de información y diseño inclusivo**.

La evaluación se desarrolla mediante una autoauditoría del equipo NovaScale, autorizada por el docente. Esta versión preliminar utiliza las observaciones documentadas en las entrevistas de Angie Moné Vásquez, Flor Velázquez y Brenda More Vázquez, pertenecientes al segmento de dueños de startups y pymes.

**Estado de la evaluación:** los hallazgos se extraen de los resúmenes publicados en la sección 5.3.2 y las severidades son propuestas iniciales. Deben contrastarse con la aplicación e incorporar las capturas y los minutos correspondientes antes de cerrar la evaluación.

### Datos generales

| Campo | Información |
| :--- | :--- |
| **CARRERA** | Ingeniería de Software |
| **CURSO** | Aplicaciones Web |
| **SECCIÓN** | 8074 |
| **PROFESOR** | Alex Humberto Sánchez Ponce |
| **EQUIPO AUDITOR** | NovaScale |
| **RESPONSABLE** | Sergio Rubén Caldas García |
| **PARTICIPANTES CONSIDERADAS** | Angie Moné Vásquez, Flor Velázquez y Brenda More Vázquez |
| **PRODUCTO EVALUADO** | NovaLeads |
| **ACCESO A LA APLICACIÓN** | https://novaleads.onrender.com/login |
| **FECHA DE LAS ENTREVISTAS** | 13 de noviembre de 2026 |

### Alcance de la evaluación

Esta revisión preliminar comprende las observaciones sobre las siguientes tareas:

1. Comprender la propuesta de valor de NovaLeads.
2. Identificar las opciones de registro e inicio de sesión.
3. Crear una cuenta e introducir una contraseña.
4. Navegar entre las pantallas de acceso y la página principal.
5. Cambiar el idioma de la interfaz.
6. Interpretar los textos e indicadores de las pantallas consultadas.
7. Localizar información de soporte y preguntas frecuentes.

La incorporación de los flujos específicos de vendedores y la revisión en dispositivos móviles se realizará conforme se disponga de sus evidencias.

No se incluyen pruebas de seguridad del backend, rendimiento de la infraestructura ni integraciones externas.

### Escala de severidad

| Nivel | Descripción |
| :--- | :--- |
| **1 - Superficial** | Dificultad de impacto limitado, fácilmente superable por el usuario. Su corrección puede realizarse cuando exista disponibilidad. |
| **2 - Menor** | Dificulta la interacción, aunque permite continuar con la tarea. Se recomienda corregirla en una siguiente versión. |
| **3 - Mayor** | Afecta considerablemente una tarea o resulta difícil de superar. Requiere prioridad alta. |
| **4 - Muy grave** | Impide continuar una tarea esencial. Su corrección es necesaria antes del lanzamiento. |

### Referencias de las entrevistas

| Código | Participante | Referencia |
| :--- | :--- | :--- |
| **E01** | Angie Moné Vásquez | Entrevista 1 del segmento de dueños, sección 5.3.2. |
| **E02** | Flor Velázquez | Entrevista 2 del segmento de dueños, sección 5.3.2. |
| **E03** | Brenda More Vázquez | Entrevista 3 del segmento de dueños, sección 5.3.2. |

### Tabla resumen de hallazgos preliminares

| N.º | Problema reportado | Severidad propuesta | Heurística o principio afectado | Fuente |
| :--- | :--- | :---: | :--- | :--- |
| **P01** | Permanencia de términos en inglés después de seleccionar español. | **2** | Diseño inclusivo: proporcionar experiencias comparables. | E01 |
| **P02** | Dificultad de lectura de textos secundarios grises sobre fondos claros. | **2** | Diseño inclusivo: proporcionar experiencias comparables. | E03 |
| **P03** | Requisitos de contraseña poco visibles antes de enviar el registro. | **2** | Usabilidad: prevención de errores. | E03 |
| **P04** | Retorno a la página principal poco explícito desde el acceso. | **2** | Usabilidad: control y libertad del usuario. | E02, E03 |
| **P05** | Diferenciación visual insuficiente entre registro e inicio de sesión. | **2** | Usabilidad: reconocimiento antes que recuerdo. | E01 |
| **P06** | Baja visibilidad del acceso a soporte y preguntas frecuentes. | **2** | Arquitectura de información: facilidad para encontrar información. | E01 |

### Detalle de hallazgos

#### PROBLEMA P01: Traducción incompleta al seleccionar español

**Severidad propuesta:** 2 - Menor.<br>
**Principio afectado:** Diseño inclusivo - proporcionar experiencias comparables.<br>
**Fuente:** E01 - Angie Moné Vásquez.

**Problema:** El resumen de la entrevista indica que algunas etiquetas secundarias permanecen en inglés después de seleccionar español. Esta combinación puede dificultar la comprensión de personas que esperan utilizar toda la interfaz en el idioma seleccionado.

**Justificación:** La observación sugiere un esfuerzo adicional de interpretación, sin documentar un bloqueo completo de la tarea.

**Recomendación:** Revisar los textos visibles de cada pantalla y completar sus traducciones. Comprobar que el idioma seleccionado se mantenga durante la navegación.

**Evidencia que se incorporará:** Captura con español seleccionado y los términos sin traducir, junto con el minuto de la observación.

#### PROBLEMA P02: Legibilidad reducida de textos secundarios

**Severidad propuesta:** 2 - Menor.<br>
**Principio afectado:** Diseño inclusivo - proporcionar experiencias comparables.<br>
**Fuente:** E03 - Brenda More Vázquez.

**Problema:** La participante recomendó incrementar el contraste de los textos secundarios grises sobre tarjetas claras. Esta observación señala una posible dificultad para leer información complementaria de las pantallas.

**Justificación:** Se propone severidad menor por el esfuerzo de lectura reportado. Todavía debe medirse el contraste para determinar si existe un incumplimiento técnico.

**Recomendación:** Medir los colores de texto y fondo y ajustar los pares que no alcancen el contraste aplicable. Comprobar también los estados interactivos.

**Evidencia que se incorporará:** Captura del texto afectado, colores utilizados y relación de contraste obtenida.

#### PROBLEMA P03: Requisitos de contraseña poco visibles durante el registro

**Severidad propuesta:** 2 - Menor.<br>
**Heurística afectada:** Usabilidad - prevención de errores.<br>
**Fuente:** E03 - Brenda More Vázquez.

**Problema:** La participante solicitó que las condiciones de seguridad de la contraseña se presenten antes de enviar el formulario. La falta de orientación previa puede provocar intentos de registro que requieran corrección.

**Justificación:** El usuario podría continuar después de corregir los datos, pero realizaría un esfuerzo evitable.

**Recomendación:** Mostrar las condiciones junto al campo de contraseña e indicar claramente cuáles se cumplen. Los mensajes deben explicar cómo corregir una entrada inválida.

**Evidencia que se incorporará:** Capturas del formulario antes del envío y de la respuesta ante una contraseña que incumpla sus condiciones.

#### PROBLEMA P04: Retorno poco explícito a la página principal

**Severidad propuesta:** 2 - Menor.<br>
**Heurística afectada:** Usabilidad - control y libertad del usuario.<br>
**Fuentes:** E02 - Flor Velázquez; E03 - Brenda More Vázquez.

**Problema:** Las participantes recomendaron incluir un acceso explícito para regresar al inicio. El resumen de E02 indica que actualmente se depende del logotipo como opción de retorno, cuyo comportamiento puede resultar poco evidente para usuarios nuevos.

**Justificación:** La dificultad afecta la identificación de la salida del flujo, aunque no demuestra que el retorno sea imposible.

**Recomendación:** Incorporar un enlace visible y comprensible, como "Volver al inicio", y comprobar su funcionamiento.

**Evidencia que se incorporará:** Captura de la pantalla afectada y referencia al momento en que se observa o comenta la dificultad.

#### PROBLEMA P05: Diferenciación insuficiente entre registro e inicio de sesión

**Severidad propuesta:** 2 - Menor.<br>
**Heurística afectada:** Usabilidad - reconocimiento antes que recuerdo.<br>
**Fuente:** E01 - Angie Moné Vásquez.

**Problema:** La participante señaló que los controles de registro e inicio de sesión presentan una apariencia similar que puede generar confusión inicial. Esto puede dificultar reconocer la acción correspondiente a una persona nueva o a una que ya tiene cuenta.

**Justificación:** La observación afecta la elección inicial, sin documentar una imposibilidad de acceder.

**Recomendación:** Revisar la jerarquía de las acciones, conservar etiquetas claras y comprobar con usuarios que ambas opciones se distingan con facilidad.

**Evidencia que se incorporará:** Captura de ambos controles en su contexto y minuto de la observación.

#### PROBLEMA P06: Acceso poco visible a soporte y preguntas frecuentes

**Severidad propuesta:** 2 - Menor.<br>
**Principio afectado:** Arquitectura de información - facilidad para encontrar información.<br>
**Fuente:** E01 - Angie Moné Vásquez.

**Problema:** La participante indicó que la información de soporte y preguntas frecuentes se encuentra muy abajo, en el pie de página. Esto puede aumentar el esfuerzo necesario para localizar ayuda durante la navegación.

**Justificación:** Se propone severidad menor porque la información estaría disponible, aunque su localización podría resultar difícil.

**Recomendación:** Evaluar un acceso adicional a ayuda desde la navegación principal o desde los formularios donde resulte pertinente, conservando etiquetas consistentes.

**Evidencia que se incorporará:** Captura de la ubicación actual y registro del recorrido necesario para encontrar la ayuda.

### Síntesis preliminar

Las observaciones documentadas permiten orientar la revisión hacia la comprensión del idioma, la legibilidad, la prevención de errores y la facilidad de navegación. Las severidades propuestas deberán confirmarse considerando el impacto observado y la posibilidad de completar las tareas.

La evaluación se completará contrastando estos hallazgos con la aplicación, incorporando sus evidencias y añadiendo las observaciones verificables del segmento de vendedores.

---

# Conclusiones

## Conclusiones y recomendaciones

### Conclusiones

1. **Validación del Problem Statement y propuesta de valor:** A partir de las entrevistas de validación realizadas con representantes de startups, pymes y equipos de ventas interactuando con NovaLeads, se confirma que la plataforma resuelve de manera efectiva la desorganización comercial derivada del uso de hojas de cálculo tradicionales. La centralización de leads, el pipeline visual por etapas y los indicadores clave en tiempo real permiten supervisar el estado del negocio con rapidez.
2. **Contrastación de Assumptions e Hypothesis Statements (Lean UX):** Se validaron las hipótesis principales planteadas en el proceso Lean UX respecto a la facilidad de adopción del sistema. Los usuarios completaron los flujos principales —registro de cuenta, autenticación, creación de leads y actualización de etapas en el pipeline— sin requerir capacitación previa, confirmando que una interfaz limpia y consistente agiliza la operación diaria.
3. **Implementación de Arquitectura y Despliegue Continuo:** Se consolidó el desarrollo modular bajo *Domain-Driven Design (DDD)* integrando el Landing Page, la *Frontend Web Application* (`novascale-webapp`) en **Vue.js** y **PrimeVue**, y los *Backend Web Services* (`novascale-platform`) en **ASP.NET Core (C#)**, respaldados por **GitFlow**, *Conventional Commits* y flujos automatizados de despliegue.

### Recomendaciones

1. **Mejoras de usabilidad, contraste e internacionalización (Corto plazo):** Implementar los ajustes identificados en la evaluación heurística (Sección 5.3.3), priorizando el incremento de contraste en textos secundarios, la traducción completa de etiquetas secundarias al español, la validación preventiva en tiempo real junto con el botón de visualización de contraseña en el registro, la diferenciación visual entre los botones de acceso y la adición de descripciones emergentes (*tooltips*) en iconos e indicadores.
2. **Evolución funcional y rigor técnico (Mediano plazo):** Incorporar recordatorios automáticos para oportunidades pendientes en el pipeline sin seguimiento reciente, filtros avanzados por fecha en el listado de leads y exportación directa de reportes comerciales, manteniendo las convenciones de nomenclatura en inglés y la revisión por *Pull Requests*.
3. **Integración omnicanal (Largo plazo):** Ampliar el módulo de *Conversaciones* mediante la integración directa con canales de mensajería empresarial (como WhatsApp Business API, Facebook, Instagram y correo electrónico) para centralizar automáticamente todas las interacciones con los clientes dentro de la plataforma.
# Anexos

A continuación, se detallan los enlaces de acceso a la plataforma de gestión ágil de tareas y a los repositorios oficiales de control de versiones en la organización de GitHub del equipo **NovaScale**:

* **Gestión de Proyecto y Product Backlog (Jira Software):** [Tablero Scrum - NovaLeads](https://johanbottger.atlassian.net/jira/software/projects/SCRUM/boards/1/backlog?atlOrigin=eyJpIjoiZGFhNGMxZDBiNWNkNGU1NTlmOTBjMmY3YjZhODZiZmQiLCJwIjoiaiJ9)
* **Organización Oficial en GitHub:** [202620-1asi0730-8074-novascale](https://github.com/202620-1asi0730-8074-novascale)
* **Web application:** https://novaleads.onrender.com/
# Bibliografía

A continuación, se detallan las referencias en formato **APA 7.ª edición** correspondientes a los marcos de trabajo, guías oficiales del curso, herramientas de software y recursos de competidores (nombres y logotipos usados con fines académicos) empleados en el proyecto:

* Conventional Commits. (s.f.). *Conventional Commits 1.0.0*. https://www.conventionalcommits.org/
* GitHub, Inc. (2026). *GitHub* [Plataforma de desarrollo colaborativo y control de versiones]. https://github.com/
* HubSpot, Inc. (2026). *HubSpot CRM* [Marca registrada y logotipo]. https://www.hubspot.com/
* JetBrains s.r.o. (2026). *WebStorm* [Entorno de desarrollo integrado]. https://www.jetbrains.com/webstorm/
* Pipedrive Inc. (2026). *Pipedrive* [Marca registrada y logotipo]. https://www.pipedrive.com/
* Typicode. (2026). *JSON Server* [Biblioteca de simulación de REST API]. GitHub. https://github.com/typicode/json-server
* Vue.js. (s.f.). *Vue Style Guide*. https://vuejs.org/v2/style-guide/
* Zoho Corporation Pvt. Ltd. (2026). *Zoho CRM* [Marca registrada y logotipo]. https://www.zoho.com/crm/
