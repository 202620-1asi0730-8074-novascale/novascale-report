# Capítulo IV: Product Design

Este capítulo guiará el proceso de diseño a través de lineamientos claros de estilo, arquitectura de información, navegación y diseño de interfaces.

---

## 4.1. Style Guidelines.
Un Style Guideline es un conjunto de reglas y normas que definen cómo se debe redactar, diseñar o presentar documentos, contenido web, software u otros trabajos creativos. A continuación se describen las directrices que aseguran la uniformidad estética del proyecto.<br>

### 4.1.1. General Style Guidelines.

#### Branding
Para la creación de la identidad visual de **NovaLeads** se optó por un diseño moderno y profesional que transmita eficiencia, transparencia, limpieza visual y organización.
El logotipo simboliza el orden y priorización de elementos que ofrece el sistema.

![](Resources/Chapter4/style/logo-NovaLeads.jpg)
![Logo Secundario](Resources/Chapter4/style/logo.jpg)

#### Typography
Para el sistema de NovaLeads se ha seleccionado **Inter** como la familia tipográfica principal. Diseñada específicamente para pantallas e interfaces de usuario, Inter es una tipografía sans-serif que ofrece una legibilidad excepcional en una amplia variedad de dispositivos y resoluciones. Su diseño neutro pero moderno permite que los datos y el contenido destaquen sin distracciones visuales, un factor crítico en un entorno CRM donde la claridad y velocidad de lectura son primordiales.

- **Títulos y encabezados (Headings)**: Utilizan el peso **Semi-Bold** y **Bold** para establecer una jerarquía visual clara, transmitiendo solidez y guiando al usuario a través de los dashboards.
- **Cuerpo de texto (Body Text)**: Emplea el peso **Regular** con un interlineado ajustado, garantizando comodidad y reduciendo la fatiga visual durante el uso prolongado de la plataforma.
- **Botones y Etiquetas (Labels)**: Se aplica el peso **Medium**, ofreciendo el contraste perfecto para elementos interactivos, estados y menús de navegación.

![Typography](Resources/Chapter4/style/typography.png)

El estilo general busca mantener una comunicación **clara, directa y confiable** para los dos públicos objetivos.


#### Colors

La paleta escogida utiliza 4 colores en forma de semáforo para representar niveles de priorización en nuestro sistema. Junto a ellos se utilizan 2 colores neutros para textos y sombras, y un color cercano al blanco para fondos.

![](Resources/Chapter4/style/paleta.png)
![](Resources/Chapter4/style/colors.png)

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

#### Desktop Web Browser
<p align="center">
  <img src="Resources/Chapter4/wireframes/landing%20page%20-wireframe.png" width="800" alt="Landing Page Wireframe Desktop">
</p>

#### Mobile Web Browser
<p align="center">
  <img src="Resources/Chapter4/wireframes-mobile/Landing page mobile.png" width="400" alt="Landing Page Wireframe Mobile">
</p>

* **Elementos clave:** 

### 4.3.2. Landing Page Mock-up.
El mock-up de alta fidelidad integra la identidad visual de la marca, incluyendo la paleta de colores, tipografía y elementos gráficos finales. Este diseño representa la apariencia exacta que tendrá la aplicación web una vez implementada.

#### Desktop Web Browser
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-landing-page.png" width="800" alt="Landing Page Mockup Desktop">
</p>

#### Mobile Web Browser
<p align="center">
  <!-- PENDIENTE: Agrega aquí la ruta de tu mockup móvil cuando lo tengas -->
  <img src="Resources/Chapter4/mockups-mobile/novaleads-landing-mobile.png" width="400" alt="Landing Page Mockup Mobile"> 
  
</p>


## 4.4. Web Applications UX/UI Design.


### 4.4.1. Web Applications Wireframes.

Los wireframes de la aplicación web definen la estructura principal de la interfaz de NovaLeads.

### 1. Inicio de Sesión (Login)
#### Desktop Version
<p align="center"><img src="Resources/Chapter4/wireframes/novaleads-login-wireframe.png" width="800" alt="Login Wireframe Desktop"></p>

#### Mobile Version
<p align="center">
  <img src="Resources/Chapter4/wireframes-mobile/NovaLeads mobile login.png" width="400" alt="Login Wireframe Mobile">
</p>

### 2. Crear Cuenta (Sign Up)
<p align="center">
  <img src="Resources/Chapter4/wireframes/novaleads-signup-wireframe.png" width="800" alt="Sign Up Wireframe">
</p>

### 3. Recuperar Contraseña (Forgot Password)
<p align="center">
  <img src="Resources/Chapter4/wireframes/NovaLeads forgot password wireframe.png" width="800" alt="Forgot Password Wireframe">
</p>

### 4. Planes de Suscripción (Pricing)
<p align="center">
  <img src="Resources/Chapter4/wireframes/NovaLeads pricing wireframe.png" width="800" alt="Pricing Wireframe">
</p>

