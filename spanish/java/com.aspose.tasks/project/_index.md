---
title: "Proyecto"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un proyecto."
type: docs
weight: 220
url: /es/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Representa un proyecto.

--------------------

La **Project** es una clase central en la biblioteca Aspose.Tasks.

Se puede usar **Project** para leer uno de los formatos de gestión de proyectos compatibles: MPP, MPT, MPX, XML.

Para cargar un documento existente en cualquiera de los formatos compatibles, pase un nombre de archivo o un flujo a uno de los constructores de **Project**. Para crear un proyecto vacío, llame al constructor sin parámetros.

Utilice una de las sobrecargas del método Save para guardar el proyecto en cualquiera de los formatos de [SaveFileFormat](../../com.aspose.tasks/savefileformat): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Diseño fijo: PDF; Imágenes: JPEG, PNG, BMP, TIFF, SVG; Texto: TXT; Otros: HTML.

Para imprimir el proyecto, use una de las sobrecargas del método [print()](../../com.aspose.tasks/project\#print--).

El **Project** almacena información a nivel de proyecto, como `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), y `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). La mayoría de estos objetos son accesibles a través de las propiedades correspondientes de la clase **Project**.

El **Project** es una entidad raíz que contiene puntos de entrada para manipular otras entidades del proyecto, como [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) y [Calendar](../../com.aspose.tasks/calendar).

