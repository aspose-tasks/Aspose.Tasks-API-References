---
title: "فئة Aspose::Tasks::Task"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks لـ C++"
description: "يمثل مهمة في Project."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

يمثل مهمة في Project.

الـ Task يمثل جزءًا ذريًا واحدًا من العمل.

يمكن للمرء استخدام Task لتخطيط مشروع عن طريق إنشاء مهام وتعيين الموارد المناسبة إليها. تُنظم المهام في المشروع كهيكل شجري هرمي جذري، مع مهمة جذرية وفروع من المهام الفرعية.

لبناء شجرة من المهام يمكن استخدام مجموعة متخصصة Aspose::Tasks::TaskCollection عبر الوصول إلى خاصية Project::RootTask على سبيل المثال:

```cpp
Project project = new Project();
 
// إضافة مهام جديدة
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
 
// احفظ المشروع بأحد الصيغ المتاحة
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clone](./clone/) | ينشئ نسخة كاملة من مهمة دون المهام الفرعية. |
| [Delete](./delete/) | يحذف مهمة من مجموعة مهام المشروع الأصلية وجميع تعييناتها. |
| [Equals (2 overloads)](./equals/) | يرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن محدد. |
| [Get](./get/) | يعيد القيمة التي تم ربط الخاصية بها في هذا الحاوية. |
| [get_ActivityId](./get_activityid/) | يمثل حقل معرف النشاط - معرف فريد للمهمة يستخدمه Primavera. (ينطبق فقط على مشاريع Primavera). |
| [get_ActualCost](./get_actualcost/) | يحصل على قيمة ActualCost. |
| [get_ActualDuration](./get_actualduration/) | يحصل على قيمة ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | يحصل على قيمة ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | يحصل على قيمة ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | يحصل على قيمة ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | يحصل على قيمة ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | يحصل على قيمة ActualStart. |
| [get_ActualWork](./get_actualwork/) | يحصل على قيمة ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | يحصل على قيمة ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | يحصل على قيمة ACWP. |
| [get_Assignments](./get_assignments/) | يحصل على مجموعة من تعيينات الموارد لهذا الكائن. |
| [get_Baselines](./get_baselines/) | يحصل على مجموعة القيم الأساسية للمهمة. |
| [get_BCWP](./get_bcwp/) | يحصل على قيمة BCWP. |
| [get_BCWS](./get_bcws/) | يحصل على قيمة BCWS. |
| [get_BudgetCost](./get_budgetcost/) | يحصل على قيمة BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | يحصل على قيمة BudgetWork. |
| [get_Calendar](./get_calendar/) | يحصل على قيمة Calendar. |
| [get_Children](./get_children/) | يحصل على مجموعة المهام الفرعية لهذا الكائن. كائن TaskCollection الذي يمثل مهام الأطفال. |
| [get_CommitmentFinish](./get_commitmentfinish/) | يحصل على قيمة CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | يحصل على قيمة CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | يحصل على قيمة CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | يحصل على قيمة ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | يحصل على قيمة ConstraintType. |
| [get_Contact](./get_contact/) | يحصل على قيمة Contact. |
| [get_Cost](./get_cost/) | يحصل على قيمة Cost. |
| [get_CostVariance](./get_costvariance/) | يحصل على قيمة CostVariance. |
| [get_Created](./get_created/) | يحصل على قيمة Created. |
| [get_CV](./get_cv/) | يحصل على قيمة CV. |
| [get_Deadline](./get_deadline/) | يحصل على قيمة Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | يحصل على قيمة تشير إلى ما إذا كان DisplayAsSummary مضبوطًا أم لا. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | يحصل على قيمة تشير إلى ما إذا كان DisplayOnTimeline مضبوطًا أم لا. |
| [get_Duration](./get_duration/) | يحصل على قيمة Duration. |
| [get_DurationFormat](./get_durationformat/) | يحصل على قيمة DurationFormat. |
| [get_DurationText](./get_durationtext/) | يحصل على قيمة DurationText. |
| [get_DurationVariance](./get_durationvariance/) | يحصل على قيمة DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | يحصل على قيمة EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | يحصل على قيمة EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | يحصل على قيمة EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | يحصل على كائن ExtendedAttributeCollection الذي يحتوي على قيم سمة موسعة. |
| [get_ExternalId](./get_externalid/) | يحصل على قيمة ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | يحصل على قيمة ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | يحصل أو يضبط المعرف الفريد للمهمة الخارجية عندما تكون المهمة خارجية. |
| [get_Finish](./get_finish/) | يحصل على قيمة Finish. |
| [get_FinishSlack](./get_finishslack/) | يحصل على قيمة FinishSlack. |
| [get_FinishText](./get_finishtext/) | يحصل على قيمة FinishText. |
| [get_FinishVariance](./get_finishvariance/) | يحصل على قيمة FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | يحصل على قيمة FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | يحصل على قيمة FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | يحصل على قيمة FreeSlack. |
| [get_Guid](./get_guid/) | يحصل على قيمة Guid. |
| [get_HideBar](./get_hidebar/) | يحصل على قيمة تشير إلى ما إذا كان HideBar مضبوطًا أم لا. |
| [get_Hyperlink](./get_hyperlink/) | يحصل على العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمهمة. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | يحصل على العنوان لرابط تشعبي مرتبط بمهمة. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | يحصل على الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمهمة. |
| [get_Id](./get_id/) | يحصل على قيمة Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | يحصل على قيمة تشير إلى ما إذا كان IgnoreResourceCalendar مضبوطًا أم لا. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | يحصل على قيمة تشير إلى ما إذا كان IgnoreWarnings مضبوطًا أم لا. |
| [get_IsActive](./get_isactive/) | يحصل على قيمة تشير إلى ما إذا كان IsActive مضبوطًا أم لا. |
| [get_IsCritical](./get_iscritical/) | يحصل على قيمة تشير إلى ما إذا كان IsCritical مضبوطًا أم لا. |
| [get_IsEffortDriven](./get_iseffortdriven/) | يحصل على قيمة تشير إلى ما إذا كان IsEffortDriven مضبوطًا أم لا. |
| [get_IsEstimated](./get_isestimated/) | يحصل على قيمة تشير إلى ما إذا كان IsEstimated مضبوطًا أم لا. |
| [get_IsExpanded](./get_isexpanded/) | يحصل على قيمة تشير إلى ما إذا كان IsExpanded مضبوطًا أم لا. |
| [get_IsExternalTask](./get_isexternaltask/) | يحصل على قيمة تشير إلى ما إذا كان IsExternalTask مضبوطًا أم لا. |
| [get_IsManual](./get_ismanual/) | يحصل على قيمة تشير إلى ما إذا كان IsManual مضبوطًا أم لا. |
| [get_IsMarked](./get_ismarked/) | يحصل على قيمة تشير إلى ما إذا كان IsMarked مضبوطًا أم لا. |
| [get_IsMilestone](./get_ismilestone/) | يحصل على قيمة تشير إلى ما إذا كان IsMilestone مضبوطًا أم لا. |
| [get_IsNull](./get_isnull/) | يحصل على قيمة تشير إلى ما إذا كان IsNull مضبوطًا أم لا. |
| [get_IsOverallocated](./get_isoverallocated/) | يحصل على قيمة تشير إلى ما إذا كان IsOverallocated مضبوطًا أم لا. |
| [get_IsPublished](./get_ispublished/) | يحصل على قيمة تشير إلى ما إذا كان IsPublished مضبوطًا أم لا. |
| [get_IsRecurring](./get_isrecurring/) | يحصل على قيمة تشير إلى ما إذا كان IsRecurring مضبوطًا أم لا. |
| [get_IsResumeValid](./get_isresumevalid/) | يحصل على قيمة تشير إلى ما إذا كان IsResumeValid مضبوطًا أم لا. |
| [get_IsRollup](./get_isrollup/) | يحصل على قيمة تشير إلى ما إذا كان IsRollup مضبوطًا أم لا. |
| [get_IsSubproject](./get_issubproject/) | يحصل على قيمة تشير إلى ما إذا كان IsSubproject مضبوطًا أم لا. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | يحصل على قيمة تشير إلى ما إذا كان IsSubprojectReadOnly مضبوطًا أم لا. |
| [get_IsSummary](./get_issummary/) | يحصل على قيمة تشير إلى ما إذا كان IsSummary مضبوطًا أم لا. |
| [get_LateFinish](./get_latefinish/) | يحصل على قيمة LateFinish. |
| [get_LateStart](./get_latestart/) | يحصل على قيمة LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | يحصل على قيمة تشير إلى ما إذا كان LevelAssignments مضبوطًا أم لا. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | يحصل على قيمة تشير إلى ما إذا كان LevelingCanSplit مضبوطًا أم لا. |
| [get_LevelingDelay](./get_levelingdelay/) | يحصل على قيمة LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | يحصل على قيمة ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | يحصل على قيمة ManualFinish. |
| [get_ManualStart](./get_manualstart/) | يحصل على قيمة ManualStart. |
| [get_Name](./get_name/) | يحصل على قيمة Name. |
| [get_NotesRTF](./get_notesrtf/) | يحصل على قيمة NotesRTF. |
| [get_NotesText](./get_notestext/) | يحصل على قيمة NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | يحصل على كائن OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | يحصل على قيمة OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | يحصل على قيمة OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | يحصل على قيمة OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | يحصل على قيمة OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | يحصل على المشروع الأب للمهمة. |
| [get_ParentTask](./get_parenttask/) | يحصل على المهمة الأب للمهمة. |
| [get_PercentComplete](./get_percentcomplete/) | يحصل على قيمة PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | يحصل على قيمة PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | يحصل على قيمة PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | يحصل على كائن TaskCollection الذي يحتوي على جميع سابقي كائن Task هذا. |
| [get_PreleveledFinish](./get_preleveledfinish/) | يحصل على قيمة PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | يحصل على قيمة PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لمهمة تم قراءتها من ملف Primavera. |
| [get_Priority](./get_priority/) | يحصل على قيمة Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | يحصل على نسخة من فئة RecurringTaskInfo للمهمة التي هي مهمة متكررة؛ إذا لم تكن المهمة متكررة فستُرجع null؛ |
| [get_RegularWork](./get_regularwork/) | يحصل على قيمة RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | يحصل على قيمة RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | يحصل على قيمة RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | يحصل على قيمة RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | يحصل على قيمة RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | يحصل على قيمة RemainingWork. |
| [get_Resume](./get_resume/) | يحصل على قيمة Resume. |
| [get_SplitParts](./get_splitparts/) | يحصل على مجموعة SplitPart التي تمثل أجزاء المهمة. |
| [get_Start](./get_start/) | يحصل على قيمة Start. |
| [get_StartSlack](./get_startslack/) | يحصل على قيمة StartSlack. |
| [get_StartText](./get_starttext/) | يحصل على قيمة StartText. |
| [get_StartVariance](./get_startvariance/) | يحصل على قيمة StartVariance. |
| [get_Status](./get_status/) | يحصل على حالة المهمة. |
| [get_StatusManager](./get_statusmanager/) | يحصل على قيمة لـ StatusManager. |
| [get_Stop](./get_stop/) | يحصل على قيمة Stop. |
| [get_SubprojectName](./get_subprojectname/) | يحصل على قيمة لـ SubprojectName. |
| [get_Successors](./get_successors/) | يحصل على كائن TaskCollection الذي يحتوي على جميع المهام اللاحقة لهذا الكائن Task. |
| [get_SV](./get_sv/) | انحراف جدول القيمة المكتسبة حتى تاريخ حالة المشروع. انحراف الجدول (SV) هو الفرق بين BCWP و BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | يحصل على كائن TimephasedDataCollection لهذه المهمة. كتلة البيانات الزمنية المرتبطة بالمهمة. |
| [get_TotalSlack](./get_totalslack/) | يحصل على قيمة لـ TotalSlack. |
| [get_Type](./get_type/) | يحصل على قيمة Type. |
| [get_Uid](./get_uid/) | يحصل على قيمة Uid. |
| [get_Warning](./get_warning/) | يحصل على قيمة تشير إلى ما إذا كان Warning مضبوطًا أم لا. |
| [get_WBS](./get_wbs/) | يحصل على قيمة لـ WBS. |
| [get_WBSLevel](./get_wbslevel/) | يحصل على قيمة لـ WBSLevel. |
| [get_Work](./get_work/) | يحصل على قيمة Work. |
| [get_WorkVariance](./get_workvariance/) | يحصل على قيمة WorkVariance. |
| [GetHashCode](./gethashcode/) | يرجع قيمة رمز تجزئة لهذا Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | يرجع كائن TimephasedDataCollection مع قيم TimephasedData ضمن تواريخ البدء والانتهاء المحددة. |
| [MoveToSibling (2 overloads)](./movetosibling/) | ينقل المهمة الحالية في نفس مستوى المخطط قبل المهمة المحددة. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحسب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، ومستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرّف المهمة، مستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، تحدد تواريخ مبكرة/متأخرة، تحسب الفجوات، والعمل، وتكاليف الحقول، وتعيد حساب المعرفات ومستويات المخطط). |
| [OutlineIndent](./outlineindent/) | يُضيف مسافة بادئة لمهمة في المخطط. |
| [OutlineOutdent](./outlineoutdent/) | يرفع مستوى مهمة في المخطط. |
| [SelectAllChildTasks](./selectallchildtasks/) | يجمع بشكل متكرر جميع المهام الفرعية لهذه المهمة. |
| [Set](./set/) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [set_ActivityId](./set_activityid/) | يمثل حقل معرف النشاط - معرف فريد للمهمة يستخدمه Primavera. (ينطبق فقط على مشاريع Primavera). |
| [set_ActualCost](./set_actualcost/) | يضبط قيمة ActualCost. |
| [set_ActualDuration](./set_actualduration/) | يضبط قيمة لـ ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | يضبط قيمة ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | يضبط قيمة ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | يضبط قيمة ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | يضبط قيمة ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | يضبط قيمة ActualStart. |
| [set_ActualWork](./set_actualwork/) | يضبط قيمة ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | يضبط قيمة ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | يضبط قيمة ACWP. |
| [set_Baselines](./set_baselines/) | يضبط مجموعة قيم الخط الأساسي للمهمة. |
| [set_BCWP](./set_bcwp/) | يضبط قيمة BCWP. |
| [set_BCWS](./set_bcws/) | يضبط قيمة BCWS. |
| [set_BudgetCost](./set_budgetcost/) | يضبط قيمة BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | يضبط قيمة BudgetWork. |
| [set_Calendar](./set_calendar/) | يضبط قيمة Calendar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | يضبط قيمة لـ CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | يضبط قيمة لـ CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | يضبط قيمة لـ CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | يضبط قيمة لـ ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | يضبط قيمة لـ ConstraintType. |
| [set_Contact](./set_contact/) | يضبط قيمة لـ Contact. |
| [set_Cost](./set_cost/) | يضبط قيمة Cost. |
| [set_CostVariance](./set_costvariance/) | يحدد قيمة CostVariance. |
| [set_Created](./set_created/) | يحدد قيمة Created. |
| [set_CV](./set_cv/) | يحدد قيمة CV. |
| [set_Deadline](./set_deadline/) | يضبط قيمة لـ Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | يضبط قيمة تشير إلى ما إذا كان DisplayAsSummary مضبوطًا أم لا. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | يضبط قيمة تشير إلى ما إذا كان DisplayOnTimeline مضبوطًا أم لا. |
| [set_Duration](./set_duration/) | يحدد قيمة Duration . |
| [set_DurationFormat](./set_durationformat/) | يضبط قيمة DurationFormat. |
| [set_DurationText](./set_durationtext/) | يحدد قيمة DurationText. |
| [set_DurationVariance](./set_durationvariance/) | يحدد قيمة DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | يحدد قيمة EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | يحدد قيمة EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | يضبط قيمة EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | يحدد قيمة ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | يحدد قيمة ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | يحصل أو يضبط المعرف الفريد للمهمة الخارجية عندما تكون المهمة خارجية. |
| [set_Finish](./set_finish/) | يحدد قيمة Finish. |
| [set_FinishSlack](./set_finishslack/) | يحدد قيمة FinishSlack. |
| [set_FinishText](./set_finishtext/) | يحدد قيمة FinishText. |
| [set_FinishVariance](./set_finishvariance/) | يضبط قيمة FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | يحدد قيمة FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | يحدد قيمة FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | يحدد قيمة FreeSlack. |
| [set_Guid](./set_guid/) | يحدد قيمة Guid. |
| [set_HideBar](./set_hidebar/) | يحدد قيمة تشير إلى ما إذا كان HideBar مضبوطًا أم لا. |
| [set_Hyperlink](./set_hyperlink/) | يحدد العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمهمة. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | يحدد العنوان لرابط تشعبي مرتبط بمهمة. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | يحدد الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمهمة. |
| [set_Id](./set_id/) | يحدد قيمة Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | يحدد قيمة تشير إلى ما إذا كان IgnoreResourceCalendar مضبوطًا أم لا. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | يحدد قيمة تشير إلى ما إذا كان IgnoreWarnings مضبوطًا أم لا. |
| [set_IsActive](./set_isactive/) | يحدد قيمة تشير إلى ما إذا كان IsActive مضبوطًا أم لا. |
| [set_IsCritical](./set_iscritical/) | يحدد قيمة تشير إلى ما إذا كان IsCritical مضبوطًا أم لا. |
| [set_IsEffortDriven](./set_iseffortdriven/) | يحدد قيمة تشير إلى ما إذا كان IsEffortDriven مضبوطًا أم لا. |
| [set_IsEstimated](./set_isestimated/) | يحدد قيمة تشير إلى ما إذا كان IsEstimated مضبوطًا أم لا. |
| [set_IsExpanded](./set_isexpanded/) | يحدد قيمة تشير إلى ما إذا كان IsExpanded مضبوطًا أم لا. |
| [set_IsExternalTask](./set_isexternaltask/) | يحدد قيمة تشير إلى ما إذا كان IsExternalTask مضبوطًا أم لا. |
| [set_IsManual](./set_ismanual/) | يحدد قيمة تشير إلى ما إذا كان IsManual مضبوطًا أم لا. |
| [set_IsMarked](./set_ismarked/) | يضبط قيمة تشير إلى ما إذا كان IsMarked مضبوطًا أم لا. |
| [set_IsMilestone](./set_ismilestone/) | يضبط قيمة تشير إلى ما إذا كان IsMilestone مضبوطًا أم لا. |
| [set_IsNull](./set_isnull/) | يحدد قيمة تشير إلى ما إذا كان IsNull مضبوطًا أم لا. |
| [set_IsOverallocated](./set_isoverallocated/) | يضبط قيمة تشير إلى ما إذا كان IsOverallocated مضبوطًا أم لا. |
| [set_IsPublished](./set_ispublished/) | يضبط قيمة تشير إلى ما إذا كان IsPublished مضبوطًا أم لا. |
| [set_IsRecurring](./set_isrecurring/) | يضبط قيمة تشير إلى ما إذا كان IsRecurring مضبوطًا أم لا. |
| [set_IsResumeValid](./set_isresumevalid/) | يضبط قيمة تشير إلى ما إذا كان IsResumeValid مضبوطًا أم لا. |
| [set_IsRollup](./set_isrollup/) | يضبط قيمة تشير إلى ما إذا كان IsRollup مضبوطًا أم لا. |
| [set_IsSubproject](./set_issubproject/) | يضبط قيمة تشير إلى ما إذا كان IsSubproject مضبوطًا أم لا. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | يضبط قيمة تشير إلى ما إذا كان IsSubprojectReadOnly مضبوطًا أم لا. |
| [set_IsSummary](./set_issummary/) | يضبط قيمة تشير إلى ما إذا كان IsSummary مضبوطًا أم لا. |
| [set_LateFinish](./set_latefinish/) | يضبط قيمة LateFinish. |
| [set_LateStart](./set_latestart/) | يضبط قيمة LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | يضبط قيمة تشير إلى ما إذا كان LevelAssignments مضبوطًا أم لا. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | يضبط قيمة تشير إلى ما إذا كان LevelingCanSplit مضبوطًا أم لا. |
| [set_LevelingDelay](./set_levelingdelay/) | يضبط قيمة LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | يضبط قيمة ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | يضبط قيمة ManualFinish. |
| [set_ManualStart](./set_manualstart/) | يضبط قيمة ManualStart. |
| [set_Name](./set_name/) | يحدد قيمة Name. |
| [set_NotesRTF](./set_notesrtf/) | يحدد قيمة NotesRTF. |
| [set_NotesText](./set_notestext/) | يحدد قيمة NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | يضبط كائن OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | يضبط قيمة OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | يضبط قيمة OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | يضبط قيمة OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | يضبط قيمة OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | يضبط قيمة PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | يضبط قيمة PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | يضبط قيمة PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | يضبط قيمة PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | يضبط قيمة PreleveledStart. |
| [set_Priority](./set_priority/) | يضبط قيمة Priority. |
| [set_RegularWork](./set_regularwork/) | يضبط قيمة RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | يضبط قيمة RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | يضبط قيمة RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | يضبط قيمة RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | يضبط قيمة RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | يضبط قيمة RemainingWork. |
| [set_Resume](./set_resume/) | يضبط قيمة Resume. |
| [set_Start](./set_start/) | يضبط قيمة Start. |
| [set_StartSlack](./set_startslack/) | يضبط قيمة StartSlack. |
| [set_StartText](./set_starttext/) | يضبط قيمة StartText. |
| [set_StartVariance](./set_startvariance/) | يضبط قيمة StartVariance. |
| [set_StatusManager](./set_statusmanager/) | يضبط قيمة StatusManager. |
| [set_Stop](./set_stop/) | يضبط قيمة Stop. |
| [set_SubprojectName](./set_subprojectname/) | يضبط قيمة SubprojectName. |
| [set_SV](./set_sv/) | انحراف جدول القيمة المكتسبة حتى تاريخ حالة المشروع. انحراف الجدول (SV) هو الفرق بين BCWP و BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | يضبط كائن TimephasedDataCollection لهذه المهمة. كتلة البيانات الزمنية المرتبطة بالمهمة. |
| [set_TotalSlack](./set_totalslack/) | يضبط قيمة TotalSlack. |
| [set_Type](./set_type/) | يضبط قيمة Type. |
| [set_Uid](./set_uid/) | يضبط قيمة Uid. |
| [set_Warning](./set_warning/) | يضبط قيمة تشير إلى ما إذا كان Warning مضبوطًا أم لا. |
| [set_WBS](./set_wbs/) | يضبط قيمة WBS. |
| [set_WBSLevel](./set_wbslevel/) | يضبط قيمة WBSLevel. |
| [set_Work](./set_work/) | يضبط قيمة Work. |
| [set_WorkVariance](./set_workvariance/) | يضبط قيمة WorkVariance. |
| [ToString](./tostring/) | يعيد تمثيلًا نصيًا قصيرًا للمهمة. التفاصيل الدقيقة للتمثيل غير محددة وقابلة للتغيير. |

