# 📄 Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema de Bankify tiene los siguientes requerimientos (descripción a alto nivel):

### 1.1 Requerimientos funcionales

El sistema de Bankify debe tener la capacidad de:

1. Permitir la autenticación de clientes mediante usuario y contraseña.
2. Permitir consultar el saldo de una cuenta bancaria.
3. Permitir realizar depósitos en una cuenta.
4. Permitir gestionar clientes (crear, actualizar, activar e inactivar).
5. Generar un reporte tributario en formato PDF.

### 1.2 Requerimientos funcionales

El sistema de Bankify debe tener:

1. Disponibilidad mínima del 99%.
2. Cifrado de información sensible (contraseñas y datos financieros).
3. tiempo de respuesta no debe superar 3 segundos en consultas normales.
4. Capacidad de escalar para soportar crecimiento de clientes.
5. Control de acceso basado en autenticacion obligatoria. 

## 2. Diagramas de caso de uso

### 2.1 Requerimiento Funcional 1

| Campo | Descripción |
|------|-------------|
| **ID** | RF-01 |
| **Nombre del requerimiento** | *Autenticación de cliente* |
| **Descripción** | *El sistema debe permitir al cliente autenticarse mediante usuario y contraseña para acceder a sus cuentas.* |
| **Precondiciones** | *El cliente debe estar previamente registrado y activo en el sistema.* |
| **Actor** | *Cliente Bankify* |
| **Flujo principal** | 1. El actor ingresa usuario y contraseña. …<br> 2. El sistema valida las credenciales.…<br>3. El sistema permite el acceso al menú principal.… |
| **Diagrama de caso de uso** |![Primer caso de uso - Bankify](lab4/docs/uml/primerCasoUso.png)|
| **Poscondiciones** | *El cliente visualiza correctamente el saldo actualizado. …* |


### 2.2 Requerimiento Funcional 2

| Campo | Descripción |
|------|-------------|
| **ID** | RF-02 |
| **Nombre del requerimiento** |*Consulta de saldo* |
| **Descripción** | *El sistema debe permitir al cliente consultar el saldo disponible de su cuenta bancaria. …* |
| **Precondiciones** | * El cliente debe estar autenticado en el sistema. …* |
| **Actor** | * Cliente Bankify * |
| **Flujo principal** | 1. El actor selecciona la opción consultar saldo. …<br>2.El sistema solicita la información al sistema principal.…<br>3. El sistema muestra el saldo actual de la cuenta.… |
| **Diagrama de caso de uso** |![Segundo caso de uso - Bankify](lab4/docs/uml/segundoCasoUso.png)|
| **Poscondiciones** | *El cliente visualiza correctamente el saldo actualizado.* |

### 2.3 Requerimiento Funcional 3

| Campo | Descripción |
|------|-------------|
| **ID** | RF-03 |
| **Nombre del requerimiento** | *Realizar depósito* |
| **Descripción** | *El sistema debe permitir al cliente realizar un depósito en una cuenta bancaria. …* |
| **Precondiciones** | *El cliente debe estar autenticado y la cuenta debe estar activa. …* |
| **Actor** | *Cliente Bankify* |
| **Flujo principal** | 1. El actor selecciona la opción realizar depósito. …<br>2. El actor ingresa el monto. …<br>3. El sistema valida el monto. …<br>4. El sistema actualiza el saldo. …<br>5. El sistema confirma la transacción. |
| **Diagrama de caso de uso** |![Tercer caso de uso - Bankify](lab4/docs/uml/tercerCasoUso.png)|
| **Poscondiciones** | *El saldo de la cuenta queda actualizado y la transacción registrada. …* |

## 3. Preguntas
a. ¿Identifica algún requerimiento que deba detallarse más?
Si. El requirimiento de cifrado de informacion sensible debe detallarse especificado el tiempo de cifrado ylos estandares de seguridad a utilizar.
b. ¿Existen requerimientos que se contradigan entre sí? ¿cuál(es)?
No se identifican contradicciones directas. Sin embargo, los requirimientos de alta disponibilidad y escalabilidad puede implicar mayores costos y complejidad tecnica.
c. Si tuviera que dar una prioridad a los requerimientos, ¿cuáles deberían ser los 2 más importantes en una primera iteración?
1. Autenticacion de cliente.
2. consulta de saldo.
Estos permiten tener una version minima funcional y segura del sistema.
d. ¿Existe algún requerimiento que no debería realizarse?
No. Todos los requerimientos definidos están alineados con el alcance del sistema.



