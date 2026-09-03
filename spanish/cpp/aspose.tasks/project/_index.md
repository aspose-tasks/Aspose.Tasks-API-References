---
title: "Clase Aspose::Tasks::Project"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks for C++"
description: "Representa un proyecto."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/project/
---

## Project class

Representa un proyecto.

El Project es una clase central en la biblioteca Aspose.Tasks.

Se puede usar Project para leer uno de los formatos de gestión de proyectos compatibles: MPP, MPT, MPX, XML.

Para cargar un documento existente en cualquiera de los formatos compatibles, pase un nombre de archivo o un flujo a uno de los constructores de Project. Para crear un proyecto vacío, llame al constructor sin parámetros.

Utilice una de las sobrecargas del método Save para guardar el proyecto en cualquiera de los formatos Aspose::Tasks::Saving::SaveFileFormat: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Diseño fijo: PDF; Imágenes: JPEG, PNG, BMP, TIFF, SVG; Texto: TXT; Otros: HTML.

Project almacena información a nivel de proyecto como Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps y Aspose::Tasks::Project::ExtendedAttributes. La mayoría de estos objetos son accesibles a través de las propiedades correspondientes de la clase Project.

Project es una entidad raíz que contiene puntos de entrada para manipular otras entidades del proyecto, como Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute y Aspose::Tasks::Calendar.

