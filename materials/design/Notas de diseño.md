# Diseño lógico

## KARDEX ESTUDIANTE

| Campo | Tipo | Descripción |
|---|---|---|
| `ke_id_kardex` | Numérico | PK, único y obligatorio |
| `ke_id_estudiantes` | Numérico | FK → tabla `ESTUDIANTE` |
| `ke_semestres` | Numérico | |
| `ke_id_asignaturas` | Numérico | FK → tabla `ASIGNATURA` |
| `ke_id_profesores` | Numérico | FK → tabla `PROFESORES` |
| `ke_nota_asignaturas` | Decimal | Rango 0 a 5, dos cifras decimales |
| `ke_estado_asignaturas` | Varchar | `APROBADA`, `PENDIENTE`, `CANCELADA`, `REPROBADA`, `EN CURSO` |

## ESTUDIANTE

| Campo | Tipo | Descripción |
|---|---|---|
| `e_id_estudiantes` | Numérico | PK, único |
| `e_id_plan_estudios` | Numérico | FK → tabla `PLAN DE ESTUDIOS` |
| `e_fecha_ingreso` | Date | |
| `e_genero` | Varchar | Averiguar |
| `e_colegio` | Varchar | |
| `e_estrato_vivienda_origen` | Numérico | 1, 2, 3, 4, 5, 6 |
| `e_ciudad_origen` | Varchar | |
| `e_estrato_vivienda_residencia` | Numérico | 1, 2, 3, 4, 5, 6 |
| `e_ciudad_residencia` | Varchar | |
| `e_puntaje_saber_11` | Numérico | |
| `e_puntaje_saber_pro` | Numérico | |
| `e_beca` | Varchar | Nombre de la beca |
| `e_padres_profesionales` | Booleano | |
| `e_promedio_acumulado` | Decimal | Rango 0 a 5 |
| `e_promedio_semestre` | Decimal | Rango 0 a 5 |
| `e_doble_programa` | Numérico | FK → tabla `PROGRAMAS`  |
| `e_empresa_practica` | Varchar | Nombre de la empresa |
| `e_estado` | Varchar | `matriculado`, `retirado`, `graduado`, `expulsado` |

## ASIGNATURA

| Campo | Tipo | Descripción |
|---|---|---|
| `a_id_asignaturas` | Numérico | PK, único |
| `a_id_planes_estudio` | Numérico | FK → tabla `PLAN DE ESTUDIO` |
| `a_nombre_asignaturas` | Varchar | |
| `a_numero_creditos` | Numérico | |
| `a_tipologia` | Varchar | `tronco_común`, `disciplinar`, `interdisciplinar`, `flexibles`, `práctica`, `institucional` |
| `a_estado` | Varchar | `vigente` o `no vigente` |