### 5. Dashboard Principal
#### Desktop Version
<p align="center"><img src="Resources/Chapter4/wireframes/novaleads-dashboard-wireframe.png" width="800" alt="Dashboard Wireframe Desktop"></p>

#### Mobile Version
<p align="center">
  <img src="Resources/Chapter4/wireframes-mobile/novaleads-dashboard-wireframe-mobile.png" width="400" alt="Dashboard Wireframe Mobile">
</p>

### 6. CRM Dashboard
<p align="center"><img src="Resources/Chapter4/wireframes/novaleads-crm-wireframe.png" width="800" alt="CRM Dashboard Wireframe"></p>

### 7. Directorio de Clientes
<p align="center"><img src="Resources/Chapter4/wireframes/crm-customer-directory-wireframe.png" width="800" alt="Customer Directory Wireframe"></p>

### 8. Conversaciones de Contacto
<p align="center"><img src="Resources/Chapter4/wireframes/crm-contact-chat-wireframe.png" width="800" alt="Contact Chat Wireframe"></p>

### 9. Modal Añadir Lead
<p align="center"><img src="Resources/Chapter4/wireframes/add-new-lead-modal.png" width="800" alt="Add Lead Modal Wireframe"></p>

### 10. Configuración del Sistema
<p align="center"><img src="Resources/Chapter4/wireframes/novaleads-settings-wireframe.png" width="800" alt="Settings Wireframe"></p>### 4.4.2. Web Applications Wireflow Diagrams.
Esta sección presenta los wireflows que conectan visualmente las pantallas de baja fidelidad para demostrar el flujo de interacción de los objetivos principales del usuario.

#### User Goal 1: Autenticación y acceso al sistema
El usuario debe poder iniciar sesión ingresando sus credenciales para acceder al Dashboard Principal.
<p align="center">
  <img src="Resources/Chapter4/mockups/userflow_login.png" width="800" alt="Wireflow Login">
</p>

#### User Goal 2: Registro de un nuevo prospecto (Lead)
El vendedor, desde el Directorio de Clientes o el Dashboard CRM, puede registrar los datos de un nuevo contacto comercial y agregarlo al pipeline.
<p align="center">
  <img src="Resources/Chapter4/mockups/userflow_lead.png" width="800" alt="Wireflow Add Lead"> 
</p>

### 4.4.3. Web Applications Mock-ups.
Esta sección presenta los mock-ups de alta fidelidad de la plataforma web de NovaLeads. Estos diseños representan la apariencia visual final del sistema, incluyendo identidad visual, paleta de colores, tipografía, distribución de componentes y experiencia de usuario orientada a la implementación real del producto.

### 1. Inicio de Sesión (Login)
#### Desktop Version
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-login.png" width="800" alt="Login Mockup Desktop">
</p>

#### Mobile Version
<p align="center">
  <img src="Resources/Chapter4/mockups-mobile/novaleads-mobile-login.png" width="400" alt="Login Mockup Mobile">
</p>
**Descripción:** Pantalla de acceso seguro al sistema principal. Adaptada responsivamente para uso en dispositivos móviles de agentes en campo.

### 2. Crear Cuenta (Sign Up)
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-signup.png" width="800" alt="Sign Up Mockup">
</p>
**Descripción:** Formulario de registro B2B inicial que captura los datos del usuario y de su compañía para crear un entorno aislado.

### 3. Recuperar Contraseña (Forgot Password)
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-forgot-password.png" width="800" alt="Forgot Password Mockup">
</p>
**Descripción:** Interfaz simple y segura para enviar el enlace de recuperación de contraseña mediante el correo electrónico de trabajo.

### 4. Planes de Suscripción (Pricing)
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-pricing.png" width="800" alt="Pricing Mockup">
</p>
**Descripción:** Presentación transparente de los tiers de suscripción (Starter, Professional, Enterprise) diseñados para escalar con el cliente.

### 5. Dashboard Principal
#### Desktop Version
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-dashboard.png" width="800" alt="Dashboard Mockup Desktop">
</p>

#### Mobile Version
<p align="center">
  <img src="Resources/Chapter4/mockups-mobile/novaleads-dashboard-mobile.png" width="400" alt="Dashboard Mockup Mobile">
</p>
**Descripción:** Vista general de indicadores y métricas del sistema. La versión móvil prioriza los KPIs más importantes para una lectura rápida.

### 6. CRM Dashboard
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-crm-dashboard.png" width="800" alt="CRM Dashboard Mockup">
</p>
**Descripción:** Panel de control especializado para la gestión de relaciones con clientes.

### 7. Directorio de Clientes
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-customers-directory.png" width="800" alt="Customer Directory Mockup">
</p>
**Descripción:** Lista completa y detallada de clientes y prospectos.

### 8. Conversaciones de Contacto
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-contact-conversations.png" width="800" alt="Contact Chat Mockup">
</p>
**Descripción:** Interfaz de comunicación directa e historial de mensajes con contactos.

