# 04. Declaración de Aplicabilidad (SoA)

Lista de los 93 controles del Anexo A de ISO/IEC 27001:2022. Para cada uno se indica si aplica, por qué y cómo está.

| | |
|---|---|
| Versión | 1.0 |
| Fecha | Noviembre de 2026 |
| Aprobada por | Dirección |

Estados: Implantado, Parcial (está en marcha pero le falta algo) y Pendiente (previsto en el plan de tratamiento).

## Resumen

| | Controles |
|---|---|
| Aplican | 90 |
| No aplican | 3 |
| Implantados | 48 |
| Parciales | 38 |
| Pendientes | 4 |

## 5. Controles organizativos

| Control | Nombre | Aplica | Justificación | Estado |
|---|---|---|---|---|
| 5.1 | Políticas de seguridad de la información | Sí | Requisito de la norma. Política aprobada por dirección | Implantado |
| 5.2 | Roles y responsabilidades de seguridad | Sí | Definidos en el documento 01 | Implantado |
| 5.3 | Segregación de funciones | Sí | Empresa pequeña: se separa quien pide un acceso de quien lo da | Parcial |
| 5.4 | Responsabilidades de la dirección | Sí | La dirección exige cumplir la política | Implantado |
| 5.5 | Contacto con las autoridades | Sí | Obligación de notificar brechas a la AEPD e INCIBE-CERT | Implantado |
| 5.6 | Contacto con grupos de interés especial | Sí | Suscripción a avisos de INCIBE y CCN-CERT | Implantado |
| 5.7 | Inteligencia de amenazas | Sí | Se revisan los avisos de INCIBE y CCN-CERT cada semana | Parcial |
| 5.8 | Seguridad en la gestión de proyectos | Sí | Los proyectos manejan información confidencial de clientes | Parcial |
| 5.9 | Inventario de información y otros activos | Sí | Base del análisis de riesgos. Documento 02 | Implantado |
| 5.10 | Uso aceptable de la información y los activos | Sí | Riesgo R01. Normas de uso firmadas por el personal | Implantado |
| 5.11 | Devolución de activos | Sí | Riesgo R10. Incluido en el procedimiento de bajas | Parcial |
| 5.12 | Clasificación de la información | Sí | Riesgo R03. Niveles: pública, interna y confidencial | Parcial |
| 5.13 | Etiquetado de la información | Sí | Riesgo R03. Etiquetas de sensibilidad de Microsoft 365 | Pendiente |
| 5.14 | Transferencia de información | Sí | Riesgo R03. Informes por enlace con caducidad | Parcial |
| 5.15 | Control de acceso | Sí | Riesgos R06 y R14. Política de control de acceso | Implantado |
| 5.16 | Gestión de identidades | Sí | Riesgo R10. Cuentas personales | Implantado |
| 5.17 | Información de autenticación | Sí | Riesgo R02. Gestor de contraseñas y normas de contraseñas | Implantado |
| 5.18 | Derechos de acceso | Sí | Riesgos R06 y R10. Revisión cada 6 meses | Parcial |
| 5.19 | Seguridad en las relaciones con proveedores | Sí | Riesgo R13. Hosting, Microsoft y gestoría | Parcial |
| 5.20 | Seguridad en los acuerdos con proveedores | Sí | Riesgo R13. Falta el anexo con la gestoría | Parcial |
| 5.21 | Seguridad en la cadena de suministro TIC | Sí | Se usan servicios en la nube de terceros | Parcial |
| 5.22 | Seguimiento y revisión de servicios de proveedores | Sí | Revisión anual de los proveedores críticos | Pendiente |
| 5.23 | Seguridad en el uso de servicios en la nube | Sí | Microsoft 365 y hosting son servicios en la nube | Parcial |
| 5.24 | Planificación de la gestión de incidentes | Sí | Procedimiento de incidentes | Implantado |
| 5.25 | Evaluación de eventos de seguridad | Sí | El responsable de seguridad clasifica los eventos | Implantado |
| 5.26 | Respuesta a incidentes | Sí | Procedimiento de incidentes | Implantado |
| 5.27 | Aprendizaje de los incidentes | Sí | Se revisa cada incidente al cerrarlo | Parcial |
| 5.28 | Recopilación de evidencias | Sí | Necesario si hay que denunciar o notificar | Parcial |
| 5.29 | Seguridad durante una interrupción | Sí | Riesgos R07 y R15 | Parcial |
| 5.30 | Preparación de las TIC para la continuidad | Sí | Riesgos R04 y R08. RPO y RTO definidos | Parcial |
| 5.31 | Requisitos legales, reglamentarios y contractuales | Sí | RGPD, LOPDGDD, LSSI y contratos con clientes | Implantado |
| 5.32 | Derechos de propiedad intelectual | Sí | Solo se usa software con licencia | Implantado |
| 5.33 | Protección de los registros | Sí | Contratos e informes se conservan según contrato | Parcial |
| 5.34 | Privacidad y protección de datos personales | Sí | Riesgo R13. Se tratan datos de clientes y empleados | Implantado |
| 5.35 | Revisión independiente de la seguridad | Sí | Auditoría interna anual (documento 06). Falta que la haga alguien independiente | Parcial |
| 5.36 | Cumplimiento de políticas y normas | Sí | Se comprueba en la auditoría interna | Implantado |
| 5.37 | Procedimientos operativos documentados | Sí | Riesgo R11. Falta documentar la configuración | Parcial |

