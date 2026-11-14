# 01. Contexto de la organización y alcance del SGSI

## 1. La empresa

Davem Cyber Consulting S.L. es una consultora de ciberseguridad con sede en Valencia. Tiene 8 personas en plantilla y trabaja sobre todo con pymes y ayuntamientos de la Comunitat Valenciana.

Servicios que ofrece:

- Implantación de ISO/IEC 27001
- Adecuación al Esquema Nacional de Seguridad (ENS)
- Adecuación a NIS2
- Auditorías internas de seguridad
- Formación y concienciación

| Puesto | Personas |
|---|---|
| Dirección | 1 |
| Responsable de seguridad (también consultor) | 1 |
| Consultores | 3 |
| Administración de sistemas | 1 |
| Administración y contabilidad | 1 |
| Comercial | 1 |

## 2. Infraestructura

- Oficina alquilada en Valencia, con una sala de reuniones y un armario de comunicaciones cerrado con llave.
- 8 portátiles con Windows 11 y cifrado de disco.
- Microsoft 365 para correo, documentos (SharePoint y OneDrive) y Teams.
- Web corporativa con área de clientes (registro e inicio de sesión), montada con Docker en un servidor virtual de un proveedor de hosting europeo.
- NAS en la oficina para copias de seguridad.
- Router con cortafuegos y dos redes wifi (interna e invitados).
- Móviles de empresa para dirección, comercial y consultores.

## 3. Cuestiones internas y externas (4.1)

Internas:

- Empresa pequeña, una misma persona hace varias funciones.
- Se maneja información confidencial de clientes (informes de auditoría, análisis de riesgos, vulnerabilidades).
- Los consultores trabajan a menudo en casa del cliente y en remoto.
- Mucha dependencia de servicios en la nube.

Externas:

- Los clientes del sector público piden cumplir el ENS a sus proveedores.
- Reglamento General de Protección de Datos (RGPD) y LOPDGDD.
- Aumento del phishing y del ransomware contra pymes.
- La competencia ya tiene la certificación ISO 27001, y los clientes la piden en los concursos.

## 4. Partes interesadas (4.2)

| Parte interesada | Qué espera |
|---|---|
| Clientes | Que su información se mantenga confidencial y que los informes se entreguen a tiempo |
| Dirección | Conseguir la certificación y no tener incidentes que dañen la imagen |
| Empleados | Tener normas claras y herramientas seguras para trabajar |
| Proveedores (hosting, Microsoft, gestoría) | Requisitos de seguridad claros en los contratos |
| Agencia Española de Protección de Datos | Cumplimiento del RGPD y notificación de brechas |
| Entidad de certificación | Un SGSI conforme con la norma y con evidencias |

## 5. Alcance del SGSI (4.3)

> Los sistemas de información que dan soporte a los servicios de consultoría y auditoría de seguridad de la información que Davem Cyber Consulting presta desde su oficina de Valencia, incluido el trabajo en remoto de su personal y la web corporativa con el área de clientes.

Dentro del alcance:

- Todo el personal de la empresa.
- La oficina de Valencia.
- Portátiles, móviles, red de la oficina y NAS.
- Microsoft 365 y la web corporativa.

Fuera del alcance:

- Los sistemas de los clientes. Se accede a ellos con las condiciones que pone cada cliente.
- La contabilidad y las nóminas, que lleva una gestoría externa. Se controla como proveedor.

## 6. Roles del SGSI

| Rol | Quién | Funciones |
|---|---|---|
| Dirección | Gerente | Aprueba la política, los riesgos y los recursos |
| Responsable de seguridad | Consultor sénior | Mantiene el SGSI, el análisis de riesgos y gestiona los incidentes |
| Administrador de sistemas | Técnico de sistemas | Aplica los controles técnicos |
| Propietarios de activos | Según el inventario | Deciden quién accede a su activo |
| Auditor interno | Persona que no participa en lo auditado | Hace la auditoría interna anual |

## 7. Objetivos de seguridad (6.2)

| Objetivo | Indicador | Meta |
|---|---|---|
| Evitar fugas de información de clientes | Incidentes de confidencialidad al año | 0 |
| Poder recuperar la información | Pruebas de restauración correctas | 2 al año |
| Tener al personal formado | Personal con la formación anual hecha | 100 % |
| Tener los equipos actualizados | Equipos con parches al día | Más del 95 % |
