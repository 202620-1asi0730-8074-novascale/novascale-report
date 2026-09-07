
# Capítulo III: Requirements Specification

## 3.1. User Stories

---

### Historias de Usuario Funcionales ()

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) | Relacionado con |
| :--- | :--- | :--- | :--- | :--- |
| **HU-01** | Inicio de sesión estándar | Acceso al panel administrativo. | **Dado** que el administrador está en el login, **Cuando** ingresa correo y clave correctos, **Entonces** accede al panel de control. | **EPIC-01** |

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

| Epic ID | Nombre de la Epic | Descripción |
| :--- | :--- | :--- |
| **EPIC-01** | **Gestión de Identidad y Cuenta** | Como usuario del sistema, quiero gestionar mi autenticación, seguridad de perfil y acceso inicial para acceder de forma segura a la plataforma. |

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