## 6. Controles de personas

| Control | Nombre | Aplica | Justificación | Estado |
|---|---|---|---|---|
| 6.1 | Comprobación de antecedentes | Sí | Se comprueban referencias y titulación al contratar | Implantado |
| 6.2 | Términos y condiciones de contratación | Sí | El contrato incluye obligaciones de seguridad | Implantado |
| 6.3 | Concienciación, educación y formación | Sí | Riesgo R02. Formación al entrar y anual | Parcial |
| 6.4 | Proceso disciplinario | Sí | Recogido en la política de seguridad | Implantado |
| 6.5 | Responsabilidades tras el cese o cambio de puesto | Sí | Riesgo R10. La confidencialidad sigue tras la baja | Implantado |
| 6.6 | Acuerdos de confidencialidad | Sí | Firmados por todo el personal y colaboradores | Implantado |
| 6.7 | Teletrabajo | Sí | Los consultores trabajan en remoto | Parcial |
| 6.8 | Notificación de eventos de seguridad | Sí | Aviso el mismo día al responsable de seguridad | Implantado |

## 7. Controles físicos

| Control | Nombre | Aplica | Justificación | Estado |
|---|---|---|---|---|
| 7.1 | Perímetros de seguridad física | Sí | Oficina con puerta de seguridad y alarma | Implantado |
| 7.2 | Controles físicos de entrada | Sí | Llave por empleado y visitas acompañadas | Implantado |
| 7.3 | Seguridad de oficinas, despachos e instalaciones | Sí | Armario de comunicaciones cerrado con llave | Implantado |
| 7.4 | Monitorización de la seguridad física | Sí | Alarma conectada a central | Implantado |
| 7.5 | Protección contra amenazas físicas y ambientales | Sí | Riesgo R15. Extintores y seguro | Implantado |
| 7.6 | Trabajo en áreas seguras | No | No hay CPD ni áreas seguras. Los servidores están en proveedores | - |
| 7.7 | Puesto de trabajo despejado y pantalla limpia | Sí | Hay visitas de clientes en la oficina | Parcial |
| 7.8 | Emplazamiento y protección de equipos | Sí | NAS y router en el armario cerrado | Implantado |
| 7.9 | Seguridad de los activos fuera de las instalaciones | Sí | Riesgo R01. Portátiles y móviles salen de la oficina | Implantado |
| 7.10 | Soportes de almacenamiento | Sí | Uso de USB limitado y cifrado | Parcial |
| 7.11 | Servicios de suministro | Sí | SAI para el NAS y el router | Implantado |
| 7.12 | Seguridad del cableado | Sí | Cableado de red dentro de canaletas y armario | Implantado |
| 7.13 | Mantenimiento de los equipos | Sí | Garantía y mantenimiento de portátiles y NAS | Implantado |
| 7.14 | Eliminación o reutilización segura de equipos | Sí | Borrado seguro antes de reutilizar o tirar un equipo | Parcial |

## 8. Controles tecnológicos

