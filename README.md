
# Capítulo IV: Product Design

Este capítulo guiará el proceso de diseño a través de lineamientos claros de estilo, arquitectura de información, navegación y diseño de interfaces.

---

## 4.1. Style Guidelines.
Un Style Guideline es un conjunto de reglas y normas que definen cómo se debe redactar, diseñar o presentar documentos, contenido web, software u otros trabajos creativos. A continuación se describen las directrices que aseguran la uniformidad estética del proyecto.<br>

### 4.1.1. General Style Guidelines.

#### Branding
Para la creación de la identidad visual de **NovaLeads** se optó por un diseño moderno y profesional que transmita eficiencia, transparencia, limpieza visual y organización.
El logotipo simboliza el orden y priorización de elementos que ofrece el sistema.

![Logo](/Resources/Chapter4/style/logo.jpg)

#### Typography
Se ha elegido una tipografía **Montserrat** variable, moderna y legible en dispositivos móviles y web. Además ofrece el beneficio de fuentes bold, light y medium.
- **Títulos y encabezados**: peso **bold**, transmitiendo fuerza y claridad.  
- **Cuerpo de texto**: peso **regular**, con interlineado amplio que favorece la lectura.

![Typography](/Resources/Chapter4/Resources/typography.png)

El estilo general busca mantener una comunicación **clara, directa y confiable** para los dos públicos objetivos.


#### Colors

La paleta escogida utiliza 4 colores en forma de semáforo para representar niveles de priorización en nuestro sistema. Junto a ellos se utilizan 2 colores neutros para textos y sombras, y un color cercano al blanco para fondos.

![Colors](/Resources/Chapter4/style/colors.png)

#### Spacing

Las reglas de espaciado visual de la interfaz: márgenes, paddings, separación entre elementos, secciones, textos, botones, etc. utilizan un sistema de espaciado consistente basado en múltiplos de 4 px.

- 4 px: separación mínima entre elementos relacionados, como iconos y texto.
- 8 px: separación entre elementos dentro de un mismo componente.
- 16 px: separación estándar entre elementos de una sección.
- 24 px: separación entre grupos de contenido relacionados.
- 32 px: separación entre bloques o componentes principales.

#### Dimensiones de comunicación y Lenguaje

La comunicación de NovaLead principia en ser clara, directa y profesional, evitando términos técnicos innecesarios. 

- Evitar mensajes ambiguos que no indiquen claramente qué ocurrirá al realizar una acción.
- Mantener la terminología consistente: utilizar siempre “lead”, “cliente”, “vendedor”, “conversación” y “dashboard” para referirse a los mismos conceptos.
- Mantener una comunicación consistente en toda la plataforma.

---

### 4.1.2. Web Style Guidelines.

El estándar visual contribuye a la consistencia a través del sistema. A continuación se detalals decisiones en la interacción de la interfaz.

- **Componentes e interacción**
Botones, formularios, cards, navegación y etiquetas.
Estados de los componentes: normal, hover, activo y deshabilitado.
Feedback visual ante las acciones del usuario.
- **Responsive Design**
Comportamiento de la interfaz en desktop, tablet y mobile.
Adaptación de grids, navegación, imágenes y componentes.
Priorización del contenido según el tamaño de pantalla.


## 4.2. Information Architecture.
La Arquitectura de Información define la estructura y organización de los contenidos y funcionalidades que conforman NovaLeads. Su objetivo es establecer una distribución clara y coherente de la información, facilitando que los usuarios puedan encontrar, comprender y utilizar las funcionalidades de la plataforma de acuerdo con sus necesidades.

### 4.2.1. Organization Systems.

#### Organizacción Jerárquica de Contenido
La organización jerárquica se utiliza para establecer diferentes niveles de importancia entre los contenidos. En NovaLeads se aplica principalmente en el Dashboard y en la Landing Page. En el Dashboard, los indicadores principales se presentan antes que la información secundaria, permitiendo que el usuario identifique rápidamente los datos más relevantes. En la Landing Page, la propuesta de valor, los beneficios principales y los Call to Action reciben mayor jerarquía visual que la información complementaria.

#### Organización Secuencial
 
La organización secuencial corresponde a las acciones que toma un usuario en serie dentro de un orden predeterminado. En el sistema se aplica principalmente en procesos como el inicio y registro de sesión, y el registro de información nueva como nuevos contactos.

#### Organización Cronológica

El esquema cronológico se utiliza en el historial de conversaciones con contactos, está directamente ligado a el sistema de prioridad. 


