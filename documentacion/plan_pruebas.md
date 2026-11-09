# Plan de pruebas del sistema de gestión de tareas
Se construira un documento desde la perspectiva de un equipo encargado de garantizar la calidasd del software.

## Objetivo del plan
El objetivo es establecer una estrategia de pruebas que permita verificar el correcto funcionamiento del Sistema de Gestión de Tareas de la empresa Plásticos Sustentables, comprobando que sus funcionalidades respondan a los requisitos establecidos y que los permisos asignados a cada tipo de usuario se respeten.
Se busca identificar errores, validar la integridad de la información, comprobar la seguridad en el acceso a las funcionalidades y garantizar que el sistema satisfaga las necesidades del administrador y de los colaboradores.

## Alcance de las pruebas
las pruebas estarán planteadas para los siguientes modulos.
  Autenticación y administración de usuarios.
  Administración de perfiles y contraseñas.
  Creación y administración de colaboradores.
  Creación y asignación de tareas.
  Consulta y seguimiento de tareas.
  Actualización de estados de las tareas.
  Control de permisos según el rol del usuario.

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



