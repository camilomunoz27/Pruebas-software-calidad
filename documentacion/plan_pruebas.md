# Plan de pruebas del sistema de gestión de tareas
Se construira un documento desde la perspectiva de un equipo encargado de garantizar la calidasd del software.

## Objetivo del plan
El objetivo es establecer una estrategia de pruebas que permita verificar el correcto funcionamiento del Sistema de Gestión de Tareas de la empresa Plásticos Sustentables, comprobando que sus funcionalidades respondan a los requisitos establecidos y que los permisos asignados a cada tipo de usuario se respeten.
Se busca identificar errores, validar la integridad de la información, comprobar la seguridad en el acceso a las funcionalidades y garantizar que el sistema satisfaga las necesidades del administrador y de los colaboradores.

## Alcance de las pruebas
las pruebas estarán planteadas para los siguientes modulos.
- Autenticación y administración de usuarios.
- Administración de perfiles y contraseñas.
- Creación y administración de colaboradores.
- Creación y asignación de tareas.
- Consulta y seguimiento de tareas.
- Actualización de estados de las tareas.
- Control de permisos según el rol del usuario.

## Roles y permisos
Se identificaran dos roles, los cuales son los que interactuaran con el sistema, pero cada uno de ellos tendrá sus respectivos permisos y tendrán funcionalidades independientes a las que podrán acceder.
### Roles
Administrador y Colaborador
### Funcionalidades
Iniciar sesión,   
Crear cuenta,
Editar perfil propio,
Cambiar contraseña propia,
Crear colaboradores,
Desactivar colaboradores,
Crear tareas,
Asignar tareas,
Consultar todas las tareas,
Modificar tareas,
Cambiar estado a ejecución o desarrollada,
Cancelar tareas,
Eliminar tareas.


# Estrategia para el desarrollo de las pruebas
La estrategia establece cómo vamos a comprobar que el sistema cumple los requisitos. Para ello, utilizaremos pruebas manuales y automatizadas, apoyándonos en GitHub para organizar la documentación y registrar los defectos encontrados.

## Pruebas manuales
Son aquellas que ejecuta una persona siguiendo una serie de pasos previamente definidos. El responsable introduce datos, interactúa con el sistema y compara el resultado obtenido con el resultado esperado.
En nuestro proyecto se utilizarán principalmente para:
- Comprobar el inicio de sesión con credenciales válidas e inválidas.
- Verificar la creación y administración de colaboradores.
- Comprobar que el administrador pueda crear y asignar tareas.
- Verificar que los colaboradores consulten todas las tareas, pero solo puedan modificar el estado de las que tienen asignadas.
- Comprobar que un colaborador no pueda cancelar tareas.
- Evaluar que los mensajes de error sean comprensibles.
- Comprobar que la navegación y las funcionalidades sean fáciles de utilizar.

## Pruebas automatizadas
Son aquellas que se ejecutan mediante programas o herramientas especializadas que verifican automáticamente si el comportamiento del sistema coincide con los resultados esperados.
Para este proyecto se propone utilizar Python y pytest como herramientas de apoyo.
Se podrían automatizar comprobaciones como:
- Validar que no se permita crear tareas sin información obligatoria.
- Comprobar que una tarea se asigne al colaborador seleccionado.
- Verificar que un colaborador no pueda modificar tareas ajenas.
- Comprobar que las transiciones entre estados sean válidas.
- Validar que una contraseña no cumpla los requisitos establecidos.
Es importante aclarar que estas son pruebas propuestas. Para ejecutarlas sobre el sistema real sería necesario disponer de sus componentes de software. Los ejercicios que estamos realizando con Python son una práctica de aprendizaje, no evidencias de que el sistema de Plásticos Sustentables ya haya sido probado.

## Nivel de pruebas
Además de distinguir entre pruebas manuales y automatizadas, debemos definir los niveles en los que se evaluará el software.
- Unitarias:	Verificar funciones individuales, como validar una contraseña o cambiar el estado de una tarea.
- Integración:	Comprobar la comunicación entre usuarios, tareas, asignaciones y permisos.
- Aceptación:	Verificar que el sistema satisfaga las necesidades del administrador y los colaboradores.


# Herramientas de apoyo
La herramienta seleccionada para organizar el proyecto es GitHub.
Se utilizara para:
- Almacenar la documentación del plan de pruebas.
- Mantener los casos de prueba organizados.
- Registrar errores o defectos mediante GitHub Issues.
- Llevar un seguimiento de las actividades pendientes.
- Conservar el historial de cambios de los documentos.

Como complemento, se propone utilizar:
- Python: lenguaje para desarrollar pequeños componentes de prueba.
- pytest: herramienta para ejecutar las pruebas automatizadas.
- GitHub Actions: servicio que, si se configura posteriormente, permitirá ejecutar automáticamente las pruebas cuando se realicen cambios en el repositorio.


# Registro y clasificación de defectos
Cuando una prueba identifique un comportamiento incorrecto, se deberá documentar el defecto para facilitar su análisis y posterior corrección.

Cada reporte debería contener:
- Identificador:	Código único del defecto.
- Título:	Descripción breve del problema.
- Funcionalidad:	Módulo donde se encontró.
- Pasos para reproducirlo:	Acciones necesarias para generar el error.
- Resultado esperado:	Comportamiento correcto.
- Resultado obtenido:	Comportamiento observado.
- Prioridad:	Nivel de atención requerido.
- Estado:	Abierto, en revisión, corregido o cerrado.


# Ventajas y desventajas del plan propuesto

## Ventajas
- Permite identificar errores antes de que afecten a los usuarios.
- Verifica que los permisos de administradores y colaboradores se respeten.
- Reduce el riesgo de asignaciones incorrectas y pérdida de información.
- Facilita la identificación y documentación de defectos.
- Permite repetir las pruebas después de corregir errores.
## Desventajas
- Las pruebas manuales requieren tiempo y personal encargado de ejecutarlas.
- Las pruebas automatizadas requieren conocimientos de programación y mantenimiento del código de prueba.
- Para ejecutar pruebas completas se necesita disponer de una aplicación funcional.
- Los resultados dependen de que los casos de prueba estén bien diseñados y actualizados.
- Algunas características, como la usabilidad, requieren evaluación humana y no se pueden comprobar únicamente mediante pruebas automatizadas.


# Organización del proceso de pruebas

1. Análisis de requisitos: Identificar las funcionalidades del sistema, los roles de usuario y sus respectivos permisos.
2. Diseño de casos de prueba: Definir escenarios, datos de entrada, resultados esperados y prioridades.
3. Preparación de pruebas: Establecer los datos de prueba, el entorno y las herramientas que se utilizarán.
4. Ejecución de pruebas: Realizar las pruebas manuales y automatizadas, registrando los resultados obtenidos.
5. Documentación y seguimiento: Registrar defectos, verificar sus correcciones y elaborar el informe final.

