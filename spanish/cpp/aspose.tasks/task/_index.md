---
title: "Aspose::Tasks::Task clase"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks for C++"
description: "Representa una tarea en un proyecto."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Representa una tarea en un proyecto.

La Task representa una unidad atómica de trabajo.

Se puede usar Task para planificar un proyecto creando tareas y asignando los recursos apropiados a ellas. Las Tasks en un proyecto se organizan como una estructura de árbol jerárquico con raíz, con una tarea raíz y subárboles de tareas hijas.

Para construir un árbol de tareas se puede usar una colección especializada Aspose::Tasks::TaskCollection accediendo a la propiedad Project::RootTask, por ejemplo:

```cpp
Project project = new Project();
 
// agregar nuevas tareas
Task task1 = project.RootTask.Children.Add(); // a parent task with empty name is added
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserts a task before the childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));
 
// guardar el proyecto en uno de los formatos disponibles
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clone](./clone/) | Crea una copia completa de una tarea sin subtareas. |
| [Delete](./delete/) | Elimina una tarea de la colección de tareas del proyecto principal y todas sus asignaciones. |
| [Equals (2 overloads)](./equals/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [Get](./get/) | Devuelve el valor al que la propiedad está asignada en este contenedor. |
| [get_ActivityId](./get_activityid/) | Representa el campo de ID de actividad: el identificador único de una tarea utilizado por Primavera. (solo aplicable a proyectos Primavera). |
| [get_ActualCost](./get_actualcost/) | Obtiene un valor de ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Obtiene un valor de ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Obtiene un valor de ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Obtiene un valor de ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Obtiene un valor de ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Obtiene un valor de ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Obtiene un valor de ActualStart. |
| [get_ActualWork](./get_actualwork/) | Obtiene un valor de ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Obtiene un valor de ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Obtiene un valor de ACWP. |
| [get_Assignments](./get_assignments/) | Obtiene una colección de asignaciones de recursos para este objeto. |
| [get_Baselines](./get_baselines/) | Obtiene la colección de valores de referencia de la tarea. |
| [get_BCWP](./get_bcwp/) | Obtiene un valor de BCWP. |
| [get_BCWS](./get_bcws/) | Obtiene un valor de BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Obtiene un valor de BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Obtiene un valor de BudgetWork. |
| [get_Calendar](./get_calendar/) | Obtiene un valor de Calendar. |
| [get_Children](./get_children/) | Obtiene una colección de tareas hijas de este objeto. Objeto TaskCollection que representa tareas hijas. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Obtiene un valor de CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Obtiene un valor de CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Obtiene un valor de CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Obtiene un valor de ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Obtiene un valor de ConstraintType. |
| [get_Contact](./get_contact/) | Obtiene un valor de Contact. |
| [get_Cost](./get_cost/) | Obtiene un valor de Cost. |
| [get_CostVariance](./get_costvariance/) | Obtiene un valor de CostVariance. |
| [get_Created](./get_created/) | Obtiene un valor de Created. |
| [get_CV](./get_cv/) | Obtiene un valor de CV. |
| [get_Deadline](./get_deadline/) | Obtiene un valor de Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Obtiene un valor que indica si DisplayAsSummary está configurado o no. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Obtiene un valor que indica si DisplayOnTimeline está configurado o no. |
| [get_Duration](./get_duration/) | Obtiene un valor de Duration. |
| [get_DurationFormat](./get_durationformat/) | Obtiene un valor de DurationFormat. |
| [get_DurationText](./get_durationtext/) | Obtiene un valor de DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Obtiene un valor de DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Obtiene un valor de EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Obtiene un valor de EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Obtiene un valor de EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Obtiene el objeto ExtendedAttributeCollection que contiene los valores de un atributo extendido. |
| [get_ExternalId](./get_externalid/) | Obtiene un valor de ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Obtiene un valor de ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Obtiene o establece el identificador único de la tarea externa cuando la tarea es externa. |
| [get_Finish](./get_finish/) | Obtiene un valor de Finish. |
| [get_FinishSlack](./get_finishslack/) | Obtiene un valor de FinishSlack. |
| [get_FinishText](./get_finishtext/) | Obtiene un valor de FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Obtiene un valor de FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Obtiene un valor de FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Obtiene un valor de FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Obtiene un valor de FreeSlack. |
| [get_Guid](./get_guid/) | Obtiene un valor de Guid. |
| [get_HideBar](./get_hidebar/) | Obtiene un valor que indica si HideBar está configurado o no. |
| [get_Hyperlink](./get_hyperlink/) | Obtiene el título o texto explicativo de un hipervínculo asociado a una tarea. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Obtiene la dirección de un hipervínculo asociado a una tarea. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Obtiene la ubicación específica en un documento de un hipervínculo asociado a una tarea. |
| [get_Id](./get_id/) | Obtiene un valor de Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Obtiene un valor que indica si IgnoreResourceCalendar está configurado o no. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Obtiene un valor que indica si IgnoreWarnings está configurado o no. |
| [get_IsActive](./get_isactive/) | Obtiene un valor que indica si IsActive está configurado o no. |
| [get_IsCritical](./get_iscritical/) | Obtiene un valor que indica si IsCritical está configurado o no. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Obtiene un valor que indica si IsEffortDriven está configurado o no. |
| [get_IsEstimated](./get_isestimated/) | Obtiene un valor que indica si IsEstimated está configurado o no. |
| [get_IsExpanded](./get_isexpanded/) | Obtiene un valor que indica si IsExpanded está configurado o no. |
| [get_IsExternalTask](./get_isexternaltask/) | Obtiene un valor que indica si IsExternalTask está configurado o no. |
| [get_IsManual](./get_ismanual/) | Obtiene un valor que indica si IsManual está configurado o no. |
| [get_IsMarked](./get_ismarked/) | Obtiene un valor que indica si IsMarked está configurado o no. |
| [get_IsMilestone](./get_ismilestone/) | Obtiene un valor que indica si IsMilestone está configurado o no. |
| [get_IsNull](./get_isnull/) | Obtiene un valor que indica si IsNull está establecido o no. |
| [get_IsOverallocated](./get_isoverallocated/) | Obtiene un valor que indica si IsOverallocated está configurado o no. |
| [get_IsPublished](./get_ispublished/) | Obtiene un valor que indica si IsPublished está configurado o no. |
| [get_IsRecurring](./get_isrecurring/) | Obtiene un valor que indica si IsRecurring está configurado o no. |
| [get_IsResumeValid](./get_isresumevalid/) | Obtiene un valor que indica si IsResumeValid está configurado o no. |
| [get_IsRollup](./get_isrollup/) | Obtiene un valor que indica si IsRollup está establecido o no. |
| [get_IsSubproject](./get_issubproject/) | Obtiene un valor que indica si IsSubproject está establecido o no. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Obtiene un valor que indica si IsSubprojectReadOnly está establecido o no. |
| [get_IsSummary](./get_issummary/) | Obtiene un valor que indica si IsSummary está establecido o no. |
| [get_LateFinish](./get_latefinish/) | Obtiene un valor de LateFinish. |
| [get_LateStart](./get_latestart/) | Obtiene un valor de LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Obtiene un valor que indica si LevelAssignments está establecido o no. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Obtiene un valor que indica si LevelingCanSplit está establecido o no. |
| [get_LevelingDelay](./get_levelingdelay/) | Obtiene un valor de LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Obtiene un valor de ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Obtiene un valor de ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Obtiene un valor de ManualStart. |
| [get_Name](./get_name/) | Obtiene un valor de Name. |
| [get_NotesRTF](./get_notesrtf/) | Obtiene un valor de NotesRTF. |
| [get_NotesText](./get_notestext/) | Obtiene un valor de NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Obtiene el objeto OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Obtiene un valor de OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Obtiene un valor de OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Obtiene un valor de OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Obtiene un valor de OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Obtiene el proyecto principal de una tarea. |
| [get_ParentTask](./get_parenttask/) | Obtiene la tarea principal de una tarea. |
| [get_PercentComplete](./get_percentcomplete/) | Obtiene un valor de PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Obtiene un valor de PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Obtiene un valor de PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Obtiene un objeto TaskCollection que contiene todos los predecesores de este objeto Task. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Obtiene un valor de PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Obtiene un valor de PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Obtiene un objeto que contiene propiedades específicas de Primavera para una tarea leída del archivo Primavera. |
| [get_Priority](./get_priority/) | Obtiene un valor de Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Obtiene la instancia de la clase RecurringTaskInfo para la tarea que es una tarea recurrente; si la tarea no es recurrente, devuelve null; |
| [get_RegularWork](./get_regularwork/) | Obtiene un valor de RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Obtiene un valor de RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Obtiene un valor de RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Obtiene un valor de RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Obtiene un valor de RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Obtiene un valor de RemainingWork. |
| [get_Resume](./get_resume/) | Obtiene un valor de Resume. |
| [get_SplitParts](./get_splitparts/) | Obtiene una colección SplitPart que representa las porciones de una tarea. |
| [get_Start](./get_start/) | Obtiene un valor de Start. |
| [get_StartSlack](./get_startslack/) | Obtiene un valor de StartSlack. |
| [get_StartText](./get_starttext/) | Obtiene un valor de StartText. |
| [get_StartVariance](./get_startvariance/) | Obtiene un valor de StartVariance. |
| [get_Status](./get_status/) | Obtiene el estado de la tarea. |
| [get_StatusManager](./get_statusmanager/) | Obtiene un valor de StatusManager. |
| [get_Stop](./get_stop/) | Obtiene un valor de Stop. |
| [get_SubprojectName](./get_subprojectname/) | Obtiene un valor de SubprojectName. |
| [get_Successors](./get_successors/) | Obtiene un objeto TaskCollection que contiene todos los sucesores de este objeto Task. |
| [get_SV](./get_sv/) | La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. La variación del cronograma (SV) es la diferencia entre el BCWP y el BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Obtiene un objeto TimephasedDataCollection de esta tarea. El bloque de datos por fases de tiempo asociado a una tarea. |
| [get_TotalSlack](./get_totalslack/) | Obtiene un valor de TotalSlack. |
| [get_Type](./get_type/) | Obtiene un valor de Type. |
| [get_Uid](./get_uid/) | Obtiene un valor de Uid. |
| [get_Warning](./get_warning/) | Obtiene un valor que indica si Warning está configurado o no. |
| [get_WBS](./get_wbs/) | Obtiene un valor de WBS. |
| [get_WBSLevel](./get_wbslevel/) | Obtiene un valor de WBSLevel. |
| [get_Work](./get_work/) | Obtiene un valor de Work. |
| [get_WorkVariance](./get_workvariance/) | Obtiene un valor de WorkVariance. |
| [GetHashCode](./gethashcode/) | Devuelve un valor de código hash para este Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Devuelve un objeto TimephasedDataCollection con valores TimephasedData dentro de las fechas de inicio y fin dadas. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Mueve la tarea actual al mismo nivel de esquema antes de la tarea especificada. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y campos de costo, niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, recalcula ids y niveles de esquema). |
| [OutlineIndent](./outlineindent/) | Identa una tarea en el esquema. |
| [OutlineOutdent](./outlineoutdent/) | Promueve una tarea en el esquema. |
| [SelectAllChildTasks](./selectallchildtasks/) | Recopila recursivamente todas las tareas hijas de esta tarea. |
| [Set](./set/) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [set_ActivityId](./set_activityid/) | Representa el campo de ID de actividad: el identificador único de una tarea utilizado por Primavera. (solo aplicable a proyectos Primavera). |
| [set_ActualCost](./set_actualcost/) | Establece un valor de ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Establece un valor de ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Establece un valor de ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Establece un valor de ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Establece un valor de ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Establece un valor de ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Establece un valor de ActualStart. |
| [set_ActualWork](./set_actualwork/) | Establece un valor de ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Establece un valor de ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Establece un valor de ACWP. |
| [set_Baselines](./set_baselines/) | Establece la colección de valores de línea base de la tarea. |
| [set_BCWP](./set_bcwp/) | Establece un valor de BCWP. |
| [set_BCWS](./set_bcws/) | Establece un valor de BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Establece un valor de BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Establece un valor de BudgetWork. |
| [set_Calendar](./set_calendar/) | Establece un valor de Calendar. |
| [set_CommitmentFinish](./set_commitmentfinish/) | Establece un valor de CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Establece un valor de CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Establece un valor de CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Establece un valor de ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Establece un valor de ConstraintType. |
| [set_Contact](./set_contact/) | Establece un valor de Contact. |
| [set_Cost](./set_cost/) | Establece un valor de Cost. |
| [set_CostVariance](./set_costvariance/) | Establece un valor de CostVariance. |
| [set_Created](./set_created/) | Establece un valor de Created. |
| [set_CV](./set_cv/) | Establece un valor de CV. |
| [set_Deadline](./set_deadline/) | Establece un valor de Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Establece un valor que indica si DisplayAsSummary está establecido o no. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Establece un valor que indica si DisplayOnTimeline está establecido o no. |
| [set_Duration](./set_duration/) | Establece un valor de Duration . |
| [set_DurationFormat](./set_durationformat/) | Establece un valor de DurationFormat. |
| [set_DurationText](./set_durationtext/) | Establece un valor de DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Establece un valor de DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Establece un valor de EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Establece un valor de EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Establece un valor de EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Establece un valor de ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Establece un valor de ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Obtiene o establece el identificador único de la tarea externa cuando la tarea es externa. |
| [set_Finish](./set_finish/) | Establece un valor de Finish. |
| [set_FinishSlack](./set_finishslack/) | Establece un valor de FinishSlack. |
| [set_FinishText](./set_finishtext/) | Establece un valor de FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Establece un valor de FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Establece un valor de FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Establece un valor de FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Establece un valor de FreeSlack. |
| [set_Guid](./set_guid/) | Establece un valor de Guid. |
| [set_HideBar](./set_hidebar/) | Establece un valor que indica si HideBar está establecido o no. |
| [set_Hyperlink](./set_hyperlink/) | Establece el título o texto explicativo para un hipervínculo asociado a una tarea. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Establece la dirección para un hipervínculo asociado a una tarea. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Establece la ubicación específica en un documento en un hipervínculo asociado a una tarea. |
| [set_Id](./set_id/) | Establece un valor de Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Establece un valor que indica si IgnoreResourceCalendar está establecido o no. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Establece un valor que indica si IgnoreWarnings está establecido o no. |
| [set_IsActive](./set_isactive/) | Establece un valor que indica si IsActive está establecido o no. |
| [set_IsCritical](./set_iscritical/) | Establece un valor que indica si IsCritical está establecido o no. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Establece un valor que indica si IsEffortDriven está establecido o no. |
| [set_IsEstimated](./set_isestimated/) | Establece un valor que indica si IsEstimated está establecido o no. |
| [set_IsExpanded](./set_isexpanded/) | Establece un valor que indica si IsExpanded está establecido o no. |
| [set_IsExternalTask](./set_isexternaltask/) | Establece un valor que indica si IsExternalTask está establecido o no. |
| [set_IsManual](./set_ismanual/) | Establece un valor que indica si IsManual está establecido o no. |
| [set_IsMarked](./set_ismarked/) | Establece un valor que indica si IsMarked está establecido o no. |
| [set_IsMilestone](./set_ismilestone/) | Establece un valor que indica si IsMilestone está establecido o no. |
| [set_IsNull](./set_isnull/) | Establece un valor que indica si IsNull está establecido o no. |
| [set_IsOverallocated](./set_isoverallocated/) | Establece un valor que indica si IsOverallocated está establecido o no. |
| [set_IsPublished](./set_ispublished/) | Establece un valor que indica si IsPublished está establecido o no. |
| [set_IsRecurring](./set_isrecurring/) | Establece un valor que indica si IsRecurring está establecido o no. |
| [set_IsResumeValid](./set_isresumevalid/) | Establece un valor que indica si IsResumeValid está establecido o no. |
| [set_IsRollup](./set_isrollup/) | Establece un valor que indica si IsRollup está establecido o no. |
| [set_IsSubproject](./set_issubproject/) | Establece un valor que indica si IsSubproject está establecido o no. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Establece un valor que indica si IsSubprojectReadOnly está establecido o no. |
| [set_IsSummary](./set_issummary/) | Establece un valor que indica si IsSummary está establecido o no. |
| [set_LateFinish](./set_latefinish/) | Establece un valor de LateFinish. |
| [set_LateStart](./set_latestart/) | Establece un valor de LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Establece un valor que indica si LevelAssignments está establecido o no. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Establece un valor que indica si LevelingCanSplit está establecido o no. |
| [set_LevelingDelay](./set_levelingdelay/) | Establece un valor de LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Establece un valor de ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Establece un valor de ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Establece un valor de ManualStart. |
| [set_Name](./set_name/) | Establece un valor de Name. |
| [set_NotesRTF](./set_notesrtf/) | Establece un valor de NotesRTF. |
| [set_NotesText](./set_notestext/) | Establece un valor de NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Establece el objeto OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Establece un valor de OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Establece un valor de OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Establece un valor de OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Establece un valor de OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Establece un valor de PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Establece un valor de PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Establece un valor de PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Establece un valor de PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Establece un valor de PreleveledStart. |
| [set_Priority](./set_priority/) | Establece un valor de Priority. |
| [set_RegularWork](./set_regularwork/) | Establece un valor de RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Establece un valor de RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Establece un valor de RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Establece un valor de RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Establece un valor de RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Establece un valor de RemainingWork. |
| [set_Resume](./set_resume/) | Establece un valor de Resume. |
| [set_Start](./set_start/) | Establece un valor de Start. |
| [set_StartSlack](./set_startslack/) | Establece un valor de StartSlack. |
| [set_StartText](./set_starttext/) | Establece un valor de StartText. |
| [set_StartVariance](./set_startvariance/) | Establece un valor de StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Establece un valor de StatusManager. |
| [set_Stop](./set_stop/) | Establece un valor de Stop. |
| [set_SubprojectName](./set_subprojectname/) | Establece un valor de SubprojectName. |
| [set_SV](./set_sv/) | La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. La variación del cronograma (SV) es la diferencia entre el BCWP y el BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Establece un objeto TimephasedDataCollection de esta tarea. El bloque de datos por fases de tiempo asociado a una tarea. |
| [set_TotalSlack](./set_totalslack/) | Establece un valor de TotalSlack. |
| [set_Type](./set_type/) | Establece un valor de Type. |
| [set_Uid](./set_uid/) | Establece un valor de Uid. |
| [set_Warning](./set_warning/) | Establece un valor que indica si Warning está establecido o no. |
| [set_WBS](./set_wbs/) | Establece un valor de WBS. |
| [set_WBSLevel](./set_wbslevel/) | Establece un valor de WBSLevel. |
| [set_Work](./set_work/) | Establece un valor de Work. |
| [set_WorkVariance](./set_workvariance/) | Establece un valor de WorkVariance. |
| [ToString](./tostring/) | Devuelve una representación corta en forma de cadena de una tarea. Los detalles exactos de la representación no están especificados y pueden cambiar. |

