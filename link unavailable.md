DOCUMENTO DE DEFINICIÓN DE REQUERIMIENTOS


PROPÓSITO:

<P><br>El objetivo de este documento es describir los requerimientos funcionales y no funcionales de un sistema de **gestión de reclamos y reparación de baches**, basado en los elementos definidos en el modelo UML.<br>Se busca formalizar el proceso desde que un usuario reporta un reclamo hasta la intervención de una cuadrilla mediante una orden de trabajo y su respectiva reparación.<br></P>

FONDO:

<P>Cuando se reportan los baches en la ciudad de Bahía Blanca, se registran en **“sistema de reparación del departamento de obras públicas”** y se les asigna un **número de identificación**, almacenado según la calle, tamaño (en una escala de 1 a 10), ubicación (en medio, cuneta, etc.), distrito (se determina con la dirección en la calle) y prioridad de reparación (determinada por el tamaño del bache).</P>

</P>El sistema de registros de baches se realiza mediante registros manuales, hojas de cálculos y planillas. Al utilizar herramientas físicas, observamos pérdidas de información, falta de control, tareas duplicadas, registros de información incompleta, poca claridad y confiabilidad. <br>Es necesario un sistema digital que **organice este registro** para así poder darle un seguimiento a la solución del problema.</P>

ALCANCE

<P>· Recepción de reclamos: Un usuario realiza un reclamo, el cual se asocia a un bache determinado. El reclamo contiene la descripción del problema.<br>· Gestión del bache: Un bache se vincula a uno o más reclamos. Se registran datos como ubicación, descripción y observaciones. El bache es inspeccionado por un inspector.<br>· Asignación de inspecciones: El inspector evalúa el bache, generando observaciones sobre el mismo.<br>· Generación de órdenes de trabajo: Una vez inspeccionado, el bache puede generar una orden de trabajo. La orden de trabajo contiene la fecha de asignación y se relaciona con el bache.<br>· Asignación de cuadrillas: A cada orden de trabajo se le asigna una cuadrilla, encargada de ejecutar la reparación.<br>· Registro de reparación: La reparación está asociada a una orden de trabajo. Contiene fecha de inicio, fecha de finalización y observaciones sobre la intervención.</P>


DEFINICIONES:

</P>· Usuario: Persona que presenta un reclamo.<br>· Reclamo: Petición presentada por un usuario en relación a un bache.<br>· Bache: Defecto en la vía pública que requiere reparación.<br>· Inspector: Empleado que analiza y documenta el estado del bache.<br>· Orden de Trabajo: Documento generado a partir de un bache para su reparación.<br>· Cuadrilla: Grupo de trabajo asignado a ejecutar la reparación.<br>· Reparación: Acción de arreglo físico del bache.<br>· ID: identificador único de bache.<br>· APP: aplicación digital para gestión del sistema.<br>· GPS: sistema de posicionamiento global.</P>

FUNCIONALIDADES DEL SISTEMA

</P>· Módulo: Usuario
Registro básico de usuarios (solo como actores del reclamo).</P>

</P>· Módulo: Reclamos
Permite registrar reclamos por parte de los usuarios. Cada reclamo se asocia a un bache específico.</P>

</P>· Módulo: Baches
Registro de información de baches (descripción, ubicación, observaciones). Asociación de reclamos al bache. Relación con inspecciones y órdenes de trabajo.</P>

</P>· Módulo: Inspector
Permite que un inspector registre observaciones sobre un bache.</P>

</P>· Módulo: Orden de Trabajo
Permite generar una orden a partir de un bache. Asociación con una cuadrilla y posterior reparación.</P>

</P>· Módulo: Cuadrilla
Registro de cuadrillas asignadas a órdenes de trabajo.</P>

</P>· Módulo: Reparación
Registro de reparaciones realizadas sobre baches. Incluye fechas y observaciones de la intervención.</P>


REQUERIMIENTOS FUNCIONALES DEL SISTEMA

</P>· Registrar un bache con ID, la ubicación del mismo, el tamaño (1-10), tipo de bache y prioridad.<br>· Permitir a los usuarios registrar un reclamo sobre un bache.<br>· Asignar cuadrillas de reparación, datos del personal que los integra.<br>· Registrar inspecciones sobre los baches por parte de inspectores.<br>· Permitir asociar reclamos a un bache existente o nuevo.<br>· Registrar las horas trabajadas y el estado del bache.<br>· Generar reportes por estado, barrio y fecha.<br>· Asociar daños reportados con datos del ciudadano y monto económico.<br>· Enviar alarmas para reparaciones pendientes.<br>· Permitir la consulta pública del estado de los reclamos.<br>· Registrar las reparaciones asociadas a una orden de trabajo, incluyendo observaciones y fechas.</P>

REQUERIMIENTOS NO FUNCIONALES

</P>·Accesibilidad: El sistema debe ser accesible desde un entorno web.<br>· Trazabilidad: Todas las entidades (reclamos, baches, órdenes, reparaciones) deben poder rastrearse mediante su identificación.<br>· Integridad de datos: Las relaciones entre entidades deben mantenerse consistentes (ej. una reparación siempre debe estar ligada a una orden).<br>· Simplicidad: El sistema debe tener una interfaz amigable y clara para los usuarios que realicen reclamos o inspecciones.</P>

CONCLUSIÓN

</P>Este documento refleja de manera clara los requerimientos claves para un sistema de seguimiento de baches. Se prioriza una visión centrada en los usuarios, entendiendo sus necesidades y frustraciones cotidianas.</P>

</P>Como señalan Sommerville y Pressman, definir claramente los servicios esperados y las restricciones operativas es fundamental para el éxito del sistema. </P>
