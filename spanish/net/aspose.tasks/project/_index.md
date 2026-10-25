---
title: "Clase Project"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Project. Representa un proyecto"
type: docs
weight: 1440
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
| [Project](project/#constructor)() | Inicializa una nueva instancia de la clase `Project`. |
| [Project](project/#constructor_1)(DbSettings) | Inicializa una nueva instancia de la clase `Project` para leer datos de una base de datos que está especificada por la instancia de la clase [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/). |
| [Project](project/#constructor_2)(Stream) | Inicializa una nueva instancia de la clase `Project` a partir de un flujo. |
| [Project](project/#constructor_7)(StreamReader) | Inicializa una nueva instancia de la clase `Project` a partir de una instancia de StreamReader. |
| [Project](project/#constructor_8)(string) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo mpp o mpt existente). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Inicializa una nueva instancia de la clase `Project` a partir del flujo con la instancia especificada de la clase [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo mpp o mpt existente). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Inicializa una nueva instancia de la clase `Project` a partir del flujo con la instancia especificada de la clase [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_6)(Stream, string) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo mpp o mpt existente). |
| [Project](project/#constructor_9)(string, LoadOptions) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo mpp o mpt existente) con la instancia especificada de la clase [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo mpp o mpt existente). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla (archivo MPP o MPT existente) con la instancia especificada de la clase [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_12)(string, string) | Inicializa una nueva instancia de la clase `Project` a partir de una plantilla protegida con contraseña (archivo mpp o mpt existente). |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Obtiene o establece un valor que indica si ActualsInSync está configurado o no. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Obtiene o establece un valor que indica si AdminProject está configurado o no. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Obtiene o establece un valor que indica si AreEditableActualCosts está configurado o no. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Obtiene o establece un valor de Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Obtiene o establece un valor que indica si AutoAddNewResourcesAndTasks está configurado o no. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Obtiene o establece si el costo de asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de recursos. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Obtiene o establece un valor que indica si Autolink está configurado o no. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Obtiene o establece un valor de BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Obtiene la colección de propiedades incorporadas del proyecto. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Obtiene o establece el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración [`CalculationMode`](./calculationmode/). |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Obtiene o establece un valor de Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Obtiene el objeto [`CalendarCollection`](../calendarcollection/) de esta instancia de Project. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Obtiene o establece un valor de Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Obtiene o establece un valor de Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Obtiene o establece un valor de Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Obtiene o establece un valor de CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Obtiene una colección que contiene una lista de tareas Critical que forman la ruta crítica de este proyecto. Esta es una operación O(n), donde n es el número de tareas del proyecto. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | MS Project considera que las tareas son críticas si el holgura total es menor o igual a este número de días. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Obtiene o establece un valor de CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Obtiene o establece un valor de CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Obtiene o establece un valor de CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Obtiene o establece un valor de CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Obtiene o establece un valor de CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Obtiene o establece un valor de CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Obtiene la colección de propiedades personalizadas del proyecto. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Obtiene o establece un valor de DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Obtiene o establece un valor de DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Obtiene o establece un valor de DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Obtiene o establece un valor de DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Obtiene o establece un valor de DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Obtiene o establece un valor de DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Obtiene o establece un valor de DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Obtiene o establece un valor de DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Obtiene o establece un valor de DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Obtiene o establece la vista predeterminada del proyecto. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Obtiene la instancia de la clase [`WeekDayCollection`](../weekdaycollection/) que representa una colección de los días laborables y horarios de trabajo semanales predeterminados del proyecto. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Obtiene una instancia de la clase [`ProjectDisplayOptions`](../projectdisplayoptions/). |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Obtiene o establece un valor de DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Obtiene o establece un valor de EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de atributos extendidos (campos personalizados) asociados a un proyecto. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Obtiene o establece un valor de ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Obtiene o establece un valor de FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Obtiene o establece un valor que indica si FiscalYearStart está configurado o no. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Obtiene o establece un valor de FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Obtiene o establece la configuración de globalización (específica de idioma) del proyecto. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Obtiene o establece un valor de Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Obtiene o establece un valor que indica si HonorConstraints está configurado o no. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Obtiene o establece un valor de HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Obtiene o establece un valor que indica si InsertedProjectsLikeSummary está configurado o no. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Obtiene o establece un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Obtiene o establece un valor de Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Obtiene o establece un valor de LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Obtiene o establece un valor de LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Obtiene o establece un valor de LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Obtiene o establece un valor de Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Obtiene o establece un valor que indica si MicrosoftProjectServerURL está configurado o no. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Obtiene o establece un valor de MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Obtiene o establece un valor de MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Obtiene o establece un valor que indica si MoveCompletedEndsBack está configurado o no. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Obtiene o establece un valor que indica si MoveCompletedEndsForward está configurado o no. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Obtiene o establece un valor que indica si MoveRemainingStartsBack está configurado o no. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Obtiene o establece un valor que indica si MoveRemainingStartsForward está configurado o no. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Obtiene o establece un valor que indica si MultipleCriticalPaths está configurado o no. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Obtiene o establece un valor de Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Obtiene o establece un valor que indica si NewTasksAreManual está configurado o no. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Obtiene o establece un valor que indica si NewTasksEffortDriven está configurado o no. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Obtiene o establece un valor que indica si NewTasksEstimated está configurado o no. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Obtiene o establece un valor de NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Obtiene una colección que contiene las instancias de la clase [`OleObject`](../oleobject/) que están vinculadas o incrustadas en este archivo de proyecto. Disponible solo para el formato de archivo mpp. Esta colección es de solo lectura, excepto para la operación 'Clear'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Obtiene el objeto OutlineCodeDefinitionCollection. La colección de definiciones de códigos de esquema asociadas a un proyecto. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Obtiene un objeto que contiene propiedades específicas de Primavera para un proyecto leído desde un archivo Primavera. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Obtiene o establece un valor que indica si ProjectExternallyEdited está configurado o no. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Obtiene o establece un valor que indica si RemoveFileProperties está configurado o no. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Obtiene el objeto ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Obtiene todas las definiciones de filtros basados en recursos. ResourceFilters es una colección de objetos [`Filter`](../filter/). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Obtiene todas las definiciones de grupos basados en recursos. ResourceGroups es una colección de objetos [`Group`](../group/). |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Obtiene el objeto ResourceCollection. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Obtiene o establece un valor de Revision. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Obtiene la raíz del árbol de tareas. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Obtiene o establece un valor de SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Obtiene o establece un valor que indica si ScheduleFromStart está configurado o no. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Obtiene o establece un valor que indica si ShowProjectSummaryTask está configurado o no. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Obtiene o establece un valor que indica si SplitsInProgressTasks está configurado o no. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Obtiene o establece un valor que indica si SpreadActualCost está configurado o no. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Obtiene o establece un valor que indica si SpreadPercentComplete está configurado o no. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Obtiene o establece un valor de StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Obtiene o establece un valor de StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Obtiene o establece un valor de Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Obtiene una lista de objetos [`Table`](../table/). |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Obtiene todas las definiciones de filtros basados en tareas. TaskFilters es una colección de objetos [`Filter`](../filter/). |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Obtiene todas las definiciones de grupos basados en tareas. TaskGroups es una colección de objetos [`Group`](../group/). |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Obtiene el objeto [`TaskLinkCollection`](../tasklinkcollection/). |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Obtiene o establece un valor que indica si TaskUpdatesResource está configurado o no. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Obtiene o establece un valor de Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Obtiene o establece un valor de TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Obtiene o establece un valor de TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Obtiene o establece un valor de Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Obtiene o establece un valor de Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Obtiene o establece un valor que indica si UpdateManuallyScheduledTasksWhenEditingLinks está configurado o no. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Obtiene una instancia de la clase [`VbaProject`](./vbaproject/). |
| [Views](../../aspose.tasks/project/views/) { get; } | Obtiene una lista de objetos [`View`](../view/). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Obtiene o establece la definición de WBS Code Definition para el proyecto. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Obtiene o establece un valor de WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Obtiene o establece un valor de WorkFormat. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Enumera recursivamente todas las tareas del proyecto, incluida la tarea raíz. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Devuelve el valor al que la propiedad está asignada en este contenedor. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Devuelve la hora de guardado de la línea base. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Obtiene el objeto [`Duration`](../duration/) con el número especificado de unidades y el formato de duración predeterminado que está definido en la configuración del proyecto [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Obtiene el objeto [`Duration`](../duration/) con el número especificado de unidades [`TimeUnitType`](../timeunittype/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Obtiene el objeto [`Duration`](../duration/) con el valor TimeSpan especificado y el valor [`TimeUnitType`](../timeunittype/) especificado. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/) predeterminado (Días). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/) predeterminado (Días) y el [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) proporcionado. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Devuelve el recuento de páginas del proyecto que se renderizará usando las [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) dadas. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/) dado. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/) y el [`PageSize`](../../aspose.tasks.visualization/pagesize/) dados. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/) y el [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) dados. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [`Timescale`](../../aspose.tasks.visualization/timescale/), el [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) y el rango de fechas. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Obtiene el objeto [`Duration`](../duration/) con el valor Double especificado y el formato de trabajo predeterminado. |
| [Print](../../aspose.tasks/project/print/#print)() | Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Imprime el proyecto en la impresora especificada con la configuración de impresora predeterminada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Imprime el proyecto según la configuración de impresora especificada y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Imprime el proyecto según la configuración de impresora especificada, opciones de guardado personalizadas y el nombre de documento especificado usando el controlador de impresión estándar (sin interfaz de usuario). |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Reprograma los IDs de todas las tareas del proyecto, los niveles de esquema, las fechas de inicio/fin, establece las fechas tempranas/tardías, calcula holguras, trabajo y campos de costo. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Reprograma los IDs de todas las tareas del proyecto, los niveles de esquema, las fechas de inicio/fin, establece las fechas tempranas/tardías, calcula holguras, trabajo y campos de costo con validación opcional. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Recalcula el ID, la fecha de inicio y la fecha de fin de los recursos. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Elimina asignaciones de recursos inválidas de la lista de asignaciones de recursos del proyecto. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Renumera el código WBS de todas las tareas. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Renumera el código WBS de las tareas completadas. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Reprograma el trabajo del proyecto no completado para que comience después de una fecha especificada. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Reprograma el trabajo no completado de una lista especificada de tareas para que comience después de una fecha especificada. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Guarda los datos del proyecto en el archivo en formato mpp. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Guarda los datos del proyecto en el flujo. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Guarda el proyecto en un flujo usando las opciones de guardado especificadas. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Guarda los datos del proyecto en el archivo. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Guarda el documento en un archivo usando las opciones de guardado especificadas. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Guarda el proyecto como una plantilla en un flujo especificado. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Guarda el proyecto como una plantilla en la ruta de archivo especificada. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Guarda el proyecto como una plantilla en un flujo especificado. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Guarda el proyecto como una plantilla. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Guarda el informe de visión general del proyecto en el flujo. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Guarda el informe de visión general del proyecto en un archivo PDF. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Guarda el informe del proyecto del tipo especificado en el flujo especificado. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Guarda el informe del proyecto del tipo especificado en formato PDF en la ruta de archivo especificada. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Recopila recursivamente todas las tareas hijas de la tarea raíz. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Guarda los campos de línea base en la línea base especificada para todo el proyecto. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Guarda los campos de línea base en la línea base especificada para las tareas seleccionadas. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Establece la hora de guardado de la línea base. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Actualiza todo el trabajo como completado hasta una fecha especificada para todo el proyecto. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Actualiza todo el trabajo como completado hasta una fecha especificada para la lista de tareas especificada. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Obtiene la información del archivo del proyecto del flujo. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Lee la información del archivo del proyecto del archivo. |

## Observaciones

El **Project** es una clase central en la biblioteca Aspose.Tasks.

Se puede usar **Project** para leer uno de los formatos de gestión de proyectos compatibles: MPP, MPT, MPX, XML.

Para cargar un documento existente en cualquiera de los formatos compatibles, pase un nombre de archivo o un flujo a uno de los constructores de **Project**. Para crear un proyecto en blanco, llame al constructor sin parámetros.

Utilice una de las sobrecargas del método Save para guardar el proyecto en cualquiera de los formatos de [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Diseño fijo: PDF; Imágenes: JPEG, PNG, BMP, TIFF, SVG; Texto: TXT; Otros: HTML.

El **Project** almacena información a nivel de proyecto como [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), y [`ExtendedAttributes`](./extendedattributes/). La mayoría de estos objetos son accesibles a través de las propiedades correspondientes de la clase **Project**.

El **Project** es una entidad raíz que contiene puntos de entrada para manipular otras entidades del proyecto, como [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) y [`Calendar`](../calendar/).

Las entidades **Project** pueden accederse mediante colecciones tipadas, por ejemplo [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), etc.

## Ejemplos

Muestra cómo trabajar con una &lt;see cref="Aspose.Tasks.Project"/&gt; instancia.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// agregando nuevas tareas y estableciendo las propiedades deseadas
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// agregando nuevos recursos
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// agregando nuevas asignaciones de recursos
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// guardar el proyecto en uno de los formatos disponibles
// aquí lo estamos guardando en el formato de archivo Microsoft Project XML.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