### 9. Modal Añadir Lead
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-crm-add lead.png" width="800" alt="Add Lead Mockup">
</p>
**Descripción:** Formulario para registrar un nuevo prospecto o cliente potencial en el CRM.

### 10. Configuración del Sistema
<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-system-settings.png" width="800" alt="System Settings Mockup">
</p>
**Descripción:** Interfaz para administrar preferencias y configuración general de la cuenta.

### 4.4.4. Web Applications User Flow Diagrams.
En la siguiente sección se detalla el diagrama de flujo de usuario (User Flow) que mapea la navegación lógica a través de la plataforma NovaLeads.

<p align="center">
  <img src="Resources/Chapter4/style/UserFlow.png" width="1000" alt="User Flow Diagram NovaLeads">
</p>

## 4.5. Web Applications Prototyping

En esta sección se presenta el prototipo interactivo de alta fidelidad para la aplicación web de **NovaLeads**. Este diseño simula la experiencia real del usuario final (SDRs y Ejecutivos Comerciales), integrando la identidad visual, la interfaz de usuario (UI) y el flujo de navegación entre las pantallas principales del sistema, como el dashboard, el CRM y la gestión de chats.

A continuación, se presentan las evidencias visuales y los enlaces de acceso directo al entorno de diseño y a la demostración interactiva:

<p align="center">
  <img src="Resources/Chapter4/mockups/novaleads-crm-dashboard.png" width="900" alt="Vista general del prototipo en Figma">
</p>

<br>

### 🔗 Enlaces de Acceso

