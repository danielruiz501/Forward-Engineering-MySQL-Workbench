# ForwardEngineering en MySQL Workbench

¿Qué es Forward Engineering?
El Forward Engineering es el proceso de generar la base de datos física (tablas, relaciones, índices y
restricciones) en MySQL a partir de un modelo EER diseñado en MySQL Workbench.

Requisitos
1 MySQL Server instalado y en ejecución
2 MySQL Workbench instalado
3 Modelo EER creado o por crear

Paso 1: Crear o abrir un modelo
Abra MySQL Workbench y seleccione File → New Model o abra un modelo existente. Ingrese a Add
Diagram y diseñe sus tablas, columnas y relaciones.

Paso 2: Iniciar Forward Engineering
En el menú superior seleccione Database → Forward Engineer… para iniciar el asistente.

Paso 3: Seleccionar conexión
Seleccione la conexión MySQL donde se creará la base de datos y haga clic en Next. Si no existe una
conexión, créela desde Database → Manage Connections.

Paso 4: Opciones de generación
1 Generate DROP Statements
2 Generate CREATE Statements
3 Generate Foreign Key Constraints
4 Generate Indexes

Paso 5: Revisión del script SQL
Revise el script SQL generado. Puede guardarlo o modificarlo antes de ejecutarlo.

Paso 6: Ejecutar
Presione Execute y espere el mensaje de confirmación. Al finalizar, haga clic en Finish.

Verificación
En el panel Navigator, haga clic derecho en Schemas y seleccione Refresh All para confirmar que las
tablas fueron creadas correctamente.

Errores comunes
1 Access denied: el usuario no tiene permisos suficientes
2 Schema already exists: la base ya existe
3 Foreign key constraint fails: incompatibilidad de tipos de datos o motor


