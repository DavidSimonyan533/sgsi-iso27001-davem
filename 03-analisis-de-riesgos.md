# 03. Análisis y tratamiento de riesgos

## 1. Metodología

He usado una metodología sencilla basada en MAGERIT:

1. Se parte de los activos del inventario con valor 3. También he metido la oficina (A15), que vale 2, porque un incendio o una inundación afectaría a todo lo demás.
2. Para cada uno se buscan las amenazas que le pueden afectar.
3. Se estima la probabilidad y el impacto, teniendo en cuenta lo que ya hay implantado.
4. Riesgo = probabilidad x impacto.
5. Se decide qué hacer con cada riesgo.

Probabilidad:

| Valor | Significado |
|---|---|
| 1 Baja | Puede pasar menos de una vez cada 3 años |
| 2 Media | Puede pasar una vez al año |
| 3 Alta | Puede pasar varias veces al año |

Impacto:

| Valor | Significado |
|---|---|
| 1 Bajo | Molestia interna, sin efecto en clientes |
| 2 Medio | Retraso en un servicio o coste moderado |
| 3 Alto | Fuga de datos de clientes, sanción o parada de varios días |

Nivel de riesgo:

| Riesgo | Nivel | Qué se hace |
|---|---|---|
| 1 - 2 | Bajo | Se acepta |
| 3 - 4 | Medio | Se trata si el coste es razonable |
| 6 - 9 | Alto | Hay que tratarlo |

La dirección ha fijado el criterio de aceptación en 4: todo lo que esté por encima se trata.

Opciones de tratamiento (ISO/IEC 27005:2022): modificar o mitigar (aplicar controles), compartir (seguro o proveedor), evitar (dejar de hacer la actividad) o retener (aceptar).

Cada riesgo tiene un propietario, que es quien aprueba su tratamiento y acepta el riesgo residual.

## 2. Análisis de riesgos

| ID | Activo | Amenaza | Vulnerabilidad | P | I | Riesgo | Nivel |
|---|---|---|---|---|---|---|---|
| R01 | A10 Portátiles | Robo o pérdida de un portátil | Los consultores viajan con los equipos | 2 | 3 | 6 | Alto |
| R02 | A07 Microsoft 365 | Robo de credenciales por phishing | Poca formación y no todos usan doble factor | 3 | 3 | 9 | Alto |
| R03 | A01 Informes de clientes | Envío de un informe a un destinatario equivocado | Se mandan por correo sin cifrar | 2 | 3 | 6 | Alto |
| R04 | A01 Informes de clientes | Ransomware que cifra los documentos | Copias no probadas | 2 | 3 | 6 | Alto |
| R05 | A08 Web y área de clientes | Ataque a la web (inyección SQL, XSS) | No se hacen pruebas de seguridad antes de publicar | 2 | 3 | 6 | Alto |
| R06 | A03 Base de datos de usuarios | Acceso no autorizado a la base de datos | Contraseñas del servidor compartidas | 2 | 3 | 6 | Alto |
| R07 | A09 Servidor virtual | Caída del proveedor de hosting | Un solo proveedor y sin copia fuera | 1 | 2 | 2 | Bajo |
| R08 | A12 NAS | Fallo del disco del NAS | No hay segunda copia fuera de la oficina | 2 | 3 | 6 | Alto |
| R09 | A13 Red | Acceso de un visitante a la red interna | La wifi de invitados no estaba separada | 2 | 2 | 4 | Medio |
| R10 | A07 Microsoft 365 | Un exempleado mantiene el acceso | No hay procedimiento de bajas | 2 | 3 | 6 | Alto |
| R11 | A16 Personal | Baja del administrador de sistemas | Solo una persona conoce la configuración | 2 | 2 | 4 | Medio |
| R12 | A14 Conexión a internet | Corte de internet en la oficina | Una sola línea | 2 | 1 | 2 | Bajo |
| R13 | A17 Gestoría | Fuga de datos de empleados en la gestoría | Contrato sin cláusulas de seguridad | 1 | 3 | 3 | Medio |
| R14 | A06 Datos de empleados | Acceso de personal no autorizado a las nóminas | Permisos de carpetas demasiado amplios | 2 | 2 | 4 | Medio |
| R15 | A15 Oficina | Incendio o inundación en la oficina | Oficina en planta baja | 1 | 3 | 3 | Medio |