*   **Prototipo Interactivo (Modo Presentación):** [Ver simulación en Figma](https://www.figma.com/proto/2WXesYSYFt2TovwFrZxvJj/Untitled?node-id=0-1&t=jnp821tF7TLgtdzl-1)
*   **Archivo de Diseño (Canvas):** [Ver entorno de trabajo en Figma](https://www.figma.com/design/2WXesYSYFt2TovwFrZxvJj/Untitled?node-id=0-1&t=jnp821tF7TLgtdzl-1)
*   **Video Explicativo:** [Ver demostración grabada](https://drive.google.com/file/d/1X63rH3-6A6zqBckWCkUrWUpIRZiFSD_c/view?usp=sharing)

<br>

## 4.6. Domain-Driven Software Architecture

En esta sección se define la arquitectura central de **NovaLeads** basándose en los principios de Domain-Driven Design (DDD). El objetivo principal es alinear la complejidad técnica del código con la realidad del modelo de negocio. Para lograrlo, la arquitectura se basará en un **RESTful API** desarrollado con **C# (ASP.NET Core)** para la lógica del lado del servidor, y **Vue.js** para las aplicaciones web del lado del cliente.

El sistema se ha dividido en los siguientes *Bounded Contexts* estratégicos:

### 4.6.1. Design-Level EventStorming

A diferencia del Big Picture, el *Design-Level EventStorming* se enfoca en definir los límites de los agregados, los comandos que disparan cambios de estado y las políticas que gobiernan las reglas de negocio de NovaLeads.

#### 1. Lead Management (Core Domain)
Contexto central encargado de la operativa comercial CRM. Su responsabilidad principal es modelar el ciclo de vida comercial, gestionando entidades como **Lead**, **Contact** y **Deal** (oportunidades). Administra la transición de un prospecto desde que ingresa al sistema hasta que se convierte en un cliente activo.

<p align="center">
  <img src="Resources/Chapter4/Evidencias/lead-management.png" alt="Lead Management EventStorming">
</p>

#### 2. Communication Management
Este contexto se enfoca estrictamente en la comunicación omnicanal con los contactos. Gestiona las interacciones mediante agregados como **Conversation**, **Message** y **InteractionHistory**. Centraliza el historial de chats para que los SDR y ejecutivos tengan todo el contexto previo a la negociación.

<p align="center">
  <img src="Resources/Chapter4/Evidencias/communication.png" alt="Communication EventStorming">
</p>

#### 3. Identity and Access Management (IAM)
Responsable de la seguridad a nivel de software, autenticación y validación de la identidad. Administra los **Users**, **Roles** (Salesperson, Administrator) y credenciales. Asegura el control de acceso a métricas financieras y asignaciones de leads.

<p align="center">
  <img src="Resources/Chapter4/Evidencias/iam.png" alt="IAM EventStorming">
</p>

#### 4. Organization & Subscriptions
Dedicado a la gestión multitenant de las empresas que contratan NovaLeads. Utiliza entidades como **Organization** y **Subscription** para controlar los planes SaaS (Starter, Pro, Enterprise), los cupos de vendedores por empresa y las fechas de renovación de licencias.

<p align="center">
  <img src="Resources/Chapter4/Evidencias/organization.png" alt="Organization EventStorming">
</p>

**Descripción de los componentes identificados:**

*   **Comandos (Azul):** Representan las intenciones de los usuarios o sistemas externos para realizar una acción específica (ej. *Create Lead*, *Send Message*).
*   **Agregados (Amarillo):** Son las entidades o grupos de objetos que mantienen la consistencia de los datos y ejecutan la lógica de negocio ante un comando (ej. *Lead*, *Conversation*).
*   **Políticas (Lila):** Definen reacciones automáticas del sistema ante eventos específicos (ej. *Siempre que un Deal pase a Closed Won, notificar al manager*).
*   **Modelos de Lectura (Verde):** Representan la información que el usuario visualiza en la interfaz (ej. *Lead Directory*, *Pipeline Dashboard*).
*   **Eventos de Dominio (Naranja):** Indican que algo relevante para el negocio ha sucedido exitosamente (ej. *LeadCreated*, *MessageSent*).

Este modelado detallado proporciona al equipo de desarrollo una guía clara para la implementación de los controladores, servicios y repositorios del **RESTful API** de NovaLeads.


### 4.6.2. Software Architecture Context Diagram.

En esta sección se presenta el Software Architecture Context Diagram de **NovaLeads**. Este diagrama ofrece una visión de alto nivel de la plataforma CRM, mostrando a los usuarios principales y los sistemas externos con los que interactúa para centralizar la gestión de leads, clientes, conversaciones y resultados de ventas.

![Software Architecture Context Diagram](Resources/Chapter4/C4/contextDiagram.png)

**Explicación del diagrama:**

* **NovaLeads:** Es el sistema central de la solución. Permite gestionar usuarios, leads, contactos, conversaciones, oportunidades y métricas de ventas desde una única plataforma.

* **Dueño de pyme o startup:** Administra el negocio dentro de NovaLeads, gestiona usuarios y permisos, consulta indicadores de ventas y supervisa el estado general de los leads y oportunidades.

* **Vendedor:** Registra y actualiza leads, consulta contactos, administra conversaciones y realiza el seguimiento de las oportunidades comerciales asignadas.

* **Visitante:** Accede a la Landing Page para conocer la propuesta de valor de NovaLeads e iniciar el flujo de registro o inicio de sesión.

* **WhatsApp Business API:** Es el sistema externo que permite a NovaLeads recibir mensajes de los contactos y enviar respuestas mediante la integración con WhatsApp.

### 4.6.3. Software Architecture Container Diagram.

En esta sección se presenta el **Container Diagram** de **NovaLeads**. Este diagrama amplía la visión del contexto del sistema y muestra los contenedores de software que componen la plataforma CRM, así como la distribución de responsabilidades, las principales decisiones tecnológicas y la comunicación entre los componentes.

![Software Architecture Container Diagram](Resources/Chapter4/C4/containerDiagram.png)

#### Explicación del diagrama

El Container Diagram descompone la arquitectura interna de NovaLeads en los siguientes componentes principales:

* **Landing Page:** Desarrollada con **HTML, CSS y JavaScript**. Presenta la propuesta de valor de NovaLeads, sus funcionalidades, beneficios y Call to Action dirigidos a dueños de pymes, startups y equipos de venta.

* **Web Application:** Desarrollada con **Vue.js**. Permite a dueños y vendedores iniciar sesión, gestionar leads, contactos, conversaciones, oportunidades, etiquetas y métricas de ventas mediante una interfaz web responsive.

* **REST API:** Desarrollada con **ASP.NET Core y C#**. Centraliza la lógica de negocio, autenticación, autorización, gestión de usuarios, leads, contactos, conversaciones, notificaciones y métricas. Expone endpoints RESTful documentados mediante OpenAPI y Swagger.

* **Base de datos relacional:** Implementada con **MySQL**. Almacena la información de usuarios, roles, permisos, contactos, leads, etiquetas, conversaciones, mensajes, oportunidades y ventas.

* **WhatsApp Business API:** Sistema externo que permite recibir mensajes de contactos mediante webhooks y enviar respuestas desde NovaLeads.

* **Comunicación:** La Landing Page redirige a los usuarios hacia la Web Application mediante HTTPS. La Web Application consume la REST API mediante solicitudes HTTP y datos en formato JSON. La REST API accede a la base de datos mediante Entity Framework Core e intercambia mensajes con WhatsApp Business API.

### 4.6.4. Software Architecture Components Diagrams.

En esta sección se presentan los Component Diagrams de NovaLeads. Estos diagramas detallan los componentes internos de los contenedores que concentran la lógica de la solución: la Web Application y la REST API.

#### Diagrama de componentes de la Web Application

![Software Architecture Web Application Component Diagram](Resources/Chapter4/C4/webApplicationComponentDiagram.png)

* **Interfaz y navegación:**
    * **App Shell:** Inicializa la aplicación y muestra el layout compartido.
    * **Router:** Gestiona la navegación entre las vistas y protege las rutas que requieren autenticación.
    * **Login View:** Permite a los usuarios iniciar sesión según sus credenciales y permisos.
    * **Dashboard View:** Muestra indicadores, gráficos y métricas comerciales.
    * **Leads View:** Permite registrar, consultar, filtrar y actualizar leads.
    * **Conversations View:** Permite visualizar conversaciones, consultar mensajes y responder a los contactos.

* **Gestión de estado:**
    * **Authentication Store:** Centraliza la sesión, el usuario autenticado y sus permisos.
    * **Lead Store:** Centraliza los leads, filtros y etiquetas utilizadas en la gestión comercial.
    * **Conversation Store:** Centraliza las conversaciones, mensajes y prioridades de atención.
    * **Dashboard Store:** Centraliza las métricas y resultados mostrados en el dashboard.

* **Comunicación con el backend:**
    * **API Client:** Realiza solicitudes HTTP mediante JSON sobre HTTPS hacia la REST API de NovaLeads.

* **Flujo de comunicación:** Las vistas interactúan con los Stores correspondientes. Los Stores utilizan el API Client para consumir los endpoints expuestos por la REST API.

#### Diagrama de componentes de la REST API

En esta sección se presenta el **Component Diagram** del contenedor REST API de **NovaLeads**. Este diagrama detalla la estructura interna de la API, mostrando cómo se organizan los controladores, servicios de aplicación y repositorios para gestionar usuarios, leads, contactos, conversaciones, notificaciones y métricas de ventas.

![Software Architecture Component Diagram](Resources/Chapter4/C4/componentDiagram.png)

#### Explicación del diagrama

El Component Diagram descompone la REST API de NovaLeads en los siguientes componentes:

* **Controllers - Capa de presentación:**
  * **Authentication Controller:** Expone los endpoints para el inicio de sesión y la autenticación de usuarios.
  * **WhatsApp Webhook Controller:** Recibe los eventos y mensajes entrantes enviados por WhatsApp Business API.

* **Services - Capa de lógica de negocio:**
  * **User Management Service:** Gestiona usuarios, roles y permisos de dueños y vendedores.
  * **Lead Management Service:** Registra, actualiza, filtra y clasifica leads, incluyendo la gestión de etiquetas.
  * **Contact Management Service:** Gestiona la información de contactos, leads y clientes.
  * **Conversation Service:** Administra conversaciones, mensajes, temporizadores y prioridades de atención.
  * **Dashboard Service:** Calcula indicadores relacionados con leads, oportunidades, ventas y rendimiento de vendedores.
  * **Notification Service:** Genera notificaciones cuando existen nuevos mensajes o conversaciones pendientes de respuesta.

* **Repositories - Capa de acceso a datos:**
  * **Repositories:** Utilizan Entity Framework Core para almacenar y consultar la información de usuarios, roles, contactos, leads, etiquetas, conversaciones, mensajes, oportunidades y ventas en la base de datos MySQL.

* **Flujo de comunicación:** La Web Application consume los endpoints expuestos por los Controllers mediante HTTPS y JSON. Los Controllers delegan las operaciones a los Services, que aplican la lógica de negocio. Finalmente, los Services utilizan los Repositories para persistir o consultar información en MySQL. El WhatsApp Webhook Controller entrega los mensajes recibidos al Conversation Service, que registra las conversaciones y puede generar notificaciones.

## 4.7. Software Object-Oriented Design.

En esta sección se presenta el diseño orientado a objetos de **NovaLeads**. Este diseño permite representar las entidades, responsabilidades y relaciones necesarias para gestionar usuarios, permisos, contactos, leads, conversaciones, oportunidades y resultados de ventas.

La propuesta se organiza en clases que reflejan los principales procesos del dominio comercial. Cada clase encapsula información y comportamientos específicos, lo que permite mantener una estructura clara, escalable y coherente con los requisitos funcionales de la plataforma.

El diseño considera la gestión de usuarios con diferentes roles, la clasificación de contactos como leads o clientes, el seguimiento de oportunidades comerciales, el registro de conversaciones y mensajes, la administración de etiquetas y la generación de métricas para el dashboard.

A partir de esta estructura se elabora el Class Diagram, el cual detalla los atributos, métodos, relaciones, multiplicidades y responsabilidades de las clases principales que conforman NovaLeads.

### 4.7.1. Class Diagrams.

Los diagramas siguen una convención común: nombres de clases, interfaces y enumeraciones en **inglés y PascalCase** (`ConversationService`, `IUserRepository`, `LeadStatus`); atributos y métodos en **camelCase** (`createdAt`, `sendMessage()`); y valores de enumeración en **UPPER_SNAKE_CASE** (`NO_RESPONSE`). Los identificadores de clases son singulares (`User`, `Contact`, `Opportunity`). La notación UML usa `+` para miembros públicos, `-` para privados y `#` para protegidos. Las asociaciones indican nombre, dirección cuando corresponde y multiplicidad. Los tipos y estados mencionados en estos diagramas deben coincidir con los del diseño de base de datos y los requisitos.

#### Diagrama de clases de la Web Application

![Class Diagram Frontend](Resources/Chapter4/class-diagrams/classDiagramFrontend.png)

La Web Application se desarrolla con Vue.js. `App`, `AppLayout` y `Router` organizan el inicio de la aplicación y la navegación. `LoginView`, `DashboardView`, `LeadsView` y `ConversationsView` representan las vistas principales. Los componentes reutilizables, como `LeadForm`, `LeadTable`, `ConversationPanel` y `MetricsCard`, presentan información y acciones al usuario. Los Stores mantienen el estado de sesión, leads, conversaciones y métricas; los servicios consumen la REST API mediante `ApiClient`. Las clases de la interfaz son representaciones del frontend y no sustituyen a las entidades de dominio de la REST API.

#### Diagrama de clases del bounded context Identity and Access

![Class Diagram Identity and Access](Resources/Chapter4/class-diagrams/classDiagramIdentityAccess.png)

`User` representa la cuenta que accede a NovaLeads y conserva los datos editables del perfil. Cada usuario tiene un `Role`; un rol puede estar asignado a varios usuarios. `Role` agrupa objetos `Permission`, que determinan las operaciones habilitadas para todos los usuarios con ese rol. `AuthenticationService` valida las credenciales con `IPasswordHasher`, obtiene el usuario mediante `IUserRepository` y solicita el token a `ITokenProvider`. `AuthController` expone el inicio de sesión. El diagrama debe expresar las multiplicidades `Role 1 — 0..* User` y `Role 0..* — 0..* Permission`.


#### Diagrama de clases del bounded context Lead and Contact Management

![Class Diagram Lead and Contact Management](Resources/Chapter4/class-diagrams/classDiagramLeadContact.png)

`Contact` contiene los datos comunes de una persona comercial y se especializa en `Lead` o `Client`. `Lead` registra su estado y puede clasificarse con varias `Tag`; una etiqueta puede aplicarse a varios leads. Un contacto puede tener varias `Opportunity`, cada una con monto estimado, estado, fecha prevista y vendedor asignado. `LeadManagementService` y `OpportunityService` aplican las reglas de negocio a través de repositorios. Los usuarios asignados se muestran como referencias al contexto **Identity and Access**, sin duplicar la clase `User` como entidad propia de este contexto. En persistencia, `Lead` y `Client` se distinguen mediante `contacts.contact_type`.

#### Diagrama de clases del bounded context Conversation Management

![Class Diagram Conversation Management](Resources/Chapter4/class-diagrams/classDiagramConversationManagement.png)

`Conversation` está vinculada con un `Contact` y contiene cero o más `Message`. Sus atributos de estado, prioridad y tiempo pendiente permiten identificar conversaciones que requieren respuesta. La aplicación determina la prioridad automática a partir del tiempo pendiente y de un umbral fijo del sistema; no se persiste una entidad de configuración en la base de datos. `Notification` avisa al usuario responsable sobre nuevos mensajes o conversaciones pendientes. `WhatsAppWebhookController` recibe eventos de WhatsApp Business API; `ConversationService` registra los mensajes y utiliza `IWhatsAppBusinessGateway` para enviar respuestas. `Contact` y `User` son referencias a otros bounded contexts. El diagrama debe mostrar la relación `Conversation 1 — 0..* Message` y las asociaciones de conversaciones y notificaciones con sus responsables.

#### Diagrama de clases del bounded context Sales and Dashboard

![Class Diagram Sales and Dashboard](Resources/Chapter4/class-diagrams/classDiagramSalesDashboard.png)

`Sale` registra una venta realizada y se relaciona con una `Opportunity` del contexto **Lead and Contact Management**. Una oportunidad produce como máximo una venta; una venta pertenece a exactamente una oportunidad. La venta conserva el vendedor responsable al momento de registrarse. `DashboardService` calcula `DashboardSummary` y `DashboardMetric` a partir de contactos, oportunidades y ventas, con filtros según el rol del usuario. `User` y `Opportunity` se muestran como referencias externas, no como entidades redefinidas en este contexto. Las métricas derivadas no requieren una tabla `dashboard`.

## 4.8. Database Design.

El diseño de base de datos de **NovaLeads** define los objetos necesarios para persistir la información de los bounded contexts de la plataforma. La propuesta utiliza un modelo relacional, en el que las entidades se representan mediante tablas y se relacionan a través de claves primarias y claves foráneas.

Los diagramas fueron elaborados en **ERDPlus** mediante Relational Schema. Esta herramienta permite representar tablas, columnas, claves primarias, claves foráneas, relaciones y restricciones de unicidad. Los tipos de datos y tamaños de las columnas se documentan junto a cada diagrama.

La base de datos se organiza en cuatro bounded contexts: **Identity and Access**, **Lead and Contact Management**, **Conversation Management** y **Sales and Dashboard**.

### 4.8.1. Database Diagrams.

##### Identity and Access

![Database Diagram Identity and Access](Resources/Chapter4/Database-diagram/databaseIdentityAccessDiagram.png)

Este diagrama presenta las tablas que permiten identificar a los usuarios y controlar sus permisos. `users` conserva la cuenta y el rol asignado; `roles` define los perfiles de acceso; `permissions` enumera las acciones autorizables; y `role_permissions` relaciona cada rol con sus permisos.

| Tabla | Columnas principales |
| :--- | :--- |
| `roles` | `id_role: BIGINT [PK]`, `name: VARCHAR(50) [UQ]`, `description: VARCHAR(255)` |
| `users` | `id_user: BIGINT [PK]`, `email: VARCHAR(120) [UQ]`, `password_hash: VARCHAR(255)`, `status: ENUM('ACTIVE','INACTIVE')`, `created_at: DATETIME`, `updated_at: DATETIME`, `full_name: VARCHAR(120)`, `id_role: BIGINT [FK]` |
| `permissions` | `id_permission: BIGINT [PK]`, `code: VARCHAR(80) [UQ]` |
| `role_permissions` | `id_role: BIGINT [PK, FK]`, `id_permission: BIGINT [PK, FK]` |

* **`roles`:** identifica perfiles como dueño y vendedor. Un rol puede estar asignado a varios usuarios.
* **`users`:** almacena los datos de acceso y el estado de cada cuenta. Su columna `id_role` referencia `roles.id_role`; la contraseña se representa mediante su hash, no mediante el valor original.
* **`permissions`:** identifica acciones como gestionar usuarios, leads y conversaciones o consultar métricas. La unicidad de `code` evita códigos de permiso duplicados.
* **`role_permissions`:** resuelve la relación de muchos a muchos entre roles y permisos. La combinación de `id_role` e `id_permission` forma su clave primaria y evita asignar dos veces el mismo permiso a un rol.

##### Lead and Contact Management

![Database Diagram Lead and Contact Management](Resources/Chapter4/Database-diagram/databaseLeadContactDiagram.png)

Este diagrama muestra cómo se guardan los leads, clientes, etiquetas y oportunidades comerciales. `contacts` reúne los datos comunes de leads y clientes; `contact_type` distingue ambas categorías y `lead_status` registra el estado de un lead. `users` aparece como referencia al contexto Identity and Access para indicar el usuario responsable de un contacto o una oportunidad.

| Tabla | Columnas principales |
| :--- | :--- |
| `contacts` | `id_contact: BIGINT [PK]`, `full_name: VARCHAR(120)`, `email: VARCHAR(120)`, `phone: VARCHAR(30) [UQ]`, `company: VARCHAR(120)`, `contact_type: VARCHAR(10)`, `lead_status: VARCHAR(20)`, `source: VARCHAR(80)`, `created_at: DATETIME`, `updated_at: DATETIME`, `id_user: BIGINT [FK]` |
| `tags` | `id_tag: BIGINT [PK]`, `name: VARCHAR(50) [UQ]`, `color: VARCHAR(20)` |
| `contact_tags` | `id_contact: BIGINT [PK, FK]`, `id_tag: BIGINT [PK, FK]` |
| `opportunities` | `id_opportunity: BIGINT [PK]`, `title: VARCHAR(150)`, `estimated_amount: DECIMAL(12,2)`, `status: VARCHAR(10)`, `expected_close_date: DATE`, `created_at: DATETIME`, `id_user: BIGINT [FK]`, `id_contact: BIGINT [FK]` |
| `users` *(referencia externa)* | Se muestran `id_user: BIGINT [PK]`, `email: VARCHAR(120) [UQ]`, `status: ENUM('ACTIVE','INACTIVE')`, `created_at: DATETIME`, `updated_at: DATETIME`, `full_name: VARCHAR(120)` y `password_hash: VARCHAR(255)`. La definición de la tabla y su relación con `roles` pertenecen a Identity and Access. |

* **`contacts`:** registra los datos de contacto y su clasificación. `id_user` identifica al usuario responsable y `phone` permite localizar un contacto cuando llega un mensaje de WhatsApp.
* **`tags` y `contact_tags`:** permiten asignar varias etiquetas a un contacto y utilizar una misma etiqueta en distintos contactos. `contact_tags` tiene una clave primaria compuesta.
* **`opportunities`:** conserva el título, monto estimado, estado, fecha esperada de cierre, contacto asociado y usuario responsable. `id_contact` referencia `contacts.id_contact` e `id_user` referencia `users.id_user`.
* **`users`:** se incluye para hacer visibles las relaciones con contactos y oportunidades. No representa una segunda tabla física ni administra roles dentro de este contexto.

##### Conversation Management

![Database Diagram Conversation Management](Resources/Chapter4/Database-diagram/databaseConversationManagementDiagram.png)

Este diagrama representa la persistencia de conversaciones, mensajes y notificaciones. Cada conversación se asocia con un contacto y un usuario responsable. Las referencias a `contacts` y `users` muestran los datos necesarios para identificar al contacto en WhatsApp y al destinatario de las alertas, sin redefinir esas tablas en este bounded context.

| Tabla | Columnas principales |
| :--- | :--- |
| `conversations` | `id_conversation: BIGINT [PK]`, `channel: VARCHAR(30)`, `status: VARCHAR(10)`, `priority: VARCHAR(10)`, `pending_since: DATETIME`, `last_message_at: DATETIME`, `created_at: DATETIME`, `id_contact: BIGINT [FK]`, `id_user: BIGINT [FK]` |
| `messages` | `id_message: BIGINT [PK]`, `sender_type: VARCHAR(10)`, `content: TEXT`, `sent_at: DATETIME`, `external_message_id: VARCHAR(120) [UQ]`, `id_conversation: BIGINT [FK]` |
| `notifications` | `id_notification: BIGINT [PK]`, `type: VARCHAR(30)`, `content: VARCHAR(255)`, `is_read: BOOLEAN`, `created_at: DATETIME`, `id_user: BIGINT [FK]`, `id_conversation: BIGINT [FK]` |
| `contacts` *(referencia externa)* | Se muestran `id_contact: BIGINT [PK]`, `full_name: VARCHAR(120)`, `phone: VARCHAR(30) [UQ]` y `contact_type: VARCHAR(10)`. Su definición corresponde a Lead and Contact Management. |
| `users` *(referencia externa)* | Se muestran `id_user: BIGINT [PK]`, `full_name: VARCHAR(120)`, `email: VARCHAR(120) [UQ]` y `status: ENUM('ACTIVE','INACTIVE')`. Su definición corresponde a Identity and Access. |

* **`conversations`:** conserva el canal, estado, prioridad y fechas necesarias para medir el tiempo pendiente de respuesta. `id_contact` apunta al contacto y `id_user` al usuario responsable.
* **`messages`:** guarda los mensajes enviados y recibidos. `external_message_id` identifica los mensajes de un proveedor externo y evita registrar dos veces un mismo identificador.
* **`notifications`:** registra alertas para un usuario relacionadas con una conversación. `is_read` permite distinguir las alertas pendientes de las ya revisadas.
* **`contacts` y `users`:** se muestran como referencias a tablas existentes. Sus claves `id_contact` e `id_user` son destinos de las FK del contexto de conversaciones.

##### Sales and Dashboard

![Database Diagram Sales and Dashboard](Resources/Chapter4/Database-diagram/databaseSalesDashboardDiagram.png)

Este diagrama registra las ventas y muestra los datos consultados para calcular las métricas del dashboard. `sales` es la tabla propia del contexto; `opportunities` y `contacts` provienen de Lead and Contact Management, mientras que `users` proviene de Identity and Access. Estas referencias permiten relacionar una venta con su oportunidad y vendedor, y contar los leads registrados.

| Tabla | Columnas principales |
| :--- | :--- |
| `sales` | `id_sale: BIGINT [PK]`, `amount: DECIMAL(12,2)`, `sale_date: DATE`, `status: VARCHAR(20)`, `notes: TEXT`, `id_user: BIGINT [FK]`, `id_opportunity: BIGINT [FK, UQ]` |
| `opportunities` *(referencia externa)* | Se muestran `id_opportunity: BIGINT [PK]`, `title: VARCHAR(150)`, `estimated_amount: DECIMAL(12,2)`, `status: VARCHAR(10)`, `expected_close_date: DATE`, `created_at: DATETIME`, `id_user: BIGINT [FK]` e `id_contact: BIGINT [FK]`. Su definición corresponde a Lead and Contact Management. |
| `contacts` *(referencia externa)* | Se muestran `id_contact: BIGINT [PK]`, `contact_type: VARCHAR(10)`, `lead_status: VARCHAR(20)` y `created_at: DATETIME`. Su definición corresponde a Lead and Contact Management. |
| `users` *(referencia externa)* | Se muestran `id_user: BIGINT [PK]`, `email: VARCHAR(120)`, `status: ENUM('ACTIVE','INACTIVE')`, `created_at: DATETIME`, `updated_at: DATETIME`, `full_name: VARCHAR(120)` y `password_hash: VARCHAR(255)`. Su definición y la unicidad de `email` se establecen en Identity and Access. |

* **`sales`:** almacena el monto, fecha, estado y observaciones de cada venta. `id_user` identifica al vendedor y `id_opportunity` enlaza con la oportunidad que se concretó.
* **`opportunities`:** enlaza cada venta con el contacto y con la información comercial de origen. La restricción única en `sales.id_opportunity` establece un máximo de una venta por oportunidad.
* **`contacts`:** permite contar los leads por clasificación y estado, incluso cuando todavía no existe una oportunidad asociada.
* **`users`:** permite agrupar las ventas y oportunidades por usuario responsable; es la misma tabla física definida en Identity and Access.
* **Dashboard:** no necesita una tabla propia. Sus indicadores se obtienen mediante consultas a `contacts`, `opportunities` y `sales`.