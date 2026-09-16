# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management


### 5.1.1. Software Development Environment Configuration


### 5.1.2. Source Code Management

### 5.1.3. Source Code Style Guide & Conventions



### 5.1.4. Software Deployment Configuration


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
| **Sprint 1 Velocity** | 20 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos). |
| **Sum of Story Points** | 20 Story Points. |

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
| US-21 | Visualización de información del negocio | T-01 | Diseñar estructura de la Landing Page | Definir la estructura visual de las secciones principales de la Landing Page y organizar la información de NovaLeads. | 3 | Lui | To Do |
| US-21 | Visualización de información del negocio | T-02 | Implementar sección principal | Implementar la sección inicial con el nombre, propuesta de valor y descripción general de NovaLeads. | 3 | Lui | To Do |
| US-21 | Visualización de información del negocio | T-03 | Implementar sección de funcionalidades | Implementar una sección que presente las principales funcionalidades de NovaLeads de forma clara y visual. | 4 | Lui | To Do |
| US-22 | Información para dueños de pymes y startups | T-04 | Diseñar sección para dueños | Diseñar la sección dirigida a dueños de pymes y startups, destacando los beneficios relacionados con la gestión comercial. | 3 | Dario | To Do |
| US-22 | Información para dueños de pymes y startups | T-05 | Implementar contenido para dueños | Implementar textos y elementos visuales relacionados con la gestión de leads, clientes, conversaciones y resultados de ventas. | 3 | Dario | To Do |
| US-23 | Información para equipos de ventas | T-06 | Diseñar sección para equipos de ventas | Diseñar la sección dirigida a equipos de ventas, considerando sus principales necesidades de gestión y seguimiento comercial. | 3 | Johan | To Do |
| US-23 | Información para equipos de ventas | T-07 | Implementar contenido para equipos de ventas | Implementar textos y elementos visuales relacionados con leads, conversaciones y rendimiento del equipo. | 3 | Johan | To Do |
| US-24 | Navegación entre secciones | T-08 | Implementar menú de navegación | Crear el menú de navegación de la Landing Page con enlaces hacia las principales secciones del sitio. | 3 | Sergio | To Do |
| US-24 | Navegación entre secciones | T-09 | Implementar navegación interna | Configurar el desplazamiento hacia las secciones correspondientes al seleccionar las opciones del menú. | 2 | Sergio | To Do |
| US-25 | Call to Action para dueños | T-10 | Diseñar Call to Action para dueños | Diseñar un Call to Action dirigido específicamente a dueños de pymes y startups. | 2 | Renzo | To Do |
| US-25 | Call to Action para dueños | T-11 | Implementar flujo del Call to Action | Implementar el enlace o acción que permita al visitante iniciar el flujo de acceso o registro correspondiente. | 2 | Renzo | To Do |
| US-26 | Call to Action para equipos de ventas | T-12 | Diseñar Call to Action para equipos de ventas | Diseñar un Call to Action dirigido específicamente a equipos de ventas. | 2 | Lui | To Do |
| US-26 | Call to Action para equipos de ventas | T-13 | Implementar flujo del Call to Action | Implementar el enlace o acción que permita al visitante iniciar el flujo de acceso o registro correspondiente. | 2 | Lui | To Do |
| US-27 | Visualización responsive | T-14 | Adaptar Landing Page a dispositivos | Adaptar la estructura y componentes de la Landing Page para desktop, tablet y dispositivos móviles. | 5 | Johan | To Do |
| US-27 | Visualización responsive | T-15 | Validar comportamiento responsive | Verificar la correcta visualización de textos, imágenes, navegación y Call to Action en diferentes tamaños de pantalla. | 3 | Johan | To Do |

#### 5.2.1.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 1 fue el desarrollo de la Landing Page institucional del producto. 
A continuación, se presentan los commits más importantes del Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo del Landing Page.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| novaleads-website | develop |  | feat: Landing Page development | - | 12-05-2026 |

#### 5.2.1.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución de la Landing Page de la aplicación como evidencia. La Landing Page es compuesta por varias secciones que se presentan en las capturas a continuación.

<img src="/Resources/Chapter5/sprint1/execution-evidence1.png"/>
<img src="/Resources/Chapter5/sprint1/execution-evidence2.png"/>
<img src="/Resources/Chapter5/sprint1/execution-evidence3.png"/>

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
No aplica a primer sprint y desarrollo de Landing Page.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.
El despliegue de la Landing Page se realizó en el servicio de Github Pages, se seleccionó esta alternativa debido a la rapidez de despliegue y su sencillez, apropiada para una página estática.
Se incluye la evidencia de despliegue del Landing Page en la plataforma Github Pages: 

#### 5.2.1.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 1:
