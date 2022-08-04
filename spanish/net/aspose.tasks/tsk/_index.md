---
title: Tsk
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Representa propiedades deTask./task objeto.
type: docs
weight: 2290
url: /es/net/aspose.tasks/tsk/
---
## Tsk class

Representa propiedades de[`Task`](../task) objeto.

```csharp
public static class Tsk
```

## Campos

| Nombre | Descripción |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid) | Representa el campo de identificación de actividad: el identificador único de una tarea utilizado por Primavera. (solo aplicable a proyectos Primavera). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost) | Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado con la tarea. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration) | El lapso de tiempo de trabajo real para una tarea, según la duración programada y el trabajo restante actual o el porcentaje completado. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish) | La fecha en que se completó una tarea. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost) | Costos incurridos por horas extras ya realizadas en tareas por recursos asignados. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework) | La cantidad real de horas extra ya realizadas por los recursos asignados a las tareas. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected) | La duración durante la cual se protege el trabajo de horas extra real.  Lectura admitida solo para formato XML. [`Duration`](./duration) tipo. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart) | La fecha y hora en que realmente comenzó una tarea. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork) | La cantidad de trabajo que ya han realizado los recursos asignados a las tareas. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected) | La duración a través de la cual se protege el trabajo real.  Lectura admitida solo para formato XML. [`Duration`](./duration) tipo. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp) | Costos incurridos por el trabajo ya realizado en una tarea, hasta la fecha de estado del proyecto o la fecha de hoy. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp) | El valor acumulativo del porcentaje completado de la tarea multiplicado por los costos de línea de base con fases de tiempo. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws) | Los costos de línea base acumulados por fases hasta la fecha de estado o la fecha de hoy. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost) | Costos presupuestarios para recursos de costo presupuestario. Los recursos del presupuesto se asignan solo a la tarea de resumen del proyecto. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork) | Trabajo presupuestario para trabajo presupuestario y recursos materiales. Los recursos del presupuesto se asignan solo a la tarea de resumen del proyecto. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar) | El calendario de tareas. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish) | La fecha de finalización de una entrega.  Lectura admitida solo para formato XML. DateTime escribe. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart) | La fecha de inicio de una entrega.  Lectura admitida solo para formato XML. DateTime escribe. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype) | Determina si una tarea tiene una entrega asociada o una dependencia de una entrega asociada.  Lectura admitida solo para formato XML. Int32 tipo. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate) | La fecha específica asociada con el tipo de restricción. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype) | Proporciona opciones para el tipo de restricción que se puede aplicar para programar una tarea. |
| static readonly [Contact](../../aspose.tasks/tsk/contact) | El nombre de una persona responsable de una tarea. |
| static readonly [Cost](../../aspose.tasks/tsk/cost) | El costo total programado o proyectado para una tarea en función de los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance) | La diferencia entre el costo de referencia y el costo total de una tarea, recurso o asignación. |
| static readonly [Created](../../aspose.tasks/tsk/created) | La fecha en que se creó una tarea. |
| static readonly [CV](../../aspose.tasks/tsk/cv) | La diferencia entre el costo de referencia y el costo total de una tarea. Variación de costo = Costo - Costo de referencia |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline) | Una fecha objetivo que indica cuándo se debe completar una tarea. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary) | Determina si la tarea debe mostrarse como una tarea de resumen.  Lectura admitida solo para formato XML. Boolean escribe. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline) | Especifica si una tarea debe mostrarse en una vista de línea de tiempo. |
| static readonly [Duration](../../aspose.tasks/tsk/duration) | El intervalo total de tiempo de trabajo activo para una tarea tal como se ingresa o calcula Microsoft Project según la fecha de inicio, la fecha de finalización, los calendarios y otros factores de programación. |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat) | Formato de duración de la tarea. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext) | Devuelve el texto de duración de la tarea. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance) | La diferencia entre la duración de referencia de una tarea y la duración total (estimación actual) de una tarea. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish) | La fecha más temprana en la que una tarea podría finalizar, según las fechas de finalización anticipadas de las tareas predecesoras y sucesoras, otras restricciones y cualquier retraso de nivelación. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart) | La fecha más temprana en la que una tarea podría comenzar, según las fechas de inicio tempranas de las tareas predecesoras y sucesoras y otras restricciones. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod) | Determina si se debe usar el campo % completado o % físico completo para calcular el costo presupuestado del trabajo realizado (BCWP). |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid) | Si una tarea es una tarea externa, contiene el Id. externo de la tarea. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject) | La ubicación de origen y el identificador de tarea de una tarea externa. |
| static readonly [Finish](../../aspose.tasks/tsk/finish) | La fecha de finalización programada de una tarea. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan) | La duración entre las fechas de finalización anticipada y finalización tardía. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext) | Devuelve el texto de finalización de la tarea. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance) | La hora que representa la diferencia entre la fecha de finalización de referencia de una tarea o asignación y su fecha de finalización actual. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost) | Muestra cualquier gasto de tarea que no sea de recursos. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual) | Determina opciones sobre cómo y cuándo se cargarán o acumularán costos fijos al costo de una tarea. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan) | El tiempo que se puede retrasar una tarea sin retrasar ninguna tarea sucesora. |
| static readonly [Guid](../../aspose.tasks/tsk/guid) | Los códigos de identificación únicos generados para una tarea. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource) | Indica si la tarea tiene un recurso asignado que tiene más trabajo en las tareas asignadas del que se puede completar dentro de la capacidad de trabajo normal. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar) | Determina si la barra de Gantt de una tarea está oculta cuando se muestra en Microsoft Project. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink) | El título o texto explicativo de un hipervínculo asociado a una tarea. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress) | La dirección de un hipervínculo asociado con una tarea. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress) | La ubicación específica en un documento en un hipervínculo asociado con una tarea. |
| static readonly [Id](../../aspose.tasks/tsk/id) | El identificador de posición de una tarea dentro de la lista de tareas. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar) | Determina si la programación de la tarea considera los calendarios de los recursos asignados a la tarea. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings) | Indica si ocultar el indicador de advertencia de conflicto de programación en Microsoft Project. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive) | Determina si una tarea está activa. Las tareas inactivas ya no afectan a otras tareas ni a la programación general del proyecto. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical) | Determina si una tarea se encuentra en la ruta crítica. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven) | Determina si la programación de la tarea es una programación basada en el esfuerzo. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated) | Determina si una tarea es estimada. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded) | Determina si una tarea de resumen se expande o no en la vista GanttChart. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask) | Determina si una tarea es externa. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual) | Determina si una tarea se programa manualmente. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked) | Muestra si una tarea está marcada para acción adicional o identificación de algún tipo. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone) | Determina si una tarea es un hito. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull) | Determina si una tarea es nula. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated) | Indica si alguno de los recursos asignados a una tarea está asignado a más trabajo en la tarea del que se puede realizar con la capacidad de trabajo normal. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished) | Determina si la tarea actual debe publicarse en Project Server con el resto del proyecto. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring) | Determina si una tarea es parte de una serie de tareas recurrentes. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid) | Determina si se puede reanudar una tarea. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup) | Determina si la información sobre las barras de Gantt de subtareas se acumulará en la barra de tareas de resumen. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject) | Determina si una tarea es un proyecto insertado. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly) | Determina si un subproyecto es de solo lectura. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary) | Determina si una tarea es una tarea de resumen. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish) | La última fecha en la que una tarea puede finalizar sin retrasar la finalización del proyecto. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart) | La última fecha en la que una tarea puede comenzar sin retrasar la finalización del proyecto. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments) | Determina si la función de nivelación puede retrasar y dividir asignaciones individuales para resolver asignaciones excesivas. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit) | Determina si la función de nivelación de recursos puede causar divisiones en el trabajo restante de esta tarea. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay) | El tiempo que se retrasará una tarea desde su fecha de inicio anticipada debido a la nivelación de recursos. |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat) | El formato para expresar la duración de un retraso. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration) | Define la duración programada manualmente de una tarea. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish) | Define el final programado manualmente de una tarea. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart) | Define el inicio programado manualmente de una tarea. |
| static readonly [Name](../../aspose.tasks/tsk/name) | Nombre de una tarea. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf) | Las notas de texto en formato RTF. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext) | Texto sin formato de notas extraído de datos RTF. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel) | El nivel de esquema de una tarea. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber) | El número que representa la posición de una tarea en la estructura de esquema jerárquico. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost) | El costo total de horas extra para una tarea, para un recurso en todas las tareas asignadas o para una asignación de recursos. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework) | La cantidad de horas extra programadas para que las realicen todos los recursos asignados a una tarea. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete) | El estado actual de una tarea, expresado como el porcentaje de la duración de la tarea que se ha completado. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete) | El estado actual de una tarea expresado como el porcentaje de trabajo que se ha completado. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete) | Porcentaje de valor completo que se puede usar como alternativa para calcular el costo presupuestado del trabajo realizado (BCWP). |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish) | La fecha de finalización de una tarea antes de que se realizara la nivelación de recursos. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart) | La fecha de inicio de una tarea antes de que se realizara la nivelación de recursos. |
| static readonly [Priority](../../aspose.tasks/tsk/priority) | El nivel de importancia otorgado a una tarea, que a su vez indica con qué facilidad se puede retrasar o dividir una tarea o asignación durante la nivelación de recursos. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork) | La cantidad total de trabajo que no es de horas extra programado para ser realizado por los recursos. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost) | El gasto programado restante en el que se incurrirá para completar el trabajo programado restante. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration) | El tiempo que se requiere para completar la parte inconclusa de una tarea. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost) | El gasto restante de horas extra programadas para una tarea. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework) | La cantidad de horas extra programadas restantes. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork) | El tiempo aún necesario para completar una tarea o conjunto de tareas. |
| static readonly [Resume](../../aspose.tasks/tsk/resume) | La fecha en que la parte restante de una tarea está programada para reanudarse después de ingresar cualquier progreso. |
| static readonly [Start](../../aspose.tasks/tsk/start) | La fecha de inicio programada de una tarea. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan) | La duración entre las fechas de Inicio temprano y Inicio tardío. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext) | Devuelve el texto de inicio de la tarea. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance) | El tiempo que representa la diferencia entre una fecha de inicio de referencia de una tarea o asignación y su fecha de inicio programada actualmente. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager) | El nombre del recurso empresarial que va a recibir actualizaciones de estado para la tarea actual de los recursos. |
| static readonly [Stop](../../aspose.tasks/tsk/stop) | La fecha que representa el final de la parte real de una tarea. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname) | La ubicación de origen de un subproyecto. |
| static readonly [SV](../../aspose.tasks/tsk/sv) | La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. La variación del cronograma (SV) es la diferencia entre el BCWP y el BCWS. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan) | El tiempo que se puede retrasar la fecha de finalización de una tarea sin retrasar la fecha de finalización del proyecto. |
| static readonly [Type](../../aspose.tasks/tsk/type) | El tipo de una tarea. |
| static readonly [Uid](../../aspose.tasks/tsk/uid) | La identificación única de una tarea. |
| static readonly [Warning](../../aspose.tasks/tsk/warning) | Representa el indicador que indica que la tarea tiene discrepancias en la programación. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs) | Códigos de estructura de descomposición del trabajo (WBS). |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel) | El nivel WBS más a la derecha de una tarea. |
| static readonly [Work](../../aspose.tasks/tsk/work) | El tiempo total programado en una tarea para todos los recursos asignados. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance) | La diferencia entre el trabajo de referencia de una tarea y el trabajo programado actualmente. |

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
