---
title: "Aspose::Tasks::Task sınıfı"
linktitle: "Task"
articleTitle: "Task"
second_title: "C++ için Aspose.Tasks"
description: "Bir projedeki görevi temsil eder."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Bir projedeki görevi temsil eder.

Task, tek bir atomik iş parçasını temsil eder.

Bir proje planlamak için görevler oluşturup uygun kaynakları atayarak Task kullanılabilir. Projedeki görevler, kök bir görev ve alt görev ağaçlarıyla köklü bir hiyerarşik ağaç yapısı olarak düzenlenir.

Görev ağacı oluşturmak için Project::RootTask özelliğine erişilerek Aspose::Tasks::TaskCollection adlı özel bir koleksiyon kullanılabilir, örn:

```cpp
Project project = new Project();
 
// yeni görevler ekle
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
 
// projeyi mevcut formatlardan birinde kaydet
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clone](./clone/) | Alt görevler olmadan bir görevin tam bir kopyasını oluşturur. |
| [Delete](./delete/) | Bir görevi üst proje görev koleksiyonundan ve tüm atamalarından siler. |
| [Equals (2 overloads)](./equals/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [Get](./get/) | Bu konteynerde özelliğin eşlendiği değeri döndürür. |
| [get_ActivityId](./get_activityid/) | Aktivite kimliği alanını temsil eder - Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı. (yalnızca Primavera projeleri için geçerlidir). |
| [get_ActualCost](./get_actualcost/) | ActualCost değerini alır. |
| [get_ActualDuration](./get_actualduration/) | ActualDuration değerini alır. |
| [get_ActualFinish](./get_actualfinish/) | ActualFinish değerini alır. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | ActualOvertimeCost değerini alır. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | ActualOvertimeWork değerini alır. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | ActualOvertimeWorkProtected değerini alır. |
| [get_ActualStart](./get_actualstart/) | ActualStart değerini alır. |
| [get_ActualWork](./get_actualwork/) | ActualWork değerini alır. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | ActualWorkProtected değerini alır. |
| [get_ACWP](./get_acwp/) | ACWP değerini alır. |
| [get_Assignments](./get_assignments/) | Bu nesne için kaynak atamalarının bir koleksiyonunu alır. |
| [get_Baselines](./get_baselines/) | Görevin temel değer koleksiyonunu alır. |
| [get_BCWP](./get_bcwp/) | BCWP değerini alır. |
| [get_BCWS](./get_bcws/) | BCWS değerini alır. |
| [get_BudgetCost](./get_budgetcost/) | BudgetCost değerini alır. |
| [get_BudgetWork](./get_budgetwork/) | BudgetWork değerini alır. |
| [get_Calendar](./get_calendar/) | Calendar değerini alır. |
| [get_Children](./get_children/) | Bu nesnenin alt görev koleksiyonunu alır. Çocuk görevleri temsil eden TaskCollection nesnesi. |
| [get_CommitmentFinish](./get_commitmentfinish/) | CommitmentFinish değerini alır. |
| [get_CommitmentStart](./get_commitmentstart/) | CommitmentStart değerini alır. |
| [get_CommitmentType](./get_commitmenttype/) | CommitmentType değerini alır. |
| [get_ConstraintDate](./get_constraintdate/) | ConstraintDate değerini alır. |
| [get_ConstraintType](./get_constrainttype/) | ConstraintType değerini alır. |
| [get_Contact](./get_contact/) | Contact değerini alır. |
| [get_Cost](./get_cost/) | Cost değerini alır. |
| [get_CostVariance](./get_costvariance/) | CostVariance değerini alır. |
| [get_Created](./get_created/) | Created değerini alır. |
| [get_CV](./get_cv/) | CV değerini alır. |
| [get_Deadline](./get_deadline/) | Deadline değerini alır. |
| [get_DisplayAsSummary](./get_displayassummary/) | DisplayAsSummary ayarlı olup olmadığını gösteren değeri alır. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | DisplayOnTimeline ayarlı olup olmadığını gösteren değeri alır. |
| [get_Duration](./get_duration/) | Duration değerini alır. |
| [get_DurationFormat](./get_durationformat/) | DurationFormat değerini alır. |
| [get_DurationText](./get_durationtext/) | DurationText değerini alır. |
| [get_DurationVariance](./get_durationvariance/) | DurationVariance değerini alır. |
| [get_EarlyFinish](./get_earlyfinish/) | EarlyFinish değerini alır. |
| [get_EarlyStart](./get_earlystart/) | EarlyStart değerini alır. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod değerini alır. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Genişletilmiş bir niteliğin değerlerini içeren ExtendedAttributeCollection nesnesini alır. |
| [get_ExternalId](./get_externalid/) | ExternalId değerini alır. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | ExternalTaskProject değerini alır. |
| [get_ExternalUid](./get_externaluid/) | Görev dışsal olduğunda dış görev'in benzersiz tanımlayıcısını alır veya ayarlar. |
| [get_Finish](./get_finish/) | Finish değerini alır. |
| [get_FinishSlack](./get_finishslack/) | FinishSlack değerini alır. |
| [get_FinishText](./get_finishtext/) | FinishText değerini alır. |
| [get_FinishVariance](./get_finishvariance/) | FinishVariance değerini alır. |
| [get_FixedCost](./get_fixedcost/) | FixedCost değerini alır. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | FixedCostAccrual değerini alır. |
| [get_FreeSlack](./get_freeslack/) | FreeSlack değerini alır. |
| [get_Guid](./get_guid/) | Guid değerini alır. |
| [get_HideBar](./get_hidebar/) | HideBar'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_Hyperlink](./get_hyperlink/) | Görevle ilişkili bir hiperlink için başlığı veya açıklama metnini alır. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Görevle ilişkili bir hiperlinkin adresini alır. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Görevle ilişkili bir hiperlinkteki belgenin belirli konumunu alır. |
| [get_Id](./get_id/) | Id değerini alır. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | IgnoreResourceCalendar'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | IgnoreWarnings'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsActive](./get_isactive/) | IsActive'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsCritical](./get_iscritical/) | IsCritical'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsEffortDriven](./get_iseffortdriven/) | IsEffortDriven'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsEstimated](./get_isestimated/) | IsEstimated'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsExpanded](./get_isexpanded/) | IsExpanded'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsExternalTask](./get_isexternaltask/) | IsExternalTask'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsManual](./get_ismanual/) | IsManual'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsMarked](./get_ismarked/) | IsMarked'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsMilestone](./get_ismilestone/) | IsMilestone'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsNull](./get_isnull/) | IsNull'ın ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [get_IsOverallocated](./get_isoverallocated/) | IsOverallocated'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsPublished](./get_ispublished/) | IsPublished'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsRecurring](./get_isrecurring/) | IsRecurring'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsResumeValid](./get_isresumevalid/) | IsResumeValid'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsRollup](./get_isrollup/) | IsRollup'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsSubproject](./get_issubproject/) | IsSubproject'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | IsSubprojectReadOnly'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_IsSummary](./get_issummary/) | IsSummary'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_LateFinish](./get_latefinish/) | LateFinish değerini alır. |
| [get_LateStart](./get_latestart/) | LateStart değerini alır. |
| [get_LevelAssignments](./get_levelassignments/) | LevelAssignments ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | LevelingCanSplit ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_LevelingDelay](./get_levelingdelay/) | LevelingDelay değerini alır. |
| [get_ManualDuration](./get_manualduration/) | ManualDuration değerini alır. |
| [get_ManualFinish](./get_manualfinish/) | ManualFinish değerini alır. |
| [get_ManualStart](./get_manualstart/) | ManualStart değerini alır. |
| [get_Name](./get_name/) | Name değerini alır. |
| [get_NotesRTF](./get_notesrtf/) | NotesRTF değerini alır. |
| [get_NotesText](./get_notestext/) | NotesText değerini alır. |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeCollection nesnesini alır. |
| [get_OutlineLevel](./get_outlinelevel/) | OutlineLevel değerini alır. |
| [get_OutlineNumber](./get_outlinenumber/) | OutlineNumber değerini alır. |
| [get_OvertimeCost](./get_overtimecost/) | OvertimeCost değerini alır. |
| [get_OvertimeWork](./get_overtimework/) | OvertimeWork değerini alır. |
| [get_ParentProject](./get_parentproject/) | Bir görevin üst proje nesnesini alır. |
| [get_ParentTask](./get_parenttask/) | Bir görevin üst görevini alır. |
| [get_PercentComplete](./get_percentcomplete/) | PercentComplete değerini alır. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | PercentWorkComplete değerini alır. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | PhysicalPercentComplete değerini alır. |
| [get_Predecessors](./get_predecessors/) | Bu Task nesnesinin tüm öncüllerini içeren bir TaskCollection nesnesini alır. |
| [get_PreleveledFinish](./get_preleveledfinish/) | PreleveledFinish değerini alır. |
| [get_PreleveledStart](./get_preleveledstart/) | PreleveledStart değerini alır. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera dosyasından okunan bir görev için Primavera'ye özgü özellikleri içeren bir nesneyi alır. |
| [get_Priority](./get_priority/) | Priority değerini alır. |
| [get_RecurringInfo](./get_recurringinfo/) | Yinelenen bir görev olan görev için RecurringTaskInfo sınıfının örneğini alır; görev yinelenen bir görev değilse null döndürür; |
| [get_RegularWork](./get_regularwork/) | RegularWork değerini alır. |
| [get_RemainingCost](./get_remainingcost/) | RemainingCost değerini alır. |
| [get_RemainingDuration](./get_remainingduration/) | RemainingDuration değerini alır. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | RemainingOvertimeCost değerini alır. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | RemainingOvertimeWork değerini alır. |
| [get_RemainingWork](./get_remainingwork/) | RemainingWork değerini alır. |
| [get_Resume](./get_resume/) | Resume değerini alır. |
| [get_SplitParts](./get_splitparts/) | Bir görevin bölümlerini temsil eden bir SplitPart koleksiyonunu alır. |
| [get_Start](./get_start/) | Start değerini alır. |
| [get_StartSlack](./get_startslack/) | StartSlack değerini alır. |
| [get_StartText](./get_starttext/) | StartText değerini alır. |
| [get_StartVariance](./get_startvariance/) | StartVariance değerini alır. |
| [get_Status](./get_status/) | Görev durumunu alır. |
| [get_StatusManager](./get_statusmanager/) | StatusManager değerini alır. |
| [get_Stop](./get_stop/) | Stop değerini alır. |
| [get_SubprojectName](./get_subprojectname/) | SubprojectName değerini alır. |
| [get_Successors](./get_successors/) | Bu Task nesnesinin tüm ardıllarını içeren bir TaskCollection nesnesi alır. |
| [get_SV](./get_sv/) | Proje durum tarihine kadar kazanılan değer zaman sapması. Zaman sapması (SV), BCWP ile BCWS arasındaki farktır. |
| [get_TimephasedData](./get_timephaseddata/) | Bu görevin bir TimephasedDataCollection nesnesini alır. Görevle ilişkili zaman aşamalı veri bloğu. |
| [get_TotalSlack](./get_totalslack/) | TotalSlack değerini alır. |
| [get_Type](./get_type/) | Type değerini alır. |
| [get_Uid](./get_uid/) | Uid değerini alır. |
| [get_Warning](./get_warning/) | Uyarının ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_WBS](./get_wbs/) | WBS değerini alır. |
| [get_WBSLevel](./get_wbslevel/) | WBSLevel değerini alır. |
| [get_Work](./get_work/) | Work değerini alır. |
| [get_WorkVariance](./get_workvariance/) | WorkVariance değerini alır. |
| [GetHashCode](./gethashcode/) | Bu Task için bir hash kod değeri döndürür. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Belirtilen başlangıç ve bitiş tarihleri arasındaki TimephasedData değerlerine sahip bir TimephasedDataCollection nesnesi döndürür. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Mevcut görevi aynı Outline Level'da belirtilen görevin önüne taşır. ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihlerini, erken/son tarihleri ayarlar) yeniden zamanlar ve gecikmeler, iş ve maliyet alanları, outline seviyeleri gibi bağımlı alanları hesaplar). ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini, outline seviyesini ve outline numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlar (başlangıç/bitiş tarihlerini, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve outline seviyelerini yeniden hesaplar). |
| [OutlineIndent](./outlineindent/) | Görevi outline içinde girintiler. |
| [OutlineOutdent](./outlineoutdent/) | Görevi outline içinde yükseltir. |
| [SelectAllChildTasks](./selectallchildtasks/) | Bu görevin tüm alt görevlerini özyinelemeli olarak toplar. |
| [Set](./set/) | Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler. |
| [set_ActivityId](./set_activityid/) | Aktivite kimliği alanını temsil eder - Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı. (yalnızca Primavera projeleri için geçerlidir). |
| [set_ActualCost](./set_actualcost/) | ActualCost değerini ayarlar. |
| [set_ActualDuration](./set_actualduration/) | ActualDuration değerini ayarlar. |
| [set_ActualFinish](./set_actualfinish/) | ActualFinish değerini ayarlar. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | ActualOvertimeCost değerini ayarlar. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | ActualOvertimeWork değerini ayarlar. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | ActualOvertimeWorkProtected değerini ayarlar. |
| [set_ActualStart](./set_actualstart/) | ActualStart değerini ayarlar. |
| [set_ActualWork](./set_actualwork/) | ActualWork değerini ayarlar. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | ActualWorkProtected değerini ayarlar. |
| [set_ACWP](./set_acwp/) | ACWP değerini ayarlar. |
| [set_Baselines](./set_baselines/) | Görevin temel değerler koleksiyonunu ayarlar. |
| [set_BCWP](./set_bcwp/) | BCWP değerini ayarlar. |
| [set_BCWS](./set_bcws/) | BCWS değerini ayarlar. |
| [set_BudgetCost](./set_budgetcost/) | BudgetCost değerini ayarlar. |
| [set_BudgetWork](./set_budgetwork/) | BudgetWork değerini ayarlar. |
| [set_Calendar](./set_calendar/) | Calendar değerini ayarlar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | CommitmentFinish değerini ayarlar. |
| [set_CommitmentStart](./set_commitmentstart/) | CommitmentStart değerini ayarlar. |
| [set_CommitmentType](./set_commitmenttype/) | CommitmentType değerini ayarlar. |
| [set_ConstraintDate](./set_constraintdate/) | ConstraintDate değerini ayarlar. |
| [set_ConstraintType](./set_constrainttype/) | ConstraintType değerini ayarlar. |
| [set_Contact](./set_contact/) | Contact değerini ayarlar. |
| [set_Cost](./set_cost/) | Cost değerini ayarlar. |
| [set_CostVariance](./set_costvariance/) | CostVariance değerini ayarlar. |
| [set_Created](./set_created/) | Created değerini ayarlar. |
| [set_CV](./set_cv/) | CV değerini ayarlar. |
| [set_Deadline](./set_deadline/) | Deadline değerini ayarlar. |
| [set_DisplayAsSummary](./set_displayassummary/) | DisplayAsSummary'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | DisplayOnTimeline'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_Duration](./set_duration/) | Duration değerini ayarlar. |
| [set_DurationFormat](./set_durationformat/) | DurationFormat değerini ayarlar. |
| [set_DurationText](./set_durationtext/) | DurationText değerini ayarlar. |
| [set_DurationVariance](./set_durationvariance/) | DurationVariance değerini ayarlar. |
| [set_EarlyFinish](./set_earlyfinish/) | EarlyFinish değerini ayarlar. |
| [set_EarlyStart](./set_earlystart/) | EarlyStart değerini ayarlar. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod değerini ayarlar. |
| [set_ExternalId](./set_externalid/) | ExternalId değerini ayarlar. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | ExternalTaskProject değerini ayarlar. |
| [set_ExternalUid](./set_externaluid/) | Görev dışsal olduğunda dış görev'in benzersiz tanımlayıcısını alır veya ayarlar. |
| [set_Finish](./set_finish/) | Finish değerini ayarlar. |
| [set_FinishSlack](./set_finishslack/) | FinishSlack değerini ayarlar. |
| [set_FinishText](./set_finishtext/) | FinishText değerini ayarlar. |
| [set_FinishVariance](./set_finishvariance/) | FinishVariance değerini ayarlar. |
| [set_FixedCost](./set_fixedcost/) | FixedCost değerini ayarlar. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | FixedCostAccrual değerini ayarlar. |
| [set_FreeSlack](./set_freeslack/) | FreeSlack değerini ayarlar. |
| [set_Guid](./set_guid/) | Guid değerini ayarlar. |
| [set_HideBar](./set_hidebar/) | HideBar'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_Hyperlink](./set_hyperlink/) | Görev ile ilişkili bir köprü için başlık veya açıklama metnini ayarlar. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Görev ile ilişkili bir köprünün adresini ayarlar. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Görev ile ilişkili bir köprüdeki bir belgedeki belirli konumu ayarlar. |
| [set_Id](./set_id/) | Id değerini ayarlar. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | IgnoreResourceCalendar'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | IgnoreWarnings'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsActive](./set_isactive/) | IsActive'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsCritical](./set_iscritical/) | IsCritical'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsEffortDriven](./set_iseffortdriven/) | IsEffortDriven'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsEstimated](./set_isestimated/) | IsEstimated'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsExpanded](./set_isexpanded/) | IsExpanded'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsExternalTask](./set_isexternaltask/) | IsExternalTask'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsManual](./set_ismanual/) | IsManual'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsMarked](./set_ismarked/) | IsMarked'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsMilestone](./set_ismilestone/) | IsMilestone'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsNull](./set_isnull/) | IsNull ayarlı olup olmadığını gösteren bir değeri ayarlar. |
| [set_IsOverallocated](./set_isoverallocated/) | IsOverallocated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsPublished](./set_ispublished/) | IsPublished'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsRecurring](./set_isrecurring/) | IsRecurring'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsResumeValid](./set_isresumevalid/) | IsResumeValid'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsRollup](./set_isrollup/) | IsRollup'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsSubproject](./set_issubproject/) | IsSubproject'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | IsSubprojectReadOnly'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_IsSummary](./set_issummary/) | IsSummary'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_LateFinish](./set_latefinish/) | LateFinish değerini ayarlar. |
| [set_LateStart](./set_latestart/) | LateStart değerini ayarlar. |
| [set_LevelAssignments](./set_levelassignments/) | LevelAssignments'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | LevelingCanSplit'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_LevelingDelay](./set_levelingdelay/) | LevelingDelay değerini ayarlar. |
| [set_ManualDuration](./set_manualduration/) | ManualDuration değerini ayarlar. |
| [set_ManualFinish](./set_manualfinish/) | ManualFinish değerini ayarlar. |
| [set_ManualStart](./set_manualstart/) | ManualStart değerini ayarlar. |
| [set_Name](./set_name/) | Name değerini ayarlar. |
| [set_NotesRTF](./set_notesrtf/) | NotesRTF değerini ayarlar. |
| [set_NotesText](./set_notestext/) | NotesText değerini ayarlar. |
| [set_OutlineCodes](./set_outlinecodes/) | OutlineCodeCollection nesnesini ayarlar. |
| [set_OutlineLevel](./set_outlinelevel/) | OutlineLevel değerini ayarlar. |
| [set_OutlineNumber](./set_outlinenumber/) | OutlineNumber değerini ayarlar. |
| [set_OvertimeCost](./set_overtimecost/) | OvertimeCost değerini ayarlar. |
| [set_OvertimeWork](./set_overtimework/) | OvertimeWork değerini ayarlar. |
| [set_PercentComplete](./set_percentcomplete/) | PercentComplete değerini ayarlar. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | PercentWorkComplete değerini ayarlar. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | PhysicalPercentComplete değerini ayarlar. |
| [set_PreleveledFinish](./set_preleveledfinish/) | PreleveledFinish değerini ayarlar. |
| [set_PreleveledStart](./set_preleveledstart/) | PreleveledStart değerini ayarlar. |
| [set_Priority](./set_priority/) | Priority değerini ayarlar. |
| [set_RegularWork](./set_regularwork/) | RegularWork değerini ayarlar. |
| [set_RemainingCost](./set_remainingcost/) | RemainingCost değerini ayarlar. |
| [set_RemainingDuration](./set_remainingduration/) | RemainingDuration değerini ayarlar. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | RemainingOvertimeCost değerini ayarlar. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | RemainingOvertimeWork değerini ayarlar. |
| [set_RemainingWork](./set_remainingwork/) | RemainingWork değerini ayarlar. |
| [set_Resume](./set_resume/) | Resume değerini ayarlar. |
| [set_Start](./set_start/) | Start değerini ayarlar. |
| [set_StartSlack](./set_startslack/) | StartSlack değerini ayarlar. |
| [set_StartText](./set_starttext/) | StartText değerini ayarlar. |
| [set_StartVariance](./set_startvariance/) | StartVariance değerini ayarlar. |
| [set_StatusManager](./set_statusmanager/) | StatusManager değerini ayarlar. |
| [set_Stop](./set_stop/) | Stop değerini ayarlar. |
| [set_SubprojectName](./set_subprojectname/) | SubprojectName değerini ayarlar. |
| [set_SV](./set_sv/) | Proje durum tarihine kadar kazanılan değer zaman sapması. Zaman sapması (SV), BCWP ile BCWS arasındaki farktır. |
| [set_TimephasedData](./set_timephaseddata/) | Bu görevin bir TimephasedDataCollection nesnesini ayarlar. Görevle ilişkili zaman aşamalı veri bloğu. |
| [set_TotalSlack](./set_totalslack/) | TotalSlack değerini ayarlar. |
| [set_Type](./set_type/) | Type değerini ayarlar. |
| [set_Uid](./set_uid/) | Uid değerini ayarlar. |
| [set_Warning](./set_warning/) | Uyarının ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [set_WBS](./set_wbs/) | WBS değerini ayarlar. |
| [set_WBSLevel](./set_wbslevel/) | WBSLevel değerini ayarlar. |
| [set_Work](./set_work/) | Work değerini ayarlar. |
| [set_WorkVariance](./set_workvariance/) | WorkVariance değerini ayarlar. |
| [ToString](./tostring/) | Bir görevin kısa dize temsilini döndürür. Temsilin kesin detayları belirtilmemiştir ve değişebilir. |

