# 06. Auditoría interna del SGSI

## 1. Plan de auditoría

| | |
|---|---|
| Objetivo | Comprobar que el SGSI cumple la norma ISO/IEC 27001:2022 y lo que dice la propia documentación |
| Alcance | El alcance del SGSI (ver documento 01) |
| Criterios | ISO/IEC 27001:2022, políticas internas y Declaración de Aplicabilidad |
| Duración | 2 jornadas |
| Auditor | David Simonyan Demchuk |
| Método | Revisión de documentos, entrevistas y comprobaciones en los sistemas por muestreo |

En una empresa real el auditor interno no puede haber participado en montar lo que audita. Aquí la hago yo porque es un ejercicio.

Agenda:

| Día | Qué se revisa | Con quién |
|---|---|---|
| Día 1, mañana | Contexto, alcance, política y objetivos (cláusulas 4, 5 y 6) | Dirección y responsable de seguridad |
| Día 1, tarde | Análisis de riesgos y Declaración de Aplicabilidad (6.1 y 8) | Responsable de seguridad |
| Día 2, mañana | Controles técnicos: accesos, copias, equipos y red | Administrador de sistemas |
| Día 2, tarde | Personal, proveedores, incidentes y reunión de cierre | Administración y dirección |

## 2. Lista de comprobación

| N.º | Requisito | Qué se comprueba | Evidencia | Resultado |
|---|---|---|---|---|
| 1 | 4.3 | El alcance está documentado | Documento 01 | Conforme |
| 2 | 5.2 | La política está aprobada y el personal la conoce | Política v1.0 y entrevista a 3 empleados | Conforme |
| 3 | 6.1.2 | Hay metodología de riesgos y se ha aplicado | Documento 03 | Conforme |
| 4 | 6.1.3 | Existe la Declaración de Aplicabilidad con justificaciones | Documento 04 | Conforme |
| 5 | 6.2 | Los objetivos tienen indicador y se miden | Documento 01 | Observación |
| 6 | 7.2 y A.6.3 | El personal ha hecho la formación anual | Registro de formación | No conforme |
| 7 | A.5.9 | El inventario está actualizado | Documento 02 y revisión de 4 equipos | Conforme |
| 8 | A.5.18 | Se revisan los accesos cada 6 meses | Listado de usuarios de Microsoft 365 | Observación |
| 9 | A.8.5 | Doble factor activado en todas las cuentas | Panel de Microsoft 365 | Conforme |
| 10 | A.8.13 | Las copias se hacen y se prueban | Registros del NAS y de las pruebas | No conforme |
| 11 | A.8.1 y A.8.24 | Portátiles con disco cifrado | Comprobación en 4 portátiles | Conforme |
| 12 | A.8.22 | La red de invitados está separada | Configuración del router | Conforme |
| 13 | A.5.19 y A.5.20 | Contratos con proveedores con cláusulas de seguridad | Contratos del hosting y la gestoría | Observación |
| 14 | A.5.24 | Hay procedimiento de incidentes y registro | Registro de incidentes | Conforme |
| 15 | 9.3 | Está planificada la revisión por la dirección | Convocatoria de la reunión | Conforme. Se hará después de esta auditoría, con sus resultados |

## 3. Informe de auditoría

### 3.1 Resumen

El SGSI está bien planteado para el tamaño de la empresa. La documentación principal existe y el personal conoce la política. Se han encontrado 2 no conformidades menores, 3 observaciones y 1 oportunidad de mejora. No hay no conformidades mayores.

| Tipo | Cantidad |
|---|---|
| No conformidad mayor | 0 |
| No conformidad menor | 2 |
| Observación | 3 |
| Oportunidad de mejora | 1 |

### 3.2 Puntos fuertes

- Doble factor activado en las 8 cuentas.
- Todos los portátiles revisados tienen el disco cifrado.
- El análisis de riesgos está relacionado con el inventario y con la Declaración de Aplicabilidad.

### 3.3 Hallazgos

**NC-01. No conformidad menor. Formación (7.2 y control 6.3)**

- Qué se ha visto: 2 de las 8 personas no han hecho la formación anual de seguridad. Las dos entraron en la empresa en septiembre.
- Qué se incumple: la política dice que todo el personal recibe formación al entrar.
- Acción propuesta: hacer la formación a las 2 personas y añadirla a la lista de comprobación de altas.

**NC-02. No conformidad menor. Copias de seguridad (control 8.13)**

- Qué se ha visto: las copias se hacen cada día, pero no hay registro de ninguna prueba de restauración.
- Qué se incumple: la política de copias pide una prueba cada 6 meses con registro.
- Acción propuesta: hacer una prueba de restauración, registrarla y ponerla en el calendario.

**OBS-01. Observación. Objetivos (6.2)**

El objetivo de equipos actualizados tiene meta, pero no se ha medido todavía.

**OBS-02. Observación. Revisión de accesos (control 5.18)**

La revisión de accesos se hizo, pero no quedó por escrito quién la hizo ni qué se cambió.

**OBS-03. Observación. Proveedores (controles 5.19 y 5.20)**

El contrato con la gestoría no tiene todavía el anexo de encargado de tratamiento. Está previsto en el plan de tratamiento (riesgo R13) y dentro de plazo.

**OM-01. Oportunidad de mejora**

Hacer un simulacro de phishing al año para medir si la formación funciona.

### 3.4 Plan de acciones correctivas

| Hallazgo | Causa | Acción | Responsable | Plazo | Estado |
|---|---|---|---|---|---|
| NC-01 | La formación no estaba en el proceso de alta | Formar a las 2 personas y cambiar la lista de altas | Responsable de seguridad | 15 días | Abierta |
| NC-02 | No había fecha fijada ni responsable de la prueba | Hacer la prueba, registrarla y programarla cada 6 meses | Administrador de sistemas | 30 días | Abierta |
| OBS-01 | No se había definido cómo medirlo | Sacar el informe de actualizaciones cada mes | Administrador de sistemas | 30 días | Abierta |
| OBS-02 | No había plantilla para la revisión | Crear una plantilla de registro | Responsable de seguridad | 30 días | Abierta |
| OBS-03 | Contrato anterior al SGSI | Firmar el anexo con la gestoría | Administración | 2 meses | Abierta |

### 3.5 Conclusión

El SGSI es adecuado y está en funcionamiento. Las no conformidades son menores y tienen acción correctiva. Se comprobará su cierre en un seguimiento dentro de 2 meses.