Las entidades **Project** pueden accederse mediante colecciones tipadas, por ejemplo `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), etc.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Project()](#Project--) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla protegida con contraseña (archivo mpp o mpt existente). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir del Stream con la instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de un stream. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo MPP o MPT existente) con la instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) para leer datos de una base de datos que es especificada por la instancia de la clase [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente) con la instancia especificada de la clase [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) desde el Stream con la instancia especificada de la clase [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Devuelve el valor al que la propiedad está mapeada en este contenedor. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Enumera recursivamente todas las tareas del proyecto, incluida la tarea raíz. |
| [getActualsInSync()](#getActualsInSync--) | Obtiene un valor que indica si ActualsInSync está configurado o no. |
| [getAdminProject()](#getAdminProject--) | Obtiene un valor que indica si AdminProject está configurado o no. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Obtiene un valor que indica si AreEditableActualCosts está configurado o no. |
| [getAuthor()](#getAuthor--) | Obtiene el valor de Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Obtiene un valor que indica si AutoAddNewResourcesAndTasks está configurado o no. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Obtiene si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos. |
| [getAutolink()](#getAutolink--) | Obtiene un valor que indica si Autolink está configurado o no. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Obtiene el valor de BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Devuelve la hora de guardado de la línea base. |
| [getBuiltInProps()](#getBuiltInProps--) | Obtiene la colección de propiedades incorporadas del proyecto. |
| [getCalculationMode()](#getCalculationMode--) | Obtiene el modo de cálculo de un proyecto. |
| [getCalendar()](#getCalendar--) | Obtiene un valor de Calendar. |
| [getCalendars()](#getCalendars--) | Obtiene el objeto [CalendarCollection](../../com.aspose.tasks/calendarcollection) de esta instancia de Project. |
| [getCategory()](#getCategory--) | Obtiene el valor de Category. |
| [getComments()](#getComments--) | Obtiene el valor de Comments. |
| [getCompany()](#getCompany--) | Obtiene el valor de Company. |
| [getCreationDate()](#getCreationDate--) | Obtiene el valor de CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | Obtiene una colección que contiene una lista de tareas Critical que forman la ruta crítica de este proyecto. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Las tareas se consideran críticas por MS Project si la holgura total es menor o igual a este número de días. |
| [getCurrencyCode()](#getCurrencyCode--) | Obtiene el valor de CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Obtiene un valor de CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Obtiene un valor de CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Obtiene un valor de CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Obtiene un valor de CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Obtiene un valor de CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Obtiene la colección de propiedades personalizadas del proyecto. |
| [getDateFormat()](#getDateFormat--) | Obtiene un valor de DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Obtiene un valor de DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Obtiene un valor de DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Obtiene un valor de DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Obtiene un valor de DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Obtiene un valor de DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Obtiene un valor de DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Obtiene un valor de DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Obtiene un valor de DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Obtiene la vista predeterminada del proyecto. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Obtiene la instancia de la clase [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) que representa una colección de los días laborables y horarios de trabajo predeterminados del proyecto. |
| [getDisplayOptions()](#getDisplayOptions--) | Obtiene una instancia de la clase [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Obtiene el objeto [Duration](../../com.aspose.tasks/duration) con el número especificado de unidades y el formato de duración predeterminado que está definido en la configuración del proyecto [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Obtiene el objeto [Duration](../../com.aspose.tasks/duration) con el número especificado de unidades de [TimeUnitType](../../com.aspose.tasks/timeunittype). |
| [getDurationFormat()](#getDurationFormat--) | Obtiene un valor de DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Obtiene un valor de EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtiene el objeto ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Obtiene un valor de ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Obtiene un valor de FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Obtiene un valor que indica si FiscalYearStart está configurado o no. |
| [getFyStartDate()](#getFyStartDate--) | Obtiene un valor de FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Obtiene la configuración de globalización (específica del idioma) del proyecto. |
| [getGuid()](#getGuid--) | Obtiene un valor de Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Obtiene un valor que indica si HonorConstraints está configurado o no. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Obtiene un valor de HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Obtiene un valor que indica si InsertedProjectsLikeSummary está configurado o no. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Obtiene un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no. |
| [getKeywords()](#getKeywords--) | Obtiene un valor de Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Obtiene un valor de LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Obtiene un valor de LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Obtiene un valor de LastSaved. |
| [getManager()](#getManager--) | Obtiene un valor de Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Obtiene un valor que indica si MicrosoftProjectServerURL está configurado o no. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Obtiene un valor de MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Obtiene un valor de MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Obtiene un valor que indica si MoveCompletedEndsBack está configurado o no. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Obtiene un valor que indica si MoveCompletedEndsForward está configurado o no. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Obtiene un valor que indica si MoveRemainingStartsBack está configurado o no. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Obtiene un valor que indica si MoveRemainingStartsForward está configurado o no. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Obtiene un valor que indica si MultipleCriticalPaths está configurado o no. |
| [getName()](#getName--) | Obtiene un valor de Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Obtiene un valor de NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Obtiene un valor que indica si NewTasksAreManual está configurado o no. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Obtiene un valor que indica si NewTasksEffortDriven está configurado o no. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Obtiene un valor que indica si NewTasksEstimated está configurado o no. |
| [getOleObjects()](#getOleObjects--) | Obtiene una colección que contiene las instancias de la clase [OleObject](../../com.aspose.tasks/oleobject) que están vinculadas o incrustadas en este archivo de proyecto. |
| [getOutlineCodes()](#getOutlineCodes--) | Obtiene el objeto OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) predeterminado (Días). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Devuelve el recuento de páginas del proyecto que se renderizará usando las [SaveOptions](../../com.aspose.tasks/saveoptions) proporcionadas. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) y el [PresentationFormat](../../com.aspose.tasks/presentationformat) proporcionados. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) y el [PageSize](../../com.aspose.tasks/pagesize) proporcionados. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale), el [PresentationFormat](../../com.aspose.tasks/presentationformat) y el rango de fechas proporcionados. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) predeterminado (Días) y el [PresentationFormat](../../com.aspose.tasks/presentationformat) proporcionado. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) proporcionado. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Obtiene un objeto que contiene propiedades específicas de Primavera para un proyecto leído del archivo Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Obtiene un valor que indica si ProjectExternallyEdited está establecido o no. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Obtiene la información del archivo del proyecto desde el flujo. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Lee la información del archivo del proyecto desde el archivo. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Obtiene un valor que indica si RemoveFileProperties está establecido o no. |
| [getResourceAssignments()](#getResourceAssignments--) | Obtiene el objeto ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | Obtiene todas las definiciones de filtros basados en recursos. |
| [getResourceGroups()](#getResourceGroups--) | Obtiene todas las definiciones de grupos basados en recursos. |
| [getResources()](#getResources--) | Obtiene el objeto ResourceCollection. |
| [getRevision()](#getRevision--) | Obtiene un valor de Revision. |
| [getRootTask()](#getRootTask--) | Obtiene la raíz del árbol de tareas. |
| [getSaveVersion()](#getSaveVersion--) | Obtiene un valor de SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Obtiene un valor que indica si ScheduleFromStart está establecido o no. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Obtiene un valor que indica si ShowProjectSummaryTask está establecido o no. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Obtiene un valor que indica si SplitsInProgressTasks está establecido o no. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Obtiene un valor que indica si SpreadActualCost está establecido o no. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Obtiene un valor que indica si SpreadPercentComplete está configurado o no. |
| [getStartDate()](#getStartDate--) | Obtiene un valor de StartDate. |
| [getStatusDate()](#getStatusDate--) | Obtiene un valor de StatusDate. |
| [getSubject()](#getSubject--) | Obtiene un valor de Subject. |
| [getTables()](#getTables--) | Obtiene una lista de objetos [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | Obtiene todas las definiciones de filtros basados en tareas. |
| [getTaskGroups()](#getTaskGroups--) | Obtiene todas las definiciones de grupos basados en tareas. |
| [getTaskLinks()](#getTaskLinks--) | Obtiene el objeto [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Obtiene un valor que indica si TaskUpdatesResource está configurado o no. |
| [getTemplate()](#getTemplate--) | Obtiene un valor de Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Obtiene un valor de TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Obtiene un valor de TimescaleStart. |
| [getTitle()](#getTitle--) | Obtiene un valor de Title. |
| [getUid()](#getUid--) | Obtiene un valor de Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Obtiene un valor que indica si UpdateManuallyScheduledTasksWhenEditingLinks está configurado o no. |
| [getVbaProject()](#getVbaProject--) | Obtiene una instancia de la clase `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | Obtiene una lista de objetos [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Obtiene la definición del código WBS para el proyecto. |
| [getWeekStartDay()](#getWeekStartDay--) | Obtiene un valor de WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Obtiene el objeto [Duration](../../com.aspose.tasks/duration) con el valor `double` especificado y el formato de trabajo predeterminado. |
| [getWorkFormat()](#getWorkFormat--) | Obtiene un valor de WorkFormat. |
| [print()](#print--) | Imprime el proyecto en la impresora predeterminada con la configuración predeterminada de la impresora usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Imprime el proyecto en la impresora predeterminada con la configuración predeterminada de la impresora y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Imprime el proyecto según la configuración de impresora especificada y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Imprime el proyecto según la configuración de impresora especificada, opciones de guardado personalizadas y el nombre de documento especificado usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario). |
| [print(String printerName)](#print-java.lang.String-) | Imprime el proyecto en la impresora especificada con la configuración predeterminada de la impresora usando el controlador de impresión estándar (sin interfaz de usuario). |
| [recalculate()](#recalculate--) | Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo con validación opcional. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Recalcula el ID, inicio y fin de los recursos. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Recalcula el inicio y fin de los recursos. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Elimina asignaciones de recursos inválidas de la lista de asignaciones de recursos del proyecto. |
| [renumberWBSCode()](#renumberWBSCode--) | Renumera el código WBS de todas las tareas. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Renumera el código WBS de las tareas pasadas. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Reprograma el trabajo del proyecto no completado para que comience después de una fecha especificada. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Reprograma el trabajo no completado de una lista especificada de tareas para que comience después de una fecha especificada. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Guarda el proyecto en un flujo usando las opciones de guardado especificadas. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Guarda los datos del proyecto en el flujo. |
| [save(String filename)](#save-java.lang.String-) | Guarda los datos del proyecto en el archivo en formato mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Guarda el documento en un archivo usando las opciones de guardado especificadas. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Guarda los datos del proyecto en el archivo. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Guarda el proyecto como una plantilla en un flujo especificado. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Guarda el proyecto como una plantilla en un flujo especificado. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Guarda el proyecto como una plantilla en la ruta de archivo especificada. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Guarda el proyecto como una plantilla. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Guarda el informe de visión general del proyecto en el flujo. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Guarda el informe del proyecto del tipo especificado en el flujo especificado. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Guarda el informe de visión general del proyecto en un archivo PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Guarda el informe del proyecto del tipo especificado en formato PDF en la ruta de archivo especificada. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Recopila recursivamente todas las tareas hijas de la tarea raíz. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Establece un valor que indica si ActualsInSync está configurado o no. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Establece un valor que indica si AdminProject está configurado o no. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Establece un valor que indica si AreEditableActualCosts está configurado o no. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece un valor de Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Establece un valor que indica si AutoAddNewResourcesAndTasks está configurado o no. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Establece si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Establece un valor que indica si Autolink está configurado o no. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Guarda los campos de línea base en la línea base especificada para todo el proyecto. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Guarda los campos de línea base en la línea base especificada para las tareas seleccionadas. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Establece un valor de BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Establece el tiempo de guardado de la línea base. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Establece el modo de cálculo de un proyecto. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Establece un valor de Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Establece un valor de Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Establece un valor de Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Establece un valor de Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Establece un valor de CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Las tareas se consideran críticas por MS Project si la holgura total es menor o igual a este número de días. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Establece un valor de CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Establece un valor de CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Establece un valor de CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Establece un valor de CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Establece un valor de CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Establece un valor de CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Establece un valor de DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Establece un valor de DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Establece un valor de DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Establece un valor de DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Establece un valor de DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Establece un valor de DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Establece un valor de DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Establece un valor de DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Establece un valor de DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Establece la vista predeterminada del proyecto. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Establece un valor de DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Establece un valor de EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Establece un valor de ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Establece un valor de FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Establece un valor que indica si FiscalYearStart está configurado o no. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Establece un valor de FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Establece la globalización (configuraciones específicas de idioma) del proyecto. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Establece un valor de Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Establece un valor que indica si HonorConstraints está configurado o no. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Establece un valor de HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Establece un valor que indica si InsertedProjectsLikeSummary está configurado o no. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Establece un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Establece un valor de Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Establece un valor de LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Establece un valor de LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Establece un valor de LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Establece un valor de Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MicrosoftProjectServerURL está configurado o no. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Establece un valor de MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Establece un valor de MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MoveCompletedEndsBack está configurado o no. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MoveCompletedEndsForward está configurado o no. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MoveRemainingStartsBack está configurado o no. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MoveRemainingStartsForward está configurado o no. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Establece un valor que indica si MultipleCriticalPaths está configurado o no. |
| [setName(String value)](#setName-java.lang.String-) | Establece un valor de Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Establece un valor de NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Establece un valor que indica si NewTasksAreManual está configurado o no. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Establece un valor que indica si NewTasksEffortDriven está configurado o no. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Establece un valor que indica si NewTasksEstimated está configurado o no. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Establece un valor que indica si ProjectExternallyEdited está configurado o no. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Establece un valor que indica si RemoveFileProperties está configurado o no. |
| [setRevision(int value)](#setRevision-int-) | Establece un valor de Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Establece un valor de SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Establece un valor que indica si ScheduleFromStart está configurado o no. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Establece un valor que indica si ShowProjectSummaryTask está configurado o no. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Establece un valor que indica si SplitsInProgressTasks está configurado o no. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Establece un valor que indica si SpreadActualCost está configurado o no. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Establece un valor que indica si SpreadPercentComplete está configurado o no. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Establece un valor de StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Establece un valor de StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Establece un valor de Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Establece un valor que indica si TaskUpdatesResource está configurado o no. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Establece un valor de Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Establece un valor de TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Establece un valor de TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Establece un valor de Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Establece un valor de Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Establece un valor que indica si UpdateManuallyScheduledTasksWhenEditingLinks está activado o no. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Establece la definición de código WBS para el proyecto. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Establece un valor de WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Establece un valor de WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Actualiza todo el trabajo como completado hasta una fecha especificada para todo el proyecto. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Actualiza todo el trabajo como completado hasta una fecha especificada para la lista de tareas especificada. |
### Project() {#Project--}
```
public Project()
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla protegida con contraseña (archivo mpp o mpt existente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | java.lang.String | Ruta a la plantilla desde la cual crear el proyecto. |
|  | protectionPassword | java.lang.String | Contraseña de protección. |

--------------------

La lectura de archivos protegidos con contraseña solo es compatible actualmente con el formato de archivo MSP 2003. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | java.lang.String | Ruta a la plantilla desde la cual crear el proyecto. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir del Stream con la instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | Flujo del proyecto java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | La instancia especificada de la [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)class que permite personalizar la lectura de los formatos Primavera (XER o XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | java.lang.String | Ruta a la plantilla desde la cual crear el proyecto. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | El método de devolución de llamada especificado para manejar errores de análisis xml. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de un stream.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream para cargar una plantilla desde. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo MPP o MPT existente) con la instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | java.lang.String | Ruta a la plantilla desde la cual crear el proyecto |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | La instancia especificada de la [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) para leer datos de una base de datos que es especificada por la instancia de la clase [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | La instancia especificada de la [DbSettings](../../com.aspose.tasks/dbsettings) class. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream para cargar una plantilla desde. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | El método de devolución de llamada especificado para manejar errores de análisis xml. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream para cargar una plantilla desde. |
|  | protectionPassword | java.lang.String | Contraseña de protección. |

--------------------

La lectura de archivos protegidos con contraseña solo es compatible actualmente con el formato de archivo MSP 2003. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) a partir de una plantilla (archivo mpp o mpt existente) con la instancia especificada de la clase [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | java.lang.String | Ruta a la plantilla desde la cual crear el proyecto |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | La instancia especificada de la [LoadOptions](../../com.aspose.tasks/loadoptions) class. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Inicializa una nueva instancia de la clase [Project](../../com.aspose.tasks/project) desde el Stream con la instancia especificada de la clase [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | Flujo del proyecto java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | La instancia especificada de la [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Devuelve el valor al que la propiedad está mapeada en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | La clave de propiedad especificada. [Prj](../../com.aspose.tasks/prj) para obtener la clave de propiedad. |

**Returns:**
T - el valor al que la propiedad está asignada en este contenedor.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mapea la propiedad especificada al valor especificado en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | La clave de propiedad especificada. [Prj](../../com.aspose.tasks/prj) para obtener la clave de propiedad. |
| val | T | el valor. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Copia los datos principales y las propiedades del proyecto a otro proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Otro proyecto al que copiar datos. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Copia los datos principales y las propiedades del proyecto a otro proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Otro proyecto al que copiar datos. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Opciones de copia para controlar el proceso de copia. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Enumera recursivamente todas las tareas del proyecto, incluida la tarea raíz.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable que puede usarse para iterar sobre todas las tareas del proyecto.

--------------------

Proporciona una forma más ligera de iterar sobre las tareas en comparación con el método [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--), ya que no asigna memoria para todas las tareas.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Obtiene un valor que indica si ActualsInSync está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Obtiene un valor que indica si AdminProject está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Obtiene un valor que indica si AreEditableActualCosts está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Obtiene el valor de Author.

**Returns:**
java.lang.String - un valor de Autor.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Obtiene un valor que indica si AutoAddNewResourcesAndTasks está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Obtiene si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos.

**Returns:**
boolean - si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Obtiene un valor que indica si Autolink está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Obtiene el valor de BaselineForEarnedValue.

**Returns:**
int - un valor de BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Devuelve la hora de guardado de la línea base. Devuelve DateTime.MinValue (00:00:00.0000000 UTC, 1 de enero de 0001) si la línea base no se guardó.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baselineNumber | int | El número de la línea base [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - La última fecha y hora de guardado de la línea base.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Obtiene la colección de propiedades incorporadas del proyecto.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Obtiene el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - modo de cálculo de un proyecto.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Obtiene un valor de Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Obtiene el objeto [CalendarCollection](../../com.aspose.tasks/calendarcollection) de esta instancia de Project.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Obtiene el valor de Category.

**Returns:**
java.lang.String - un valor de Categoría.
### getComments() {#getComments--}
```
public final String getComments()
```


Obtiene el valor de Comments.

**Returns:**
java.lang.String - un valor de Comentarios.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Obtiene el valor de Company.

**Returns:**
java.lang.String - un valor de Empresa.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Obtiene el valor de CreationDate.

**Returns:**
java.util.Date - un valor de CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Obtiene una colección que contiene una lista de tareas Critical que forman la ruta crítica de este proyecto.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Esta es una operación O(n), donde n es el número de tareas en el proyecto.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Las tareas se consideran críticas por MS Project si la holgura total es menor o igual a este número de días.

**Returns:**
int - el valor máximo del tiempo total de holgura (en días) en el que una tarea se considera crítica
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Obtiene el valor de CurrencyCode.

**Returns:**
java.lang.String - un valor de CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Obtiene un valor de CurrencyDigits.

**Returns:**
int - un valor de CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Obtiene un valor de CurrencySymbol.

**Returns:**
java.lang.String - un valor de CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Obtiene un valor de CurrencySymbolPosition.

**Returns:**
int - un valor de CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Obtiene un valor de CurrentDate.

**Returns:**
java.util.Date - un valor de CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Obtiene un valor de CustomDateFormat.

**Returns:**
java.lang.String - un valor de CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Obtiene la colección de propiedades personalizadas del proyecto.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Obtiene un valor de DateFormat.

**Returns:**
int - un valor de DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Obtiene un valor de DaysPerMonth.

**Returns:**
int - un valor de DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Obtiene un valor de DefaultFinishTime.

**Returns:**
java.util.Date - un valor de DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Obtiene un valor de DefaultFixedCostAccrual.

**Returns:**
int - un valor de DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Obtiene un valor de DefaultOvertimeRate.

**Returns:**
double - un valor de DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Obtiene un valor de DefaultStandardRate.

**Returns:**
double - un valor de DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Obtiene un valor de DefaultStartTime.

**Returns:**
java.util.Date - un valor de DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Obtiene un valor de DefaultTaskEVMethod.

**Returns:**
int - un valor de DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Obtiene un valor de DefaultTaskType.

**Returns:**
int - un valor de DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Obtiene la vista predeterminada del proyecto.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Obtiene la instancia de la clase [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) que representa una colección de los días laborables y horarios de trabajo predeterminados del proyecto.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Los datos solo están en archivos mpp (no en xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Obtiene una instancia de la clase [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Obtiene el objeto [Duration](../../com.aspose.tasks/duration) con el número especificado de unidades y el formato de duración predeterminado que está definido en la configuración del proyecto [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | val | double | número especificado de unidades. |

--------------------

Este método debe usarse con cuidado porque devuelve duraciones diferentes según la configuración de Project.DurationFormat. Por ejemplo, GetWork(1.0) devolverá 1 hora cuando Project.DurationFormat sea TimeUnitType.Hour o 1 día si Project.DurationFormat es TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Obtiene el objeto [Duration](../../com.aspose.tasks/duration) con el número especificado de unidades de [TimeUnitType](../../com.aspose.tasks/timeunittype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| val | double | número especificado de unidades. |
| unidadDeTiempo | byte | valor especificado de TimeUnitType. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Obtiene un valor de DurationFormat.

**Returns:**
byte - un valor de DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Obtiene un valor de EarnedValueMethod.

**Returns:**
int - un valor de EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de atributos extendidos (campos personalizados) asociados a un proyecto.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Obtiene un valor de ExtendedCreationDate.

**Returns:**
java.util.Date - un valor de ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Obtiene un valor de FinishDate.

**Returns:**
java.util.Date - un valor de FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Obtiene un valor que indica si FiscalYearStart está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Obtiene un valor de FyStartDate.

**Returns:**
int - un valor de FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Obtiene la configuración de globalización (específica del idioma) del proyecto.

La forma recomendada es usar literales o formatos invariables a la cultura en todo el proyecto. Sin embargo, si un proyecto usa literales específicos de la cultura, esta clase puede usarse para ayudar al motor de cálculo a analizar esos literales.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtiene un valor de Guid.

**Returns:**
java.util.UUID - un valor de Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Obtiene un valor que indica si HonorConstraints está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Obtiene un valor de HyperlinkBase.

**Returns:**
java.lang.String - un valor de HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Obtiene un valor que indica si InsertedProjectsLikeSummary está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Obtiene un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Obtiene un valor de Keywords.

**Returns:**
java.lang.String - un valor de Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Obtiene un valor de LastAuthor.

**Returns:**
java.lang.String - un valor de LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Obtiene un valor de LastPrinted.

**Returns:**
java.util.Date - un valor de LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Obtiene un valor de LastSaved.

**Returns:**
java.util.Date - un valor de LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Obtiene un valor de Manager.

**Returns:**
java.lang.String - un valor de Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Obtiene un valor que indica si MicrosoftProjectServerURL está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Obtiene un valor de MinutesPerDay.

**Returns:**
int - un valor de MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Obtiene un valor de MinutesPerWeek.

**Returns:**
int - un valor de MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Obtiene un valor que indica si MoveCompletedEndsBack está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Obtiene un valor que indica si MoveCompletedEndsForward está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Obtiene un valor que indica si MoveRemainingStartsBack está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Obtiene un valor que indica si MoveRemainingStartsForward está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Obtiene un valor que indica si MultipleCriticalPaths está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Obtiene un valor de Name.

**Returns:**
java.lang.String - un valor de Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Obtiene un valor de NewTaskStartDate.

**Returns:**
int - un valor de NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Obtiene un valor que indica si NewTasksAreManual está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Obtiene un valor que indica si NewTasksEffortDriven está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Obtiene un valor que indica si NewTasksEstimated está configurado o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Obtiene una colección que contiene las instancias de la clase [OleObject](../../com.aspose.tasks/oleobject) que están vinculadas o incrustadas en este archivo de proyecto.

--------------------

Disponible solo para el formato de archivo mpp. Esta colección es de solo lectura excepto para la operación 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Obtiene el objeto OutlineCodeDefinitionCollection. La colección de definiciones de códigos de esquema asociadas a un proyecto.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Devuelve el recuento de páginas del proyecto que se renderizará usando el [Timescale](../../com.aspose.tasks/timescale) predeterminado (Días).

**Returns:**
int - Cantidad de páginas a renderizar.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Devuelve el recuento de páginas del proyecto que se renderizará usando las [SaveOptions](../../com.aspose.tasks/saveoptions) proporcionadas.

--------------------

&gt; ```
&gt; En este ejemplo se escribe en la consola la instancia de HtmlSaveOptions y el número de páginas en el HTML resultante.
&gt; ``````

  [C#]
Project project = new Project(@\"test.mpp\");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
public final int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
public final NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
public final boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
public final NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
public final NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
public final NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
public final Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
public final String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
public final NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
public final String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
public final Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
public final Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
public final String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
public final String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
public final NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
public final int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

