---
title: Project
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Representa un proyecto.
type: docs
weight: 1180
url: /es/net/aspose.tasks/project/
---
## Project class

Representa un proyecto.

```csharp
public class Project
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Project](project#constructor)() | Inicializa una nueva instancia del[`Project`](../project) clase. |
| [Project](project#constructor_1)(DbSettings) | Inicializa una nueva instancia del[`Project`](../project) clase para leer datos de una base de datos que se especifica por la instancia de la[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) clase. |
| [Project](project#constructor_2)(Stream) | Inicializa una nueva instancia del[`Project`](../project) clase de un stream. |
| [Project](project#constructor_9)(StreamReader) | Inicializa una nueva instancia del[`Project`](../project) clase de una instancia de StreamReader. |
| [Project](project#constructor_10)(string) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo mpp o mpt existente). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Inicializa una nueva instancia del[`Project`](../project) clase del Stream con la instancia especificada del[`LoadOptions`](../loadoptions) clase. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo mpp o mpt existente). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Inicializa una nueva instancia del[`Project`](../project) clase del Stream con la instancia especificada del[`PrimaveraReadOptions`](../primaverareadoptions) clase. |
| [Project](project#constructor_8)(Stream, string) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo mpp o mpt existente). |
| [Project](project#constructor_11)(string, LoadOptions) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo mpp o mpt existente) con la instancia especificada del[`LoadOptions`](../loadoptions) clase. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo mpp o mpt existente). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla (archivo MPP o MPT existente) con la instancia especificada del[`PrimaveraReadOptions`](../primaverareadoptions) clase. |
| [Project](project#constructor_16)(string, string) | Inicializa una nueva instancia del[`Project`](../project) clase de una plantilla protegida por contraseña (archivo mpp o mpt existente). |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Obtiene la colección de propiedades integradas del proyecto. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Obtiene o establece el modo de cálculo de un proyecto. Puede ser uno de los valores de[`CalculationMode`](./calculationmode) enumeración. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Obtiene[`CalendarCollection`](../calendarcollection) objeto de esta instancia de Proyecto. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Obtiene una colección que contiene una lista de tareas críticas que comprenden la ruta crítica de este proyecto. Esta es una operación O(n), donde n es el número de tareas en el proyecto. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Obtiene la colección de propiedades personalizadas del proyecto. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Obtiene o establece la vista predeterminada del proyecto. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Obtiene la instancia de[`WeekDayCollection`](../weekdaycollection) clase que representa una colección de días laborables y horarios laborales predeterminados de la semana del proyecto. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Obtiene una instancia del[`ProjectDisplayOptions`](../projectdisplayoptions) clase. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de atributos extendidos (campos personalizados) asociados con un proyecto. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Obtiene una colección que contiene las instancias del[`OleObject`](../oleobject) class que están vinculados o incrustados en este archivo de proyecto. Disponible solo para formato de archivo mpp. Esta colección es de solo lectura excepto para la operación 'Borrar'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Obtiene el objeto OutlineCodeDefinitionCollection. La colección de definiciones de código de esquema asociadas con un proyecto. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Obtiene el objeto ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Obtiene todas las definiciones de filtro basadas en recursos. ResourceFilters es una colección de[`Filter`](../filter) objetos. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Obtiene todas las definiciones de grupos basadas en recursos. ResourceGroups es una colección de[`Group`](../group) objetos. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Obtiene el objeto ResourceCollection. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Obtiene la raíz del árbol de tareas. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Obtiene una lista de[`Table`](../table) objetos. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Obtiene todas las definiciones de filtro basadas en tareas. TaskFilters es una colección de[`Filter`](../filter) objetos. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Obtiene todas las definiciones de grupos basadas en tareas. TaskGroups es una colección de[`Group`](../group) objetos. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Obtiene[`TaskLinkCollection`](../tasklinkcollection) objeto. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Obtiene una instancia de[`VbaProject`](./vbaproject) clase. |
| [Views](../../aspose.tasks/project/views) { get; } | Obtiene una lista de[`View`](../view) objetos. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Obtiene o establece la definición de código WBS para el proyecto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Enumera recursivamente todas las tareas del proyecto, incluida la tarea raíz. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Devuelve el valor al que se asigna la propiedad en este contenedor. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Devuelve el tiempo de ahorro de referencia. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Obtiene[`Duration`](../duration) objeto con el número especificado de unidades y el formato de duración predeterminado que se define en la configuración del proyecto[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Obtiene[`Duration`](../duration) objeto con el número especificado de[`TimeUnitType`](../timeunittype) unidades. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Obtiene[`Duration`](../duration) objeto con el especificadoTimeSpan valor y especificado[`TimeUnitType`](../timeunittype) valor. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Devuelve el recuento de páginas para que el proyecto se represente usando el valor predeterminado[`Timescale`](../../aspose.tasks.visualization/timescale) (Días). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Devuelve el recuento de páginas para que el proyecto se represente usando el valor predeterminado[`Timescale`](../../aspose.tasks.visualization/timescale) (Días) y dado[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Devuelve el recuento de páginas del proyecto que se representará utilizando[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../aspose.tasks.visualization/timescale) y[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../aspose.tasks.visualization/timescale) y[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Devuelve el recuento de páginas del proyecto que se representará utilizando[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) y rango de fechas. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Obtiene[`Duration`](../duration) objeto con el especificadoDouble valor y formato de trabajo por defecto. |
| [Print](../../aspose.tasks/project/print#print)() | Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada mediante el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Imprime el proyecto de acuerdo con la configuración de impresora especificada mediante el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada y las opciones de guardado personalizadas mediante el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Imprime el proyecto en la impresora especificada con la configuración de impresora predeterminada utilizando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Imprime el proyecto de acuerdo con la configuración de impresora especificada y las opciones de guardado personalizadas mediante el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Imprime el proyecto de acuerdo con la configuración de impresora especificada mediante el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Imprime el proyecto de acuerdo con la configuración de la impresora especificada, las opciones personalizadas para guardar y el nombre del documento especificado utilizando el controlador de impresión estándar (sin interfaz de usuario). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Reprograma todas las identificaciones de tareas del proyecto, niveles de esquema, fechas de inicio/finalización, establece fechas tempranas/finales, calcula espacios libres, trabajo y campos de costos. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Reprograma todas las identificaciones de tareas del proyecto, niveles de esquema, fechas de inicio/finalización, establece fechas tempranas/tardías, calcula espacios libres, trabajo y campos de costos con validación opcional. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Recalcula Id, Inicio y Fin de recursos. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Recalcula Inicio y Fin de recursos. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Elimina las asignaciones de recursos no válidas de la lista de asignaciones de recursos del proyecto. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Renumerar código WBS de todas las tareas. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Renumerar código WBS de tareas pasadas. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Reprograma el trabajo del proyecto incompleto para comenzar después de una fecha específica. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Reprograma el trabajo incompleto para una lista específica de tareas para comenzar después de una fecha específica. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Guarda los datos del proyecto en el archivo en formato mpp. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Guarda el proyecto en una secuencia usando las opciones de guardado especificadas. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Guarda los datos del proyecto en la secuencia. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Guarda el proyecto en una secuencia usando las opciones de guardado especificadas. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Guarda el documento en formato de archivo mpp utilizando las opciones de guardado especificadas. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Guarda los datos del proyecto en el archivo. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Guarda el documento en un archivo usando las opciones de guardado especificadas. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Guarda el proyecto como plantilla en un flujo específico. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Guarda el proyecto como plantilla en la ruta de archivo especificada. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Guarda el proyecto como plantilla en un flujo específico. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Guarda el proyecto como plantilla. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Guarda el informe de descripción general del proyecto en la ruta. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Guarda el informe general del proyecto en un archivo PDF. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Guarda el informe del proyecto del tipo especificado en la secuencia especificada. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Guarda el informe del proyecto del tipo especificado en formato PDF en la ruta de archivo especificada. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Recopila recursivamente todas las tareas secundarias de la tarea raíz. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Asigna la propiedad especificada al valor especificado en este contenedor. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Asigna la propiedad especificada al valor especificado en este contenedor. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Guarda los campos de línea base en la línea base especificada para todo el proyecto. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Guarda los campos de línea base en la línea base especificada para las tareas seleccionadas. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Establece el tiempo de ahorro de referencia. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Actualiza todo el trabajo como completado hasta una fecha específica para todo el proyecto. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Actualiza todo el trabajo como completo hasta una fecha específica para la lista de tareas especificada. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Obtiene información del archivo del proyecto de la transmisión. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Lee la información del archivo del proyecto desde el archivo. |

### Observaciones

los **Proyecto** es una clase central en la biblioteca Aspose.Tasks.

Uno puede usar **Proyecto** para leer uno de los formatos de gestión de proyectos admitidos: MPP, MPT, MPX, XML.

Para cargar un documento existente en cualquiera de los formatos admitidos, pase un nombre de archivo o una secuencia a uno de los **Proyecto** constructores Para crear un proyecto en blanco, llame al constructor sin parámetros.

Utilice una de las sobrecargas del método Save para guardar el proyecto en cualquiera de los[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) formatos: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Diseño fijo: PDF; Imágenes: JPEG, PNG, BMP, TIFF, SVG; Texto: TXT; Otros: HTML.

Para imprimir el proyecto, utilice uno de los[`Print`](./print) sobrecargas de métodos.

los **Proyecto** almacena información de todo el proyecto, como[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , y[`ExtendedAttributes`](./extendedattributes) . La mayoría de estos objetos son accesibles a través de las propiedades correspondientes del **Proyecto** clase.

los **Proyecto** es una entidad raíz que contiene puntos de entrada para manipular otras entidades del proyecto, como[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) y[`Calendar`](../calendar).

El **Proyecto** se puede acceder a las entidades a través de colecciones escritas, por ejemplo[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , etc.

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
