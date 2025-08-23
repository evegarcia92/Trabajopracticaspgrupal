DOCUMENTO DE DEFINICIÓN DE REQUERIMIENTOS


PROPÓSITO:

El objetivo de este documento es describir los requerimientos funcionales y no funcionales de un sistema de gestión de reclamos y reparación de baches, basado en los elementos definidos en el modelo UML. Se busca formalizar el proceso desde que un usuario reporta un reclamo hasta la intervención de una cuadrilla mediante una orden de trabajo y su respectiva reparación.

FONDO:

Cuando se reportan los baches en la ciudad de Bahía Blanca, se registran en “sistema de reparación del departamento de obras públicas” y se les asigna un número de identificación, almacenado según la calle, tamaño (en una escala de 1 a 10), ubicación (en medio, cuneta, etc.), distrito (se determina con la dirección en la calle) y prioridad de reparación (determinada por el tamaño del bache). El sistema de registros de baches se realiza mediante registros manuales, hojas de cálculos y planillas. Al utilizar herramientas físicas, observamos pérdidas de información, falta de control, tareas duplicadas, registros de información incompleta, poca claridad y confiabilidad. 
Es necesario un sistema digital que organice este registro para así poder darle un seguimiento a la solución del problema.

ALCANCE
Recepción de reclamos: Un usuario realiza un reclamo, el cual se asocia a un bache determinado. El reclamo contiene la descripción del problema.
Gestión del bache: Un bache se vincula a uno o más reclamos. Se registran datos como ubicación, descripción y observaciones. El bache es inspeccionado por un inspector.
Asignación de inspecciones: El inspector evalúa el bache, generando observaciones sobre el mismo.
Generación de órdenes de trabajo: Una vez inspeccionado, el bache puede generar una orden de trabajo. La orden de trabajo contiene la fecha de asignación y se relaciona con el bache.
Asignación de cuadrillas: A cada orden de trabajo se le asigna una cuadrilla, encargada de ejecutar la reparación.
Registro de reparación: La reparación está asociada a una orden de trabajo. Contiene fecha de inicio, fecha de finalización y observaciones sobre la intervención.


DEFINICIONES:
Usuario: Persona que presenta un reclamo.
Reclamo: Petición presentada por un usuario en relación a un bache.
Bache: Defecto en la vía pública que requiere reparación.
Inspector: Empleado que analiza y documenta el estado del bache.
Orden de Trabajo: Documento generado a partir de un bache para su reparación.
Cuadrilla: Grupo de trabajo asignado a ejecutar la reparación.
Reparación: Acción de arreglo físico del bache
ID: identificador único de bache
APP: aplicación digital para gestión del sistema
GPS: sistema de posicionamiento global
FUNCIONALIDADES DEL SISTEMA
Módulo: Usuario
Registro básico de usuarios (solo como actores del reclamo).
Módulo: Reclamos
Permite registrar reclamos por parte de los usuarios. Cada reclamo se asocia a un bache específico.
Módulo: Baches
Registro de información de baches (descripción, ubicación, observaciones). Asociación de reclamos al bache. Relación con inspecciones y órdenes de trabajo.
Módulo: Inspector
Permite que un inspector registre observaciones sobre un bache.
Módulo: Orden de Trabajo
Permite generar una orden a partir de un bache. Asociación con una cuadrilla y posterior reparación.
Módulo: Cuadrilla
Registro de cuadrillas asignadas a órdenes de trabajo.
Módulo: Reparación
Registro de reparaciones realizadas sobre baches. Incluye fechas y observaciones de la intervención.


REQUERIMIENTOS FUNCIONALES DEL SISTEMA
Registrar un bache con ID, la ubicación del mismo, el tamaño (1-10), tipo de bache y prioridad.
Permitir a los usuarios registrar un reclamo sobre un bache.
Asignar cuadrillas de reparación, datos del personal que los integra 
Registrar inspecciones sobre los baches por parte de inspectores.
Permitir asociar reclamos a un bache existente o nuevo.
Registrar las horas trabajadas y el estado del bache
Generar reportes por estado, barrio y fecha
Asociar daños reportados con datos del ciudadano y monto económico
Enviar alarmas para reparaciones pendientes
Permitir la consulta pública del estado de los reclamos
Registrar las reparaciones asociadas a una orden de trabajo, incluyendo observaciones y fechas.

REQUERIMIENTOS NO FUNCIONALES
·  Accesibilidad: El sistema debe ser accesible desde un entorno web.
· Trazabilidad: Todas las entidades (reclamos, baches, órdenes, reparaciones) deben poder rastrearse mediante su identificación.
· Integridad de datos: Las relaciones entre entidades deben mantenerse consistentes (ej. una reparación siempre debe estar ligada a una orden).
· Simplicidad: El sistema debe tener una interfaz amigable y clara para los usuarios que realicen reclamos o inspecciones.

CONCLUSIÓN

Este documento refleja de manera clara los requerimientos claves para un sistema de seguimiento de baches. Se prioriza una visión centrada en los usuarios, entendiendo sus necesidades y frustraciones cotidianas.
Como señalan Sommerville y Pressman, definir claramente los servicios esperados y las restricciones operativas es fundamental para el éxito del sistema. 