## 3. Plan de tratamiento de riesgos

| Riesgo | Propietario del riesgo | Decisión | Acciones | Controles Anexo A | Responsable de la acción | Plazo | Riesgo residual |
|---|---|---|---|---|---|---|---|
| R01 | Dirección | Mitigar | Cifrado de disco en todos los portátiles, bloqueo automático y borrado remoto | 7.9, 8.1, 8.24 | Administrador de sistemas | Hecho | 2 |
| R02 | Responsable de seguridad | Mitigar | Doble factor obligatorio para todos, formación anual y simulacros de phishing | 5.17, 6.3, 8.5 | Responsable de seguridad | Doble factor hecho. Formación: 1 mes | 3 |
| R03 | Responsable de seguridad | Mitigar | Compartir los informes con enlace de SharePoint con caducidad en vez de adjuntos, y clasificar la información | 5.12, 5.13, 5.14 | Responsable de seguridad | 2 meses | 2 |
| R04 | Responsable de seguridad | Mitigar | Antimalware en todos los equipos, copias diarias y pruebas de restauración cada 6 meses | 8.7, 8.13 | Administrador de sistemas | 2 meses | 2 |
| R05 | Administrador de sistemas | Mitigar | Revisión de seguridad antes de cada publicación, actualizaciones y validación de entradas | 8.8, 8.26, 8.28, 8.29 | Administrador de sistemas | 3 meses | 3 |
| R06 | Administrador de sistemas | Mitigar | Cuentas personales en el servidor, acceso por clave SSH y contraseñas con hash en la base de datos | 5.15, 5.18, 8.2, 8.5 | Administrador de sistemas | 1 mes | 2 |
| R07 | Dirección | Aceptar | Riesgo bajo. Se revisa cada año | - | Dirección | - | 2 |
| R08 | Administrador de sistemas | Mitigar | Segunda copia cifrada en la nube (regla 3-2-1) | 8.13, 8.14 | Administrador de sistemas | 1 mes | 2 |
| R09 | Administrador de sistemas | Mitigar | Red de invitados separada de la interna | 8.20, 8.22 | Administrador de sistemas | Hecho | 2 |
| R10 | Responsable de seguridad | Mitigar | Procedimiento de altas y bajas con lista de comprobación y revisión de accesos cada 6 meses | 5.11, 5.16, 5.18, 6.5 | Responsable de seguridad | 1 mes | 2 |
| R11 | Dirección | Mitigar | Documentar la configuración y formar a una segunda persona | 5.37 | Administrador de sistemas | 3 meses | 2 |
| R12 | Dirección | Aceptar | Riesgo bajo. Se puede trabajar desde casa o con el móvil | - | Dirección | - | 2 |
| R13 | Administración | Compartir y mitigar | Firmar contrato de encargado de tratamiento con medidas de seguridad | 5.19, 5.20, 5.34 | Administración | 2 meses | 2 |
| R14 | Administración | Mitigar | Revisar los permisos de SharePoint y dar acceso solo a quien lo necesita | 5.15, 8.3 | Administrador de sistemas | 1 mes | 2 |
| R15 | Dirección | Mitigar y compartir | La información está en la nube y hay copia fuera de la oficina. Seguro de oficina contratado | 7.5 | Dirección | - | 3 |

Cada propietario ha aprobado el tratamiento de sus riesgos y acepta el riesgo residual. La dirección aprueba el plan completo.

El análisis se repite una vez al año y cuando hay cambios importantes (un servicio nuevo, un incidente grave o un cambio de proveedor).
