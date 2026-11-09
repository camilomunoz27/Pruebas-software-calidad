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
Funcionalidad	                             Administrador	              Colaborador
Iniciar sesión	                                Sí	                        Sí
Crear cuenta	                          Proceso restringido	        Mediante administrador
Editar perfil propio	                          Sí	                        Sí
Cambiar contraseña propia	                      Sí	                        Sí
Crear colaboradores	                            Sí	                        No
Desactivar colaboradores	                      Sí	                        No
Crear tareas	                                  Sí	                        No
Asignar tareas	                                Sí	                        No
Consultar todas las tareas	                    Sí	                        Sí
Modificar tareas	                              Sí	             Solo las asignadas, según permisos
Cambiar estado a ejecución o desarrollada	      Sí	                  Solo las asignadas
Cancelar tareas	                                Sí	                        No
Eliminar tareas	                        Sí, según autorización	            No

