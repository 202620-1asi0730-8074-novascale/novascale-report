
# Capítulo III: Requirements Specification

## 3.1. User Stories

---

### Historias de Usuario Funcionales ()

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) | Relacionado con |
| :--- | :--- | :--- | :--- | :--- |
| **HU-01** | Inicio de sesión | Como usuario, quiero iniciar sesión para acceder a las funcionalidades de NovaLeads según mis permisos. | **Dado** que el usuario está en la pantalla de inicio de sesión, **cuando** ingresa credenciales válidas, **entonces** el sistema debe autenticarlo y mostrar el panel correspondiente a su rol. | **EPIC-01** |
| **HU-02** | Gestión de usuarios y permisos | Como dueño, quiero gestionar los permisos de los usuarios para controlar qué funcionalidades puede utilizar cada vendedor. | **Dado** que el usuario tiene permisos de dueño, **cuando** modifica los permisos de un vendedor, **entonces** el sistema debe guardar los cambios y aplicar los nuevos permisos al usuario. | **EPIC-01** |
| **HU-03** | Dashboard del dueño | Como dueño, quiero visualizar un dashboard con indicadores y gráficos para conocer el estado general de las ventas y los leads de mi negocio. | **Dado** que el dueño accede al dashboard, **cuando** existen datos registrados de leads y ventas, **entonces** el sistema debe mostrar gráficos e indicadores relacionados con el estado de los leads y el rendimiento de ventas. | **EPIC-02** |
| **HU-04** | Dashboard del vendedor | Como vendedor, quiero visualizar mis indicadores de ventas para conocer mi rendimiento personal. | **Dado** que el vendedor accede al dashboard, **cuando** tiene ventas registradas, **entonces** el sistema debe mostrar sus indicadores y tasa de ventas personales sin mostrar información restringida de otros vendedores. | **EPIC-02** |
| **HU-05** | Visualización de ventas por vendedor | Como dueño, quiero visualizar las ventas realizadas por cada vendedor para evaluar el rendimiento individual del equipo. | **Dado** que el dueño accede al dashboard, **cuando** existen ventas asociadas a diferentes vendedores, **entonces** el sistema debe mostrar las ventas correspondientes a cada vendedor. | **EPIC-02** |
| **HU-06** | Registro de leads | Como vendedor, quiero registrar nuevos leads para incorporarlos al proceso comercial. | **Dado** que el usuario tiene permisos para crear leads, **cuando** registra la información requerida de un nuevo lead, **entonces** el sistema debe crear el lead y mostrarlo en la sección correspondiente. | **EPIC-03** |
| **HU-07** | Filtrado de leads | Como usuario, quiero filtrar los leads para encontrar rápidamente aquellos que cumplen determinados criterios. | **Dado** que existen leads registrados, **cuando** el usuario aplica filtros como estado, vendedor o etiqueta, **entonces** el sistema debe mostrar únicamente los leads que cumplen con los filtros seleccionados. | **EPIC-03** |
| **HU-08** | Cambio de estado de un lead | Como usuario, quiero cambiar el estado de un lead para mantener actualizado su progreso dentro del proceso comercial. | **Dado** que el usuario visualiza un lead, **cuando** selecciona un nuevo estado como activo, hot, perdido o sin respuesta, **entonces** el sistema debe actualizar y mostrar el nuevo estado del lead. | **EPIC-03** |
| **HU-09** | Etiquetado de leads por producto | Como usuario, quiero asignar etiquetas relacionadas con productos a los leads para identificar sus intereses comerciales. | **Dado** que el usuario tiene acceso a un lead, **cuando** selecciona una o más etiquetas de productos, **entonces** el sistema debe asociarlas al lead y mostrarlas en su información. | **EPIC-03** |
| **HU-10** | Gestión de etiquetas | Como usuario autorizado, quiero crear y editar etiquetas para mantener organizada la información comercial. | **Dado** que el usuario tiene permisos para gestionar etiquetas, **cuando** crea o modifica una etiqueta, **entonces** el sistema debe guardar el cambio y actualizar la etiqueta en los registros donde corresponda. | **EPIC-03** |
| **HU-11** | Visualización de contactos | Como usuario, quiero visualizar una lista de contactos para consultar las personas registradas en el sistema. | **Dado** que existen contactos registrados, **cuando** el usuario accede a la sección de contactos, **entonces** el sistema debe mostrar los contactos disponibles según sus permisos de acceso. | **EPIC-04** |
| **HU-12** | Clasificación de contacto | Como usuario, quiero identificar si un contacto es un lead o un cliente para conocer su situación comercial. | **Dado** que existe un contacto registrado, **cuando** el usuario consulta su información, **entonces** el sistema debe mostrar si está clasificado como lead o cliente. | **EPIC-04** |
| **HU-13** | Edición de información de contacto | Como usuario autorizado, quiero editar la información de un contacto para mantener sus datos actualizados. | **Dado** que el usuario tiene permisos de edición, **cuando** modifica los datos de un contacto y guarda los cambios, **entonces** el sistema debe actualizar la información del contacto. | **EPIC-04** |
| **HU-14** | Creación automática de contactos | Como usuario, quiero que un contacto se cree automáticamente cuando una persona inicia una conversación por WhatsApp. | **Dado** que una persona que no está registrada envía un mensaje por WhatsApp, **cuando** el sistema recibe el mensaje, **entonces** debe crear automáticamente un contacto utilizando la información disponible. | **EPIC-05** |
| **HU-15** | Visualización de conversaciones | Como vendedor, quiero visualizar las conversaciones vinculadas a mis contactos para gestionar la comunicación con ellos desde NovaLeads. | **Dado** que existe un contacto con una conversación asociada a WhatsApp, **cuando** el vendedor accede a la sección de conversaciones, **entonces** debe poder visualizar el historial de mensajes correspondiente. | **EPIC-05** |
| **HU-16** | Notificación de nuevos mensajes | Como usuario, quiero recibir una notificación cuando llegue un nuevo mensaje para poder responder oportunamente. | **Dado** que el usuario está utilizando NovaLeads, **cuando** un contacto envía un nuevo mensaje, **entonces** el sistema debe mostrar una notificación en la parte superior de la pantalla. | **EPIC-05** |
| **HU-17** | Temporizador de conversaciones | Como vendedor, quiero visualizar cuánto tiempo lleva sin responder una conversación para priorizar la atención de los contactos. | **Dado** que una conversación tiene un mensaje pendiente de respuesta, **cuando** transcurre el tiempo desde la recepción del mensaje, **entonces** el sistema debe mostrar un temporizador asociado a la conversación. | **EPIC-05** |
| **HU-18** | Prioridad automática de conversaciones | Como usuario, quiero que las conversaciones sin respuesta reciban una etiqueta de prioridad después de un tiempo determinado para identificar aquellas que requieren atención. | **Dado** que una conversación tiene un mensaje sin responder, **cuando** el temporizador supera el umbral configurado, **entonces** el sistema debe agregar automáticamente la etiqueta de prioridad a la conversación. | **EPIC-05** |
| **HU-19** | Ordenamiento y filtrado de conversaciones | Como usuario, quiero ordenar y filtrar las conversaciones para encontrar rápidamente aquellas que requieren atención. | **Dado** que existen múltiples conversaciones, **cuando** el usuario selecciona criterios como prioridad, etiquetas o vendedor, **entonces** el sistema debe mostrar las conversaciones que cumplen con los criterios seleccionados. **Dado** que el usuario es dueño, **cuando** selecciona un vendedor como filtro, **entonces** el sistema debe mostrar las conversaciones asignadas a dicho vendedor. | **EPIC-05** |
| **HU-20** | Perfil del vendedor | Como vendedor, quiero consultar y editar mi perfil para mantener actualizada mi información personal dentro de NovaLeads. | **Dado** que el vendedor ha iniciado sesión, **cuando** accede a la sección de perfil y modifica información permitida, **entonces** el sistema debe guardar y mostrar los datos actualizados. | **EPIC-06** |
---