---

### 4.2.2. Labeling Systems.

Las principales etiquetas consistentes a través del sistema son las siguientes:

- Dashboard : Indicadores y métricas
- Leads : Contactos registrados como clientes potenciales
- Contacto : Personas registradas con la empresa
- Cliente : Contacto con relación comercial (previamente lead)
- Conversaciones : Comunicación con contacto
- Etiquetas : Marcadores de contactos
- Perfil : Información de Usuario
- Ventas : Resultado comercial
- Mensaje : Mensaje de texto en conversación
- Estado : Activo, Hot, Perdido, Sin respuesta



---

### 4.2.3. SEO Tags and Meta Tags.

El objetivo es que NovaLeads resalta en motores de búsqueda sobre otros sistemas CRM.

### **Landing Page**
* **Título:** `<title>NovaLeads | Gestor de relación con clientes</title>`
* **Descripción:** `<meta name="description" content="CRM organiza tu negocio en un solo lugar. Ventas, servicio al cliente, comunicación directa."/>`
* **Keywords:** `<meta name="keywords" content="Ventas, CRM, Leads, Clientes, Servicio al cliente."/>`
* **Autor:** `<meta name="author" content="NovaScale" />`

### **Web Application**
* **Título:** `<title>Dash Board Novaleads</title>`
* **Descripción:** `<meta name="description" content="Panel de administración "/>`

---

### 4.2.4. Searching Systems.
No queremos que el usuario "busque", queremos que "encuentre" rápido:

* **Búsqueda Predictiva:** A medida que el administrador escribe (ej. un DNI o nombre), el sistema sugiere usuarios registrados para ahorrar tiempo.
* **Filtros:** La bandeja de conversaciones permite sleccionar únicamente aquellas que cumplan criterios de prioridad, antiguedad, estado.


---
### 4.2.5. Navigation Systems.


* **Menú Lateral:** Prioriza el espacio de trabajo central a las secciones de la aplicación, manteniendo los módulos principales a un solo clic.
* **Acciones Contextuales** El sistema ofrece información y acciones a medida que sean relevantes, disminuyendo el ruido visual.



## 4.3. Landing Page UI Design.


### 4.3.1. Landing Page Wireframe.
El wireframe de baja fidelidad define la estructura visual y la jerarquía de la información. Se ha priorizado una navegación intuitiva, destacando las funcionalidades principales.

![Landing Page Wireframe](/Resources/Chapter4/LandingPage/Wireframe%20Landing%20Page.png)

* **Elementos clave:** 

### 4.3.2. Landing Page Mock-up.
El mock-up de alta fidelidad integra la identidad visual de la marca, incluyendo la paleta de colores, tipografía y elementos gráficos finales. Este diseño representa la apariencia exacta que tendrá la aplicación web una vez implementada.

![Landing Page Mock-up](/Resources/Chapter4/Resources/landingpage-mock.png)


## 4.4. Web Applications UX/UI Design.


### 4.4.1. Web Applications Wireframes.






### 4.4.2. Web Applications Wireflow Diagrams.


User goals

### 4.4.3. Web Applications Mock-ups.
Esta sección presenta los mock-ups de alta fidelidad de la plataforma web de SmartLock. Estos diseños representan la apariencia visual final del sistema, incluyendo identidad visual, paleta de colores, tipografía, distribución de componentes y experiencia de usuario orientada a la implementación real del producto.

### 1. Inicio de Sesión (Login)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/InicioSesión-Mockup.png" width="800" alt="Login Mockup">
</p>

**Descripción:** Pantalla de acceso seguro al sistema principal.

### 2. Registro de Usuario (Sign Up)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/RegistroSesión-Mockup.png" width="800" alt="Registro Mockup">
</p>

**Descripción:** Formulario rápido para crear una cuenta nueva.

### 3. Autenticación de Dos Factores (2FA)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/Autenticacion2FA-mockup.png" width="800" alt="2FA Mockup">
</p>

**Descripción:** Capa extra de seguridad con código móvil.

### 4. Creación de Organización

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/crear-organizacion-mockup.png" width="800" alt="Creación de Organización Mockup">
</p>

**Descripción:** Paso inicial para registrar tu nueva organización.

### 5. Selección Plan de Suscripción

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/seleccionar-plan-mockup.png" width="800" alt="Plan de Suscripción Mockup">
</p>

**Descripción:** Pantalla de selección de plan de suscripción.

### 6. Configuración Organización

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/form-organizacion-mockup.png" width="800" alt="Configuración Organización Mockup">
</p>

