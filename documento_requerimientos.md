<H1>DOCUMENTO DE DEFINICIÓN DE REQUERIMIENTOS</H1>  :rocket:



<H3>PROPÓSITO:</H3>

<P><br>El objetivo de este documento es describir los <strong>requerimientos funcionales</strong>y <strong>no funcionales</strong> de un <strong>sistema de gestión de reclamos y reparación de baches</strong>, basado en los elementos definidos en el modelo UML.<br>Se busca formalizar el proceso desde que un usuario reporta un reclamo hasta la intervención de una cuadrilla mediante una orden de trabajo y su respectiva reparación.<br></P>

<H3>FONDO:</H3>

<P>Cuando se reportan los baches en la ciudad de Bahía Blanca, se registran en <strong>sistema de reparación</strong> del <strong>departamento de obras públicas</strong> y se les asigna un <strong>número de identificación</strong>, almacenado según la <strong>calle</strong>, <strong>tamaño</strong> (en una escala de 1 a 10), <strong>ubicación</strong> (en medio, cuneta, etc.), <strong>distrito</strong> (se determina con la dirección en la calle) y <strong>prioridad de reparación</strong> (determinada por el tamaño del bache).</P>

</P>El sistema de registros de baches se realiza mediante registros manuales, hojas de cálculos y planillas. Al utilizar herramientas físicas, observamos <strong>pérdidas de información</strong>, <strong>falta de control</strong>, <strong>tareas duplicadas</strong>, <strong>registros de información incompleta</strong>, <strong>poca claridad</strong> y <strong>confiabilidad</strong>. <br>Es necesario un sistema digital que <strong>organice este registro</strong> para así poder darle un seguimiento a la solución del problema.</P>

<H3>ALCANCE</H3>

<P><strong>· Recepción de reclamos:</strong> Un usuario realiza un reclamo, el cual se asocia a un bache determinado. El reclamo contiene la descripción del problema.<br><strong>· Gestión del bache:</strong> Un bache se vincula a uno o más reclamos. Se registran datos como ubicación, descripción y observaciones. El bache es inspeccionado por un inspector.<br><strong>· Asignación de inspecciones:</strong> El inspector evalúa el bache, generando observaciones sobre el mismo.<br><strong>· Generación de órdenes de trabajo:</strong> Una vez inspeccionado, el bache puede generar una orden de trabajo. La orden de trabajo contiene la fecha de asignación y se relaciona con el bache.<br><strong>· Asignación de cuadrillas:</strong> A cada orden de trabajo se le asigna una cuadrilla, encargada de ejecutar la reparación.<br><strong>· Registro de reparación:</strong> La reparación está asociada a una orden de trabajo. Contiene fecha de inicio, fecha de finalización y observaciones sobre la intervención.</P>


<H3>DEFINICIONES:</H3>

</P><strong>· Usuario:</strong> Persona que presenta un reclamo.<br><strong>· Reclamo:</strong>Petición presentada por un usuario en relación a un bache.<br><strong>· Bache:</strong> Defecto en la vía pública que requiere reparación.<br><strong>· Inspector:</strong> Empleado que analiza y documenta el estado del bache.<br><strong>· Orden de Trabajo:</strong> Documento generado a partir de un bache para su reparación.<br><strong>· Cuadrilla:</strong>Grupo de trabajo asignado a ejecutar la reparación.<br><strong>· Reparación:</strong> Acción de arreglo físico del bache.<br><strong>· ID:</strong> identificador único de bache.<br><strong>· APP:</strong> aplicación digital para gestión del sistema.<br><strong>· GPS:</strong>sistema de posicionamiento global.</P>

<H3>FUNCIONALIDADES DEL SISTEMA</H3>

</P>· Módulo: <strong>Usuario</strong><br> :bust_in_silhouette:
Registro básico de usuarios (solo como actores del reclamo).</P>

</P>· Módulo: <strong>Reclamos</strong><br>

:warning: Permite registrar reclamos por parte de los usuarios. Cada reclamo se asocia a un bache específico.</P>

</P>· Módulo: <strong>Baches</strong><br> 	:construction:
Registro de información de baches (descripción, ubicación, observaciones). Asociación de reclamos al bache. Relación con inspecciones y órdenes de trabajo.</P>

</P>· Módulo: <strong>Inspector</strong><br> :mag_right:
Permite que un inspector registre observaciones sobre un bache.</P>

</P>· Módulo: <strong>Orden de Trabajo</strong><br>  :memo:
Permite generar una orden a partir de un bache. Asociación con una cuadrilla y posterior reparación.</P>

</P>· Módulo: <strong>Cuadrilla</strong><br> :construction_worker:
Registro de cuadrillas asignadas a órdenes de trabajo.</P>

</P>· Módulo: <strong>Reparación</strong><br> :wrench:
Registro de reparaciones realizadas sobre baches. Incluye fechas y observaciones de la intervención.</P>


<H3>REQUERIMIENTOS FUNCIONALES DEL SISTEMA</H3>

</P><strong>· Registrar un bache con ID</strong>, la ubicación del mismo, el tamaño (1-10), tipo de bache y prioridad.<br><strong>· Permitir a los usuarios registrar un reclamo sobre un bache.</strong><br><strong>· Asignar cuadrillas de reparación</strong>, datos del personal que los integra.<br><strong>· Registrar inspecciones</strong> sobre los baches por parte de inspectores.<br><strong>· Permitir asociar reclamos</strong> a un bache existente o nuevo.<br><strong>· Registrar</strong> las horas trabajadas y el estado del bache.<br><strong>· Generar reportes</strong> por estado, barrio y fecha.<br><strong>· Asociar daños</strong> reportados con datos del ciudadano y monto económico.<br><strong>· Enviar alarmas</strong> para reparaciones pendientes.<br><strong>· Permitir la consulta pública</strong> del estado de los reclamos.<br><strong>· Registrar las reparaciones</strong> asociadas a una orden de trabajo, incluyendo observaciones y fechas.</P>

<H3>REQUERIMIENTOS NO FUNCIONALES</H3>

</P><strong>·Accesibilidad:</strong> El sistema debe ser accesible desde un entorno web.<br><strong>· Trazabilidad:</strong> Todas las entidades (reclamos, baches, órdenes, reparaciones) deben poder rastrearse mediante su identificación.<br><strong>· Integridad de datos:</strong> Las relaciones entre entidades deben mantenerse consistentes (ej. una reparación siempre debe estar ligada a una orden).<br><strong>· Simplicidad:</strong> El sistema debe tener una interfaz amigable y clara para los usuarios que realicen reclamos o inspecciones.</P>

<H3>CONCLUSIÓN</H3>

</P>Este documento refleja de manera clara los requerimientos claves para un sistema de seguimiento de baches. Se prioriza una visión centrada en los usuarios, entendiendo sus necesidades y frustraciones cotidianas.</P>

</P>Como señalan Sommerville y Pressman, definir claramente los servicios esperados y las restricciones operativas es fundamental para el éxito del sistema. </P>