### Historias de Usuario No Funcionales ()

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) | Epic Relacionada |
| :--- | :--- | :--- | :--- | :--- |
| **HNF-01** | Latencia Dashboard | Actualización inmediata. | **Dado** que , **Cuando** la DB registra el evento, **Entonces** actualiza el dashboard en < 1 segundo. | **EPIC-08** |

---

### Technical Stories

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) |
| :--- | :--- | :--- | :--- |
| **TS-01** | Documentación OpenAPI | Como equipo backend, quiero implementar documentación automática con Swagger/OpenAPI, para mantener una especificación actualizada y accesible de todos los endpoints de la API. | Dado que la API se encuentra en ejecución, cuando un usuario accede al endpoint /api/docs, entonces debe visualizar todos los recursos, métodos y esquemas de respuesta actualizados. |

---

### Definición de Epics (Módulos Generales)

| Épica | Nombre | Descripción | Historias relacionadas |
| :--- | :--- | :--- | :--- |
| **EPIC-01** | Autenticación y permisos | Gestionar el acceso de los usuarios a NovaLeads, incluyendo el inicio de sesión, los roles y los permisos que determinan las funcionalidades disponibles para cada usuario. | HU-01, HU-02 |
| **EPIC-02** | Dashboard y métricas | Proporcionar indicadores y gráficos que permitan a los dueños visualizar el rendimiento general del negocio y a los vendedores consultar sus propios resultados de ventas. | HU-03, HU-04, HU-05 |
| **EPIC-03** | Gestión de leads | Permitir registrar, consultar, filtrar, clasificar y actualizar leads, así como utilizar etiquetas para identificar intereses relacionados con productos y facilitar su seguimiento comercial. | HU-06, HU-07, HU-08, HU-09, HU-10 |
| **EPIC-04** | Gestión de contactos | Centralizar la información de los contactos y permitir identificar si corresponden a leads o clientes, además de consultar y actualizar sus datos según los permisos del usuario. | HU-11, HU-12, HU-13 |
| **EPIC-05** | Gestión de conversaciones | Gestionar las conversaciones vinculadas con WhatsApp, incluyendo la creación automática de contactos, notificaciones de nuevos mensajes, temporizadores de respuesta, prioridades y filtros para organizar las conversaciones. | HU-14, HU-15, HU-16, HU-17, HU-18, HU-19 |
| **EPIC-06** | Perfil de usuario | Permitir a los vendedores consultar y actualizar la información de su perfil dentro de NovaLeads. | HU-20 |

## 3.2. Impact Mapping

<div align="center">
  <img src="/Resources/Chapter3/MapaImpacto.png" alt="Mapa de Impacto" width="700"/>
</div>
<br>

## 3.3. Product Backlog Priorizado

| # Orden | User Story Id | Título | Descripción | Story Points (1 / 2 / 3 / 5 / 8) |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **HU-01** | Inicio de sesión estándar | Como administrador, deseo ingresar con correo y clave para acceder al panel de control. | 8 |

---

### Evidencias de Gestión en Jira

A continuación, se adjuntan las capturas del tablero de Jira utilizado para la gestión del Backlog y la estimación de Story Points del equipo de NovaScale.

<div align="center">
  <img src="/Resources/Chapter3/story_points.png" alt="Story Points" width="500"/><br>
  <i>Story Points</i><br><br>
  
  <img src="/Resources/Chapter3/formato.png" alt="Formato de HU" width="500"/><br>
  <i>Formato de Historias de Usuario</i><br><br>
  
  <img src="/Resources/Chapter3/organizacion.png" alt="Estructura de prioridad" width="500"/><br>
  <i>Estructura de Prioridad</i>
</div>
<br>

**Enlace al tablero de Jira:** 
