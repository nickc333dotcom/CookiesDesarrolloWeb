| Criterio | LocalStorage | Cookies (HttpOnly) |
| :--- | :--- | :--- |
| **Acceso desde JavaScript** | Sí (Vulnerable a ataques XSS) | No (El flag HttpOnly bloquea el acceso a JS) |
| **Envío al servidor** | Manual (Debes incluirlo en cada Header) | Automático (El navegador la envía solo) |
| **Tamaño máximo** | Grande (Aprox. 5MB - 10MB) | Muy pequeño (Aprox. 4KB) |
| **Seguridad CSRF** | Inmune por defecto | Vulnerable (Requiere configurar flag SameSite) |
| **Persistencia / Expiración** | Permanente hasta que se borre a mano | Configurable (Se puede poner fecha de expiración) |
