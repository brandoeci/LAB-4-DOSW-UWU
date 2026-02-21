## 3. Diagrama de Contexto

### 3.1 Diagrama

A continuación se relaciona el diagrama de contexto del sistema **Bankify**:

![Diagrama de contexto - Bankify](https://github.com/brandoeci/LAB-4-DOSW-UWU/blob/develop/lab4/docs/uml/Diagrama_Contexto.png)


---

### 3.2 Actores

En este cuadro se muestran los actores (roles) que interactúan con el sistema según el diagrama:

| Actor / Rol        | Descripción |
|--------------------|-------------|
| Cliente Bankify     | Cliente que tiene una o más cuentas registradas en Bankify y usa el sistema para ver sus cuentas y hacer transacciones (por ejemplo depósitos). |

---

### 3.3 Sistemas externos

En este cuadro se muestran los sistemas externos que se comunican con Bankify según el diagrama:

| Sistema                              | Descripción |
|--------------------------------------|-------------|
| Sistema Principal de gestión Bankify | Sistema central donde se almacena y se gestiona toda la información relacionada con las cuentas de los clientes. Recibe las solicitudes del sistema virtual y realiza las acciones necesarias. |

## 4. Alcance del Sistema

El sistema incluirá:

- Autenticación de usuarios (clientes y operadores).
- Gestión de clientes (crear, activar, inactivar, actualizar).
- Gestión de cuentas bancarias.
- Consulta de saldo.
- Realización de depósitos.
- Generación de reporte tributario en PDF.
- Generación y envío de reporte tributario global en JSON a la DIAN.

Fuera del alcance:

- Transferencias entre bancos.
- Retiros de dinero.
- Integración con pasarelas de pago.
- Servicios financieros avanzados (créditos, inversiones, etc.).