**Descripción:** Ajustes detallados de la organización activa.

### 7. Confirmación de creación de organización

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/confirm-plan-mockup.png" width="800" alt="Confirmación Organización Mockup">
</p>

**Descripción:** Mensaje de éxito al registrar la organización.

### 8. Crear Sedes

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/crear-sede-Mockup.png" width="800" alt="Configuración de Sedes Mockup">
</p>

**Descripción:** Interfaz para añadir una nueva ubicación física.

### 9. Configuración de Sedes

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/crear-sede-info-Mockup.png" width="800" alt="Configuración de Sedes Mockup">
</p>

**Descripción:** Ajuste de parámetros para cada sede creada.

### 10. Panel de Control

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/panel-control-Mockup.png" width="800" alt="Panel de Control Mockup">
</p>

**Descripción:** Vista general del estado de las sedes.

### 11. Bitácora de accesos

<p align="center">
  <img src="Resources/Chapter4/Web-Application/mockups/Dashboard-bitacora-Mockup.png" width="800" alt="Bitácora Mockup">
</p>

**Descripción:** Registro detallado del historial de los accesos.

### 12. Control de Entidades (Accesos)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-accesos-mockup.png" width="800" alt="Accesos Mockup">
</p>

**Descripción:** Directorio completo de usuarios con acceso permitido.

### 13. Control de Entidades (Personas)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-personas-mockup.png" width="800" alt="Personas Mockup">
</p>

**Descripción:** Asignación de roles y permisos por usuario.

### 14. Control de Entidades (Grupos)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-grupos-mockup.png" width="800" alt="Grupos Mockup">
</p>

**Descripción:** Interfaz para la gestión de grupos operativos.

### 15. Control de Entidades (Administradores)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-admins-mockup.png" width="800" alt="Administradores Mockup">
</p>

**Descripción:** Asignación de permisos a administradores del sistema.

### 16. Control de Entidades (Añadir Accesos)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-añadir-accesos-mockup.png" width="800" alt="Añadir Accesos Mockup">
</p>

**Descripción:** Formulario para registrar nuevos permisos de entrada.

### 17. Control de Entidades (Añadir Personas)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-añadir-personas-mockup.png" width="800" alt="Añadir Personas Mockup">
</p>

**Descripción:** Registro de nuevos integrantes a la plataforma.

### 18. Control de Entidades (Añadir Grupos)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-añadir-grupo-mockup.png" width="800" alt="Añadir Grupos Mockup">
</p>

**Descripción:** Creación de nuevos grupos de trabajo específicos.

### 19. Control de Entidades (Añadir Administradores)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/ControlEntidades-admins-añadir-mockup.png" width="800" alt="Añadir Administradores Mockup">
</p>

**Descripción:** Alta de nuevos perfiles con privilegios administrativos.

### 20. Confirmación de Cierre de Sesión

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/mockups/CerrarSesion-mockup.png" width="800" alt="Logout Mockup">
</p>

**Descripción:** Ventana segura para salir de la plataforma.

### 4.4.4. Web Applications User Flow Diagrams.
En la siguiente sección se puede observar de manera detallada el  diagrama Userflow.

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/userflow/userflow.png" width="800" alt="userflow">
</p>

## 4.5. Web Applications Prototyping.


<p align="center">
  <img src="../Resources/Chapter4/Web-Application/figma prototype.jpg" width="900">
</p>

<br>