| Control | Nombre | Aplica | Justificación | Estado |
|---|---|---|---|---|
| 8.1 | Dispositivos de usuario | Sí | Riesgo R01. Cifrado, bloqueo y borrado remoto | Implantado |
| 8.2 | Derechos de acceso privilegiado | Sí | Riesgo R06. Cuentas de administrador separadas | Implantado |
| 8.3 | Restricción del acceso a la información | Sí | Riesgo R14. Permisos por grupos en SharePoint | Parcial |
| 8.4 | Acceso al código fuente | Sí | El código de la web está en un repositorio privado | Implantado |
| 8.5 | Autenticación segura | Sí | Riesgos R02 y R06. Doble factor | Implantado |
| 8.6 | Gestión de la capacidad | Sí | Se vigila el espacio del NAS y del servidor | Parcial |
| 8.7 | Protección contra el malware | Sí | Riesgo R04. Antimalware en todos los equipos | Implantado |
| 8.8 | Gestión de vulnerabilidades técnicas | Sí | Riesgo R05. Actualizaciones automáticas y revisión mensual | Parcial |
| 8.9 | Gestión de la configuración | Sí | Configuración de la web en ficheros versionados | Parcial |
| 8.10 | Borrado de información | Sí | Se borra la información del cliente al acabar el plazo del contrato | Parcial |
| 8.11 | Enmascaramiento de datos | No | No se usan datos reales fuera de producción ni se muestran datos sensibles a terceros | - |
| 8.12 | Prevención de fuga de datos | Sí | Riesgo R03. Reglas básicas de Microsoft 365 | Pendiente |
| 8.13 | Copias de seguridad | Sí | Riesgos R04 y R08. Política de copias | Parcial |
| 8.14 | Redundancia de los recursos | Sí | Riesgo R08. Segunda copia en la nube | Parcial |
| 8.15 | Registro de eventos | Sí | Registros de Microsoft 365 y del servidor web | Parcial |
| 8.16 | Actividades de monitorización | Sí | Alertas de inicio de sesión sospechoso en Microsoft 365 | Parcial |
| 8.17 | Sincronización de relojes | Sí | Equipos y servidor sincronizados por NTP | Implantado |
| 8.18 | Uso de programas de utilidad con privilegios | Sí | Solo el administrador puede instalarlos | Implantado |
| 8.19 | Instalación de software en sistemas en producción | Sí | Los usuarios no tienen permisos de administrador | Implantado |
| 8.20 | Seguridad de redes | Sí | Riesgo R09. Cortafuegos y wifi con WPA3 | Implantado |
| 8.21 | Seguridad de los servicios de red | Sí | Servicios contratados con el operador y el hosting | Implantado |
| 8.22 | Segregación de redes | Sí | Riesgo R09. Red de invitados separada | Implantado |
| 8.23 | Filtrado web | Sí | Filtrado por DNS de sitios maliciosos | Parcial |
| 8.24 | Uso de la criptografía | Sí | Riesgo R01. Cifrado de discos, HTTPS y copias cifradas | Implantado |
| 8.25 | Ciclo de vida de desarrollo seguro | Sí | Riesgo R05. La web se desarrolla internamente | Parcial |
| 8.26 | Requisitos de seguridad de las aplicaciones | Sí | Riesgo R05. Área de clientes con inicio de sesión | Parcial |
| 8.27 | Arquitectura segura y principios de ingeniería | Sí | Web separada en contenedores | Parcial |
| 8.28 | Codificación segura | Sí | Riesgo R05. Validación de entradas y consultas preparadas | Parcial |
| 8.29 | Pruebas de seguridad en desarrollo y aceptación | Sí | Riesgo R05. Revisión antes de publicar | Pendiente |
| 8.30 | Desarrollo externalizado | No | No se encarga desarrollo a terceros | - |
| 8.31 | Separación de entornos | Sí | Entorno de pruebas en local y producción en el servidor | Implantado |
| 8.32 | Gestión de cambios | Sí | Los cambios de la web pasan por el repositorio | Parcial |
| 8.33 | Información de pruebas | Sí | Las pruebas se hacen con datos inventados | Implantado |
| 8.34 | Protección de los sistemas durante las auditorías | Sí | Las pruebas técnicas se planifican con el administrador | Implantado |

## Controles excluidos

| Control | Motivo |
|---|---|
| 7.6 Trabajo en áreas seguras | No hay CPD ni áreas seguras. Los servidores están en proveedores |
| 8.11 Enmascaramiento de datos | No se usan datos reales fuera de producción ni se muestran datos sensibles a terceros |
| 8.30 Desarrollo externalizado | No se encarga desarrollo a terceros |
