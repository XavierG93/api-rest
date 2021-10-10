# api-rest
Un api-rest para un geriátrico, parte del proyecto de final de ciclo, se estableció control sobre los usuarios, sus datos, sus roles dentro del geriátrico también sobre actividades, cuidados y los residentes.
Se establecieron las entidades:
  - Usuarios: profesionales y administrador que se registran en la aplicación.
  - Roles: roles asignados a los usuarios.
  - Privilegios: que irían asignados a los roles y permitirían desbloquear funciones en la aplicación.
  - Actividades: actividades que realizarían los residentes, tendrían un registro y observación sobre cada paciente.
  - Atenciones: cuidados recibidos por los pacientes, también con espacio para observaciones.
  - Residentes: los residentes del geriátrico, con sus datos asociados.

Después, por la relación  entre  clases, se harían dos entidades; ActivitiesResidents y AttentionsResidents, que enlazarían la clase residente con las clases de actividades y atenciones, así guardando la observación en relación al residente dentro de la actividad o cuidado que llevara a cabo.
Una vez establecida la base, se añaden los controladores para ofrecer una vigilancia sobre los datos introducidos, no se admitían repeticiones de según que atributos de las entidades. También se estableció un sistema de registro y login con el cual se ofrecía acceso solo a las operaciones asignadas a los privilegios de los roles.
Por último también se añadieron dependencias para hacer test unitarios.