**Link del Figma:**  
[Ver enlace](https://www.figma.com/design/kVDoKtb6qnhzGb0kD1rCyR/Untitled?node-id=0-1&t=ZrgcAyr2GfzBtvf7-1)

<br>

**Link del video de explicación:**  
[Ver enlace](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a860_upc_edu_pe/IQAoeufOBXR1Q4_QgHSUq5ZoAdnsC9hr3FJfDiVG26U60XM?e=5zpImg&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

<br>

<p align="center">
  <img src="../Resources/Chapter4/Web-Application/Captura Prototype evidencia.jpg" width="900">
</p>

## 4.6. Domain-Driven Software Architecture.
En esta sección se detalla el diseño táctico del sistema, profundizando en la arquitectura y los componentes técnicos necesarios para implementar la solución. A diferencia del Big Picture, el DesignLevel Event Storming se enfoca en definir los límites de los agregados, los comandos que disparan cambios de estado y las políticas que gobiernan las reglas de negocio.

<p align="center">
  <img src="Resources/Evidencias/total-ddd.png" width="800" alt="Design Level Event Storming">
</p>

### 1. Space Management (Gestión de Espacios)
Es el contexto central encargado de la infraestructura física y lógica de la plataforma. Su responsabilidad principal es modelar la jerarquía operativa, gestionando entidades como **Organizations**, **Sites** (sedes) y **Zones**. Este contexto administra la relación entre los activos físicos y su ubicación, permitiendo que la plataforma identifique la posición de los dispositivos de bloqueo digital.
<img src="Resources/Evidencias/space-management.png">

### 2. Access (Control de Acceso)
Este contexto se enfoca estrictamente en la autorización y la seguridad física. Gestiona las identidades mediante la entidad **Subject** y su agrupación en **Groups** para facilitar la asignación masiva de permisos. Su lógica de negocio define quién tiene permitido ingresar a áreas específicas basándose en la validación de tokens y reglas de seguridad configuradas.
<img src="Resources/Chapter4/eventStormin/Acces-Context.png">

### 3. IAM (Autenticación e Identidad)
Responsable de la seguridad a nivel de software y la validación de la identidad del usuario en el sistema. Administra las **Accounts**, los hashes de contraseñas y los roles de usuario. Asegura que el usuario sea quien dice ser antes de permitirle interactuar con la interfaz del frontend o las APIs de la aplicación.
<img src="Resources/Evidencias/access.png">

### 4. Report (Reportes y Auditoría)
Dedicado a la observabilidad y la persistencia de eventos históricos dentro del ecosistema SmartLock. Utiliza entidades como **Audit**, **AuditRecord** y **Alert** para registrar cada acción realizada por los usuarios y cada anomalía detectada por los dispositivos. Es fundamental para el cumplimiento normativo y la reconstrucción de líneas de tiempo ante incidentes de seguridad.
<img src="Resources/Evidencias/report.png">

### 5. Billing (Facturación y Suscripciones)
Gestiona el aspecto comercial y la viabilidad del servicio para cada organización. Se encarga de la entidad **Subscription**, controlando los planes activos, precios y fechas de renovación. Este contexto habilita o restringe funcionalidades avanzadas, como el control por franjas horarias o alertas automáticas, según el estado de pago del cliente.
<img src="Resources/Evidencias/billing.png">

Descripción de los componentes identificados:
- **Comandos (Azul):** Representan las intenciones de los usuarios o sistemas externos para realizar una acción específica (ej. "Generar Código QR", "Validar Acceso").
- **Agregados (Amarillo):** Son las entidades o grupos de objetos que mantienen la consistencia de los datos y ejecutan la lógica de negocio ante un comando.
- **Políticas (Lila):** Definen reacciones automáticas del sistema ante eventos específicos ("Siempre que ocurra el Evento X, ejecutar el Comando Y").
- **Modelos de Lectura (Verde):** Representan la información que el usuario visualiza en la interfaz para poder tomar una decisión y ejecutar un comando.
- **Eventos de Dominio (Naranja):** Indican que algo relevante para el negocio ha sucedido exitosamente (ej. "Código QR Generado", "Acceso Denegado").

Este modelado permite al equipo de desarrollo tener una guía clara para la implementación de los servicios y la definición de la lógica en el código.
Descripción de los componentes identificados:
- **Comandos (Azul):** Representan las intenciones de los usuarios o sistemas externos para realizar una acción específica (ej. "Generar Código QR", "Validar Acceso"). 
- **Agregados (Amarillo):** Son las entidades o grupos de objetos que mantienen la consistencia de los datos y ejecutan la lógica de negocio ante un comando. 
- **Políticas (Lila):** Definen reacciones automáticas del sistema ante eventos específicos ("Siempre que ocurra el Evento X, ejecutar el Comando Y"). 
- **Modelos de Lectura (Verde):** Representan la información que el usuario visualiza en la interfaz para poder tomar una decisión y ejecutar un comando. 
- **Eventos de Dominio (Naranja):** Indican que algo relevante para el negocio ha sucedido exitosamente (ej. "Código QR Generado", "Acceso Denegado"). 

Este modelado permite al equipo de desarrollo tener una guía clara para la implementación de los servicios y la definición de la lógica en el código.


### 4.6.2. Software Architecture Context Diagram.

In this section, the team introduces the Software Architecture Context Diagram. This high-level overview illustrates the **SmartLock** software system as a central entity, surrounded by the key user personas and the external systems it interacts with to deliver its "Asset-Light" access control value proposition.

![Software Architecture Context Diagram](/Resources/Chapter4/umlfiles/contextDiagram.png)

**Explicación del diagrama:**

* **SmartLock System:** Es el núcleo de la plataforma que centraliza la lógica de generación de códigos QR dinámicos y la validación de reglas de acceso.
* **Usuarios:** El diagrama identifica al **Administrator** (configuración), **Security Staff** (validación móvil) y **Attendee** (usuario final) como los actores principales.
* **Sistemas Externos:** Se detalla la integración con **AWS SES** para la gestión de correos electrónicos y **Twilio API** para el envío de alertas críticas de seguridad vía SMS.

### 4.6.3. Software Architecture Container Diagrams.

In this section, the team presents the **Container Diagram** for SmartLock. This diagram expands the system's context to reveal the software containers that compose it (web applications, mobile applications, APIs, and databases). It illustrates the high-level distribution of responsibilities, exposes key technology decisions—such as Angular for the frontend, Java Spring Boot for the backend, and MySQL for persistence—and details how these containers communicate through the AWS cloud infrastructure.

![Software Architecture Container Diagram](/Resources/Chapter4/umlfiles/containerDiagram.png)

#### Diagram Explanation

The Container Diagram breaks down the internal architecture of SmartLock into the following key components:

* **Landing Page & Web Application (Frontend):** Developed using **Angular, TypeScript, and TailwindCSS**. The web application acts as a Single Page Application (SPA) that consumes the backend API. Both containers are hosted on **AWS S3** and distributed globally via **Amazon CloudFront** to ensure low latency and security via HTTPS.
* **Scanner Mobile App:** A specialized application for security staff, optimized for scanning QR codes and communicating with the server with minimal latency.
* **Core Backend API:** The system's main engine, developed in **Java using the Spring Boot framework**. It centralizes all domain-driven business logic (DDD), validates access attempts, and generates encrypted dynamic QR codes. It is deployed on **AWS Elastic Beanstalk** for automated load balancing and scaling.
* **Relational Database:** A **MySQL** database hosted on **Amazon RDS**, serving as the single source of truth. it ensures the immutability of access logs (audit trails) and the integrity of user profiles and access rules.
* **Communication:** The frontend and mobile app communicate asynchronously with the Backend API via **JSON over HTTPS**. The backend interacts with the database through **JDBC** and with third-party services (AWS SES and Twilio) via REST APIs.

### 4.6.4. Software Architecture Components Diagrams.

In this section, the team presents the **Component Diagram** for the Core Backend API container. This diagram zooms into the Java Spring Boot application to illustrate its internal structure based on Domain-Driven Design (DDD) and Layered Architecture. It shows how the system is divided into Controllers (Presentation), Services (Business Logic/Domain), and Repositories (Data Access), and how these components interact to execute the access control logic.

![Software Architecture Component Diagram](/Resources/Chapter4/umlfiles/componentDiagram.png)

#### Diagram Explanation

The Component Diagram breaks down the **Core Backend API** into the following functional layers:

* **Controllers (Presentation Layer):**
  * **Auth & Security Controller:** Exposes REST endpoints to handle user login, 2FA verification, and JSON Web Token (JWT) issuance.
  * **Access Validation Controller:** Receives API calls from the Scanner Mobile App to validate dynamic QR payloads in real-time.
  * **Space Manager Controller:** Provides endpoints for administrators (via the Web App) to perform CRUD operations on physical spaces and configure access schedules.

* **Services (Domain / Business Logic Layer):**
  * **Access Credential Service (Core Domain):** The heart of the system. It evaluates complex access policies, generates dynamic QR codes using cryptographic signatures, and determines whether an access attempt is granted or denied.
  * **Authentication Service:** Implements Role-Based Access Control (RBAC) and manages the lifecycle of credentials and tokens.
  * **Notification Publisher:** Uses the Spring ApplicationEventPublisher to asynchronously delegate alerts to prevent blocking the main execution thread during access validations.

* **Repositories (Infrastructure Layer):**
  * **Audit & Log Repository:** Uses Spring Data JPA to securely write immutable logs of every access attempt and security event into the database.
  * **Domain Data Repository:** Manage the persistence of user profiles, organizational data, doors, and policies.

* **Communication Flow:** The web and mobile applications send HTTP requests to the **Controllers**. These controllers delegate the business logic to the **Services**. The services evaluate the rules and use the **Repositories** to interact with the MySQL database via JDBC, or use the **Notification Publisher** to dispatch asynchronous emails and SMS via AWS SES and Twilio.

## 4.7. Software Object-Oriented Design.

En esta sección, el equipo presenta el diseño orientado a objetos del software, detallando la implementación interna y la estructura de componentes para cada *Bounded Context* de **SmartLock**. Los diagramas a continuación ilustran cómo se ha aplicado el enfoque de *Domain-Driven Design* (DDD) a nivel de código, definiendo claramente las responsabilidades, los límites de los agregados y los patrones de diseño utilizados tanto en la capa de presentación (Frontend) como en la lógica de negocio (Backend). Esta estructura garantiza un código modular, mantenible y altamente escalable.

### 4.7.1. Class Diagrams.

#### Diagrama de clases (Frontend)

<img src="/Resources/Chapter4/Diagram-Class/Frontend/Diagrama-de-clases-Frontend-SmartLock.png" alt="Class Diagram Frontend">

La arquitectura se organiza bajo los principios de **Domain-Driven Design (DDD)**, estructurando el frontend en contextos delimitados que separan lógicamente las responsabilidades de negocio. El núcleo reside en `spaceManagement`, que gestiona la jerarquía física desde la `Organization` hasta los `Device`, utilizando un `spaceManagementStore` en la capa de aplicación para centralizar el estado y desacoplar la vista de la infraestructura. Este se complementa con `authentication` y `access`, encargados de la identidad y los permisos mediante `Account` y `Subject`, mientras que `report` se especializa en la observabilidad a través de entidades de auditoría y alertas. Finalmente, `billing` opera de forma independiente para controlar el ciclo de vida de las suscripciones en el dominio de pagos.
<br><br>
La interacción entre estos contextos y las clases de frontend se facilita mediante un **Kernel Compartido** (`shared`), donde la capa de infraestructura provee una `BaseApiEndpoint` de la cual heredan los servicios específicos para estandarizar el consumo de APIs. En la capa de presentación, los componentes se dividen en `views` (contenedores de alto nivel) y `components` (piezas reutilizables como `OrganizationCard`), los cuales interactúan con los **Stores** para obtener datos de manera reactiva en lugar de consultar directamente a los servicios. Todo el sistema es orquestado por el `AppComponent`, que integra el `Layout` compartido para mantener una interfaz consistente en toda la plataforma.
#### Diagrama de clases (Backend)

<img src="/Resources/Chapter4/Diagram-Class/Backend/Class-Diagram-Backend-image.png" alt="Class Diagram Backend">

El backend de SmartLock ha sido estructurado estrictamente bajo los principios de *Domain-Driven Design* (DDD) utilizando el framework Spring Boot. La arquitectura se divide en 5 *Bounded Contexts* y 8 agregados principales, derivados del *Event Storming*, garantizando un alto nivel de cohesión y un bajo acoplamiento. Se emplean *Aggregate Roots* (como Security y Organization) para orquestar entidades secundarias (Door y Office), asegurando el cumplimiento de las reglas de negocio en la capa de dominio antes de ejecutar cualquier cambio de estado. 

Adicionalmente, se implementaron patrones de diseño estratégico como *Assembler* para la conversión de datos y aislamiento de la capa de presentación, el uso de *Records* de Java para garantizar la inmutabilidad de los DTOs, e interfaces dedicadas para los servicios y repositorios. Esta abstracción asegura un sistema altamente mantenible y preparado para escalar sin generar deuda técnica.

## 4.8. Database Design.

### 4.8.1. Database Diagrams.

<img src="/Resources/Chapter4/Data-Base-Diagram/Data-Base-Diagram-image.png" alt="Database Diagram">

El diagrama de base de datos para SmartLock se ha estructurado bajo un enfoque de normalización 3FN y *Domain-Driven Design* (DDD), organizando la información en *Bounded Contexts* que actúan como *Aggregate Roots* (como Users y Organization) para garantizar la integridad operativa y la escalabilidad mediante el uso de tipos de datos atómicos en MySQL. Desde la perspectiva de seguridad y persistencia, el diseño separa estrictamente las credenciales en la tabla *authentications* y los datos sensibles en *user_profiles* (con correos encriptados) para cumplir con las leyes de protección de datos, mientras que la tabla *access_logs* asegura una auditoría inmutable de cada evento físico. Finalmente, la arquitectura está totalmente optimizada para un ORM como Hibernate, facilitando el mapeo de relaciones uno-a-muchos y uno-a-uno mediante claves foráneas claras y tipos bigint, lo que permite un manejo eficiente de la carga perezosa (*Lazy Loading*) y una transición fluida del modelo relacional al código en Spring Boot.
