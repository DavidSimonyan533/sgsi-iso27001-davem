# Política de copias de seguridad

| | |
|---|---|
| Versión | 1.0 |
| Aprobada por | Dirección |
| Fecha | Noviembre de 2026 |
| Revisión | Anual |
| Controles relacionados | 8.13, 8.14, 5.30 |

## 1. Objetivo

Poder recuperar la información y los sistemas después de un borrado, una avería o un ataque de ransomware.

## 2. Qué se copia

| Información | Frecuencia | Dónde | Cuánto se guarda |
|---|---|---|---|
| SharePoint y OneDrive | Diaria | NAS de la oficina | 30 días |
| Buzones de correo | Diaria | NAS de la oficina | 30 días |
| Base de datos de la web | Diaria | NAS y nube | 30 días |
| Código y configuración de la web | En cada cambio | Repositorio Git y nube | Siempre |
| Copia completa del NAS | Semanal | Nube, cifrada | 3 meses |

## 3. Regla 3-2-1

Se mantienen 3 copias de la información, en 2 soportes distintos y 1 fuera de la oficina.

## 4. Protección de las copias

- Las copias que salen de la oficina van cifradas.
- Al NAS solo accede el administrador de sistemas con una cuenta distinta a la de uso diario.
- El NAS está en el armario de comunicaciones cerrado con llave.

## 5. Pruebas de restauración

- Cada 6 meses se restaura una carpeta de SharePoint y la base de datos de la web en un entorno de pruebas.
- Se anota la fecha, lo que se restauró, el tiempo que se tardó y si salió bien.

## 6. Tiempos objetivo

| | Objetivo |
|---|---|
| Pérdida máxima de datos (RPO) | 24 horas |
| Tiempo máximo de recuperación (RTO) | 48 horas |

## 7. Responsables

- Administrador de sistemas: configura las copias, revisa cada semana que se han hecho y hace las pruebas de restauración.
- Responsable de seguridad: comprueba que las pruebas se hacen y guarda los registros.
