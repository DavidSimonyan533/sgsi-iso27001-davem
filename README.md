# SGSI de Davem Cyber Consulting (ISO/IEC 27001:2022)

Proyecto de práctica en el que monto la documentación básica de un Sistema de Gestión de Seguridad de la Información (SGSI) para una empresa pequeña, siguiendo la norma ISO/IEC 27001:2022.

La empresa, Davem Cyber Consulting, es ficticia. Es la misma consultora que uso en mi proyecto de la web corporativa del curso de especialización en ciberseguridad. Los datos, personas y hallazgos de la auditoría son inventados para el ejercicio.

## Contenido

| Documento | Qué es | Cláusula ISO 27001 |
|---|---|---|
| [01-contexto-y-alcance.md](01-contexto-y-alcance.md) | Descripción de la empresa, partes interesadas y alcance del SGSI | 4 |
| [02-inventario-de-activos.md](02-inventario-de-activos.md) | Activos de información y su valoración | Control 5.9 |
| [03-analisis-de-riesgos.md](03-analisis-de-riesgos.md) | Metodología, análisis y plan de tratamiento de riesgos | 6.1.2, 6.1.3 y 8 |
| [04-declaracion-de-aplicabilidad.md](04-declaracion-de-aplicabilidad.md) | Los 93 controles del Anexo A con su justificación y estado | 6.1.3 d) |
| [05-politicas/](05-politicas/) | Política de seguridad, control de acceso y copias de seguridad | 5.2 y Anexo A |
| [06-auditoria-interna.md](06-auditoria-interna.md) | Plan, lista de comprobación e informe de auditoría interna | 9.2 |
| [07-revision-por-la-direccion.md](07-revision-por-la-direccion.md) | Revisión por la dirección (pendiente) | 9.3 |

## Cómo está hecho

1. Primero definí la empresa y el alcance.
2. Hice el inventario de activos y valoré cada uno en confidencialidad, integridad y disponibilidad.
3. Con los activos más importantes analicé los riesgos (probabilidad por impacto) y decidí el tratamiento.
4. A partir del tratamiento rellené la Declaración de Aplicabilidad.
5. Redacté tres políticas que salían como necesarias en el análisis.
6. Hice una auditoría interna para comprobar lo anterior.
7. Falta la revisión por la dirección, que iría después de la auditoría.

## Decisiones que tomé

- **Escala de 1 a 3.** Para una empresa de 8 personas, una escala de 1 a 5 daba más trabajo sin aportar mucho. Con 3 niveles es fácil explicar cada valor.
- **Umbral de aceptación en 4.** Así todo lo alto se trata sí o sí, y lo medio lo decido según el coste. Al final traté casi todos los medios porque las acciones eran baratas.
- **Solo activos de valor 3.** Para no hacer un análisis enorme. Hice una excepción con la oficina, porque un incendio afecta a todo.
- **Controles excluidos.** Solo quité 3 (7.6, 8.11 y 8.30), y solo cuando el motivo estaba claro. Es fácil caer en excluir controles para ahorrarse trabajo, y eso un auditor lo ve.
- **La auditoría la hice yo.** En una empresa real no valdría, porque no se puede auditar lo que has montado tú. Por eso en la SoA el control 5.35 está como parcial.

## Lo que aprendí

- Lo importante no es tener muchos documentos, sino que estén conectados: cada control de la SoA tiene que salir de un riesgo, y cada riesgo de un activo.
- La auditoría sirve de verdad. Encontró cosas que yo daba por hechas, como las pruebas de restauración, que estaban en la política pero nadie las había hecho.
- Hay detalles de la norma que se pasan fácil: los propietarios del riesgo, las interfaces y dependencias del alcance o que los objetivos necesiten un plan y no solo una meta.

## Uso de IA

He usado IA como apoyo para revisar el proyecto contra la norma y corregir algunos fallos (propietarios del riesgo, objetivos, coherencia entre documentos) y para ayudarme a redactar algunas partes. Las decisiones y el planteamiento del SGSI son míos.

## Referencias

- ISO/IEC 27001:2022 e ISO/IEC 27002:2022
- MAGERIT v3 (para el catálogo de amenazas)
- Guías CCN-STIC del Esquema Nacional de Seguridad

Autor: David Simonyan Demchuk
