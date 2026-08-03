# Diseño lógico

## KARDEX ESTUDIANTE
* ke_id_kardex único y obligatorio (PK), númerica
* ke_id_estudiantes FK y proviene de la tabla estudiante, numérica
* ke_semestres, numérico
* ke_id_asignaturas FK y proviene de la tabla asignatura, numérica
* ke_id_profesores, FK proviene de la tabla profesores, numérica
* ke_nota_asignaturas debe ser un decimal , debe estar en el rango de 0 a 5 con dos cifras decimales
* ke_estado_asignaturas, varchar
  ** APROBADA
  ** PENDIENTE
  ** CANCELADA
  ** REPROBADA
  ** EN CURSO

## ESTUDIANTE
e_id_estudiantes, PK, único, numérico
e_id_plan_estudios FK, numérico, viene de la tabla PLAN DE ESTUDIOS
e_fecha_ingreso, DATE
e_genero: AVERIGUAR, varchar
e_colegio: varchar
e_estrato_vivienda_origen: numérico, 1,2,3,4,5,6
e_ciudad_origen VARCHAR
e_estrato_vivienda_residencia: numérico, 1,2,3,4,5,6
e_ciudad_residencia VARCHAR
e_puntaje_saber_11 numérico
e_puntaje_saber_pro numérico
e_beca VARCHAR (nombre de la beca)
e_padres_profesionales BOOLEANO
e_promedio_acumulado, decimales en el rango de 0 a 5
e_promedio_semestre, decimales en el rango de 0 a 5
e_doble_programa, VARCHAR (nombre programa)
e_empresa_practica VARCHAR (nombre empresa)
e_estado VARCHAR: matriculado, retirado, graduado, expulsado

## ASIGNATURA
a_id_asignaturas: numérico, único, PK
a_id_planes_estudio: numérico, FK viene de PLAN DE ESTUDIO
a_nombre_asignaturas: VARCHAR
a_numero_creditos: numérico
a_tipologia: VARCHAR, tronco_común, disciplinar, interdisciplinar,
	           flexibles,  práctica, institucional
a_estado: VARCHAR, vigente o no vigente


