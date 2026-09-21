## Arquitectura

La aplicación está organizada en diferentes componentes que permiten gestionar la interacción con el usuario, la autenticación, el acceso a datos y el registro de actividades.

```mermaid
flowchart LR
    U[Usuario] --> F[Frontend - React / HTML / CSS]
    F --> API[API - Node.js / Express]
    API --> AUTH[Autenticación]
    API --> BD[(PostgreSQL)]
    API --> LOG[Registro de actividad]