Las entidades de Project pueden accederse a través de colecciones tipadas, por ejemplo Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments, etc.

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Project (13 overloads)](./project/) | Inicializa una nueva instancia de la clase Project. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Copia los datos principales y las propiedades del proyecto a otro proyecto. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Enumera recursivamente todas las tareas del proyecto, incluida la tarea raíz. |
| [Get](./get/) | Devuelve el valor al que la propiedad está asignada en este contenedor. |
| [get_ActualsInSync](./get_actualsinsync/) | Obtiene un valor que indica si ActualsInSync está establecido o no. |
| [get_AdminProject](./get_adminproject/) | Obtiene un valor que indica si AdminProject está establecido o no. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Obtiene un valor que indica si AreEditableActualCosts está establecido o no. |
| [get_Author](./get_author/) | Obtiene el valor de Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Obtiene un valor que indica si AutoAddNewResourcesAndTasks está establecido o no. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Obtiene si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos. |
| [get_Autolink](./get_autolink/) | Obtiene un valor que indica si Autolink está establecido o no. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Obtiene el valor de BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Obtiene la colección de propiedades integradas del proyecto. |
| [get_CalculationMode](./get_calculationmode/) | Obtiene el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración CalculationMode. |
| [get_Calendar](./get_calendar/) | Obtiene un valor de Calendar. |
| [get_Calendars](./get_calendars/) | Obtiene el objeto CalendarCollection de esta instancia de Project. |
| [get_Category](./get_category/) | Obtiene el valor de Category. |
| [get_Comments](./get_comments/) | Obtiene el valor de Comments. |
| [get_Company](./get_company/) | Obtiene el valor de Company. |
| [get_CreationDate](./get_creationdate/) | Obtiene el valor de CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Obtiene una colección que contiene una lista de tareas Critical que componen la ruta crítica de este proyecto. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Obtiene un valor de CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Obtiene un valor de CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Obtiene un valor de CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Obtiene un valor de CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Obtiene un valor de CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Obtiene un valor de CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Obtiene un valor de CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Obtiene la colección de propiedades personalizadas del proyecto. |
| [get_DateFormat](./get_dateformat/) | Obtiene un valor de DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Obtiene un valor de DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Obtiene un valor de DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Obtiene un valor de DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Obtiene un valor de DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Obtiene un valor de DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Obtiene un valor de DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Obtiene un valor de DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Obtiene un valor de DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Obtiene la vista predeterminada del proyecto. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Obtiene la instancia de la clase WeekDayCollection que representa una colección de los días laborables semanales predeterminados del proyecto y sus horarios de trabajo. |
| [get_DisplayOptions](./get_displayoptions/) | Obtiene una instancia de la clase ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Obtiene un valor de DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Obtiene un valor de EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de atributos extendidos (campos personalizados) asociados a un proyecto. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Obtiene un valor de ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Obtiene un valor de FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Obtiene un valor que indica si FiscalYearStart está configurado o no. |
| [get_FyStartDate](./get_fystartdate/) | Obtiene un valor de FyStartDate. |
| [get_Guid](./get_guid/) | Obtiene un valor de Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Obtiene un valor que indica si HonorConstraints está configurado o no. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Obtiene un valor de HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Obtiene un valor que indica si InsertedProjectsLikeSummary está configurado o no. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Obtiene un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no. |
| [get_Keywords](./get_keywords/) | Obtiene un valor de Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Obtiene un valor de LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Obtiene un valor de LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Obtiene un valor de LastSaved. |
| [get_Manager](./get_manager/) | Obtiene un valor de Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Obtiene un valor que indica si MicrosoftProjectServerURL está configurado o no. |
| [get_MinutesPerDay](./get_minutesperday/) | Obtiene un valor de MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Obtiene un valor de MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Obtiene un valor que indica si MoveCompletedEndsBack está configurado o no. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Obtiene un valor que indica si MoveCompletedEndsForward está configurado o no. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Obtiene un valor que indica si MoveRemainingStartsBack está configurado o no. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Obtiene un valor que indica si MoveRemainingStartsForward está configurado o no. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Obtiene un valor que indica si MultipleCriticalPaths está configurado o no. |
| [get_Name](./get_name/) | Obtiene un valor de Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Obtiene un valor que indica si NewTasksAreManual está configurado o no. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Obtiene un valor que indica si NewTasksEffortDriven está configurado o no. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Obtiene un valor que indica si NewTasksEstimated está configurado o no. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Obtiene un valor de NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Obtiene una colección que contiene las instancias de la clase OleObject que están vinculadas o incrustadas a este archivo de proyecto. |
| [get_OutlineCodes](./get_outlinecodes/) | Obtiene el objeto OutlineCodeDefinitionCollection. La colección de definiciones de códigos de esquema asociadas a un proyecto. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Obtiene un objeto que contiene propiedades específicas de Primavera para un proyecto leído del archivo Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Obtiene un valor que indica si ProjectExternallyEdited está establecido o no. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Obtiene un valor que indica si RemoveFileProperties está establecido o no. |
| [get_ResourceAssignments](./get_resourceassignments/) | Obtiene el objeto ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Obtiene todas las definiciones de filtros basados en recursos. ResourceFilters es una colección de objetos Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Obtiene todas las definiciones de grupos basados en recursos. ResourceGroups es una colección de objetos Group. |
| [get_Resources](./get_resources/) | Obtiene el objeto ResourceCollection. |
| [get_Revision](./get_revision/) | Obtiene un valor de Revision. |
| [get_RootTask](./get_roottask/) | Obtiene la raíz del árbol de tareas. |
| [get_SaveVersion](./get_saveversion/) | Obtiene un valor de SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Obtiene un valor que indica si ScheduleFromStart está establecido o no. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Obtiene un valor que indica si ShowProjectSummaryTask está establecido o no. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Obtiene un valor que indica si SplitsInProgressTasks está establecido o no. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Obtiene un valor que indica si SpreadActualCost está establecido o no. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Obtiene un valor que indica si SpreadPercentComplete está establecido o no. |
| [get_StartDate](./get_startdate/) | Obtiene un valor de StartDate. |
| [get_StatusDate](./get_statusdate/) | Obtiene un valor de StatusDate. |
| [get_Subject](./get_subject/) | Obtiene un valor de Subject. |
| [get_Tables](./get_tables/) | Obtiene una lista de objetos Table. |
| [get_TaskFilters](./get_taskfilters/) | Obtiene todas las definiciones de filtros basados en tareas. TaskFilters es una colección de objetos Filter. |
| [get_TaskGroups](./get_taskgroups/) | Obtiene todas las definiciones de grupos basados en tareas. TaskGroups es una colección de objetos Group. |
| [get_TaskLinks](./get_tasklinks/) | Obtiene el objeto TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Obtiene un valor que indica si TaskUpdatesResource está establecido o no. |
| [get_Template](./get_template/) | Obtiene un valor de Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Obtiene un valor de TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Obtiene un valor de TimescaleStart. |
| [get_Title](./get_title/) | Obtiene un valor de Title. |
| [get_Uid](./get_uid/) | Obtiene un valor de Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Obtiene un valor que indica si UpdateManuallyScheduledTasksWhenEditingLinks está configurado o no. |
| [get_VbaProject](./get_vbaproject/) | Obtiene una instancia de la clase VbaProject. |
| [get_Views](./get_views/) | Obtiene una lista de objetos View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Obtiene la definición del código WBS para el proyecto. |
| [get_WeekStartDay](./get_weekstartday/) | Obtiene un valor de WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Obtiene un valor de WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Devuelve la hora de guardado de la línea base. |
| [GetDuration (3 overloads)](./getduration/) | Obtiene un objeto Duration con el número especificado de unidades y el formato de duración predeterminado que está definido en la configuración del proyecto Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Devuelve el recuento de páginas del proyecto que se renderizará usando la escala de tiempo predeterminada (Días). |
| [GetPredecessors](./getpredecessors/) | Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Obtiene la información del archivo del proyecto desde el flujo. |
| [GetWork](./getwork/) | Obtiene un objeto Duration con el valor double especificado y el formato de trabajo predeterminado. |
| [Recalculate (2 overloads)](./recalculate/) | Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Recalcula el Id, Inicio y Fin de los recursos. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Recalcula el Inicio y Fin de los recursos. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Elimina asignaciones de recursos inválidas de la lista de asignaciones de recursos del proyecto. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Renumera el código WBS de todas las tareas. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Reprograma el trabajo del proyecto no completado para que comience después de una fecha especificada. |
| [Save (5 overloads)](./save/) | Guarda el proyecto en un flujo usando las opciones de guardado especificadas. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Guarda el proyecto como una plantilla en un flujo especificado. |
| [SaveReport (4 overloads)](./savereport/) | Guarda el informe de visión general del proyecto en el flujo. |
| [SelectAllChildTasks](./selectallchildtasks/) | Recopila recursivamente todas las tareas hijas de la tarea raíz. |
| [Set (2 overloads)](./set/) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [set_ActualsInSync](./set_actualsinsync/) | Establece un valor que indica si ActualsInSync está configurado o no. |
| [set_AdminProject](./set_adminproject/) | Establece un valor que indica si AdminProject está configurado o no. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Establece un valor que indica si AreEditableActualCosts está configurado o no. |
| [set_Author](./set_author/) | Establece un valor de Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Establece un valor que indica si AutoAddNewResourcesAndTasks está configurado o no. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Establece si el costo de la asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos. |
| [set_Autolink](./set_autolink/) | Establece un valor que indica si Autolink está configurado o no. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Establece un valor de BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Establece el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración CalculationMode. |
| [set_Calendar](./set_calendar/) | Establece un valor de Calendar. |
| [set_Category](./set_category/) | Establece un valor de Category. |
| [set_Comments](./set_comments/) | Establece un valor de Comments. |
| [set_Company](./set_company/) | Establece un valor de Company. |
| [set_CreationDate](./set_creationdate/) | Establece un valor de CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Establece un valor de CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Establece un valor de CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Establece un valor de CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Establece un valor de CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Establece un valor de CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Establece un valor de CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Establece un valor de CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Establece un valor de DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Establece un valor de DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Establece un valor de DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Establece un valor de DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Establece un valor de DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Establece un valor de DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Establece un valor de DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Establece un valor de DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Establece un valor de DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Establece la vista predeterminada del proyecto. |
| [set_DurationFormat](./set_durationformat/) | Establece un valor de DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Establece un valor de EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Establece un valor de ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Establece un valor de FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Establece un valor que indica si FiscalYearStart está configurado o no. |
| [set_FyStartDate](./set_fystartdate/) | Establece un valor de FyStartDate. |
| [set_Guid](./set_guid/) | Establece un valor de Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Establece un valor que indica si HonorConstraints está configurado o no. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Establece un valor de HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Establece un valor que indica si InsertedProjectsLikeSummary está configurado o no. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Establece un valor que indica si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled está configurado o no. |
| [set_Keywords](./set_keywords/) | Establece un valor de Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Establece un valor de LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Establece un valor de LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Establece un valor de LastSaved. |
| [set_Manager](./set_manager/) | Establece un valor de Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Establece un valor que indica si MicrosoftProjectServerURL está configurado o no. |
| [set_MinutesPerDay](./set_minutesperday/) | Establece un valor de MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Establece un valor de MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Establece un valor que indica si MoveCompletedEndsBack está configurado o no. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Establece un valor que indica si MoveCompletedEndsForward está configurado o no. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Establece un valor que indica si MoveRemainingStartsBack está configurado o no. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Establece un valor que indica si MoveRemainingStartsForward está configurado o no. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Establece un valor que indica si MultipleCriticalPaths está configurado o no. |
| [set_Name](./set_name/) | Establece un valor de Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Establece un valor que indica si NewTasksAreManual está configurado o no. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Establece un valor que indica si NewTasksEffortDriven está configurado o no. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Establece un valor que indica si NewTasksEstimated está configurado o no. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Establece un valor de NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Establece un valor que indica si ProjectExternallyEdited está configurado o no. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Establece un valor que indica si RemoveFileProperties está configurado o no. |
| [set_Revision](./set_revision/) | Establece un valor de Revision. |
| [set_SaveVersion](./set_saveversion/) | Establece un valor de SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Establece un valor que indica si ScheduleFromStart está configurado o no. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Establece un valor que indica si ShowProjectSummaryTask está configurado o no. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Establece un valor que indica si SplitsInProgressTasks está configurado o no. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Establece un valor que indica si SpreadActualCost está configurado o no. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Establece un valor que indica si SpreadPercentComplete está configurado o no. |
| [set_StartDate](./set_startdate/) | Establece un valor de StartDate. |
| [set_StatusDate](./set_statusdate/) | Establece un valor de StatusDate. |
| [set_Subject](./set_subject/) | Establece un valor de Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Establece un valor que indica si TaskUpdatesResource está configurado o no. |
| [set_Template](./set_template/) | Establece un valor de Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Establece un valor de TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Establece un valor de TimescaleStart. |
| [set_Title](./set_title/) | Establece un valor de Title. |
| [set_Uid](./set_uid/) | Establece un valor de Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Establece un valor que indica si UpdateManuallyScheduledTasksWhenEditingLinks está configurado o no. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Establece la definición del código WBS para el proyecto. |
| [set_WeekStartDay](./set_weekstartday/) | Establece un valor de WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Establece un valor de WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Guarda los campos de línea base en la línea base especificada para todo el proyecto. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Establece la hora de guardado de la línea base. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Actualiza todo el trabajo como completado hasta una fecha especificada para todo el proyecto. |

