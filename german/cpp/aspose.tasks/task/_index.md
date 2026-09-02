---
title: "Aspose::Tasks::Task Klasse"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks für C++"
description: "Stellt eine Aufgabe in einem Projekt dar."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Stellt eine Aufgabe in einem Projekt dar.

Der Task stellt ein einzelnes atomares Arbeitspaket dar.

Man kann Task verwenden, um ein Projekt zu planen, indem man Tasks erstellt und geeignete Ressourcen zuweist. Tasks in einem Projekt sind als baumartige hierarchische Struktur mit einer Root-Task und Unterbäumen von Kind-Tasks organisiert.

Um einen Aufgabenbaum zu erstellen, kann man eine spezialisierte Sammlung Aspose::Tasks::TaskCollection verwenden, indem man die Eigenschaft Project::RootTask zugreift, z. B.:

```cpp
Project project = new Project();
 
// neue Aufgaben hinzufügen
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
 
// Projekt in einem der verfügbaren Formate speichern
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clone](./clone/) | Erstellt eine vollständige Kopie einer Aufgabe ohne Unteraufgaben. |
| [Delete](./delete/) | Löscht eine Aufgabe aus der Aufgabensammlung des übergeordneten Projekts und alle zugehörigen Zuweisungen. |
| [Equals (2 overloads)](./equals/) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [Get](./get/) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [get_ActivityId](./get_activityid/) | Stellt das Aktivitäts‑ID‑Feld dar – die eindeutige Kennung einer Aufgabe, die von Primavera verwendet wird. (nur für Primavera‑Projekte anwendbar). |
| [get_ActualCost](./get_actualcost/) | Ermittelt einen Wert von ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Liefert einen Wert von ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Liest einen Wert von ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Gibt einen Wert von ActualOvertimeCost zurück. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Gibt einen Wert von ActualOvertimeWork zurück. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Gibt einen Wert von ActualOvertimeWorkProtected zurück. |
| [get_ActualStart](./get_actualstart/) | Liest einen Wert von ActualStart. |
| [get_ActualWork](./get_actualwork/) | Gibt einen Wert von ActualWork zurück. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Gibt einen Wert von ActualWorkProtected zurück. |
| [get_ACWP](./get_acwp/) | Gibt einen Wert von ACWP zurück. |
| [get_Assignments](./get_assignments/) | Gibt eine Sammlung von Ressourcenzuweisungen für dieses Objekt zurück. |
| [get_Baselines](./get_baselines/) | Liefert die Sammlung der Basislinienwerte der Aufgabe. |
| [get_BCWP](./get_bcwp/) | Gibt einen Wert von BCWP zurück. |
| [get_BCWS](./get_bcws/) | Gibt einen Wert von BCWS zurück. |
| [get_BudgetCost](./get_budgetcost/) | Gibt einen Wert von BudgetCost zurück. |
| [get_BudgetWork](./get_budgetwork/) | Gibt einen Wert von BudgetWork zurück. |
| [get_Calendar](./get_calendar/) | Gibt einen Wert von Calendar zurück. |
| [get_Children](./get_children/) | Liefert eine Kindaufgabensammlung dieses Objekts. TaskCollection-Objekt, das Kindaufgaben darstellt. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Liefert einen Wert von CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Liefert einen Wert von CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Liefert einen Wert von CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Liefert einen Wert von ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Liefert einen Wert von ConstraintType. |
| [get_Contact](./get_contact/) | Liefert einen Wert von Contact. |
| [get_Cost](./get_cost/) | Gibt einen Wert von Cost zurück. |
| [get_CostVariance](./get_costvariance/) | Gibt einen Wert von CostVariance zurück. |
| [get_Created](./get_created/) | Ruft den Wert von Created ab. |
| [get_CV](./get_cv/) | Ruft den Wert von CV ab. |
| [get_Deadline](./get_deadline/) | Liefert einen Wert von Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Liefert einen Wert, der angibt, ob DisplayAsSummary gesetzt ist oder nicht. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Liefert einen Wert, der angibt, ob DisplayOnTimeline gesetzt ist oder nicht. |
| [get_Duration](./get_duration/) | Liefert einen Wert von Duration. |
| [get_DurationFormat](./get_durationformat/) | Liefert einen Wert von DurationFormat. |
| [get_DurationText](./get_durationtext/) | Liefert einen Wert von DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Liefert einen Wert von DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Liefert einen Wert von EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Liefert einen Wert von EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Liefert einen Wert von EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Liefert das ExtendedAttributeCollection-Objekt, das die Werte eines erweiterten Attributs enthält. |
| [get_ExternalId](./get_externalid/) | Liefert einen Wert von ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Liefert einen Wert von ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Liest oder setzt die eindeutige Kennung der externen Aufgabe, wenn die Aufgabe extern ist. |
| [get_Finish](./get_finish/) | Ruft den Wert von Finish ab. |
| [get_FinishSlack](./get_finishslack/) | Liest den Wert von FinishSlack. |
| [get_FinishText](./get_finishtext/) | Liest den Wert von FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Liest einen Wert von FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Liest den Wert von FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Liest den Wert von FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Liest den Wert von FreeSlack. |
| [get_Guid](./get_guid/) | Ruft den Wert von Guid ab. |
| [get_HideBar](./get_hidebar/) | Liest einen Wert, der angibt, ob HideBar gesetzt ist oder nicht. |
| [get_Hyperlink](./get_hyperlink/) | Liest den Titel oder erläuternden Text für einen mit einer Aufgabe verknüpften Hyperlink. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Liest die Adresse für einen mit einer Aufgabe verknüpften Hyperlink. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Liest den spezifischen Ort in einem Dokument in einem mit einer Aufgabe verknüpften Hyperlink. |
| [get_Id](./get_id/) | Ruft den Wert von Id ab. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Liest einen Wert, der angibt, ob IgnoreResourceCalendar gesetzt ist oder nicht. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Liest einen Wert, der angibt, ob IgnoreWarnings gesetzt ist oder nicht. |
| [get_IsActive](./get_isactive/) | Liest einen Wert, der angibt, ob IsActive gesetzt ist oder nicht. |
| [get_IsCritical](./get_iscritical/) | Liest einen Wert, der angibt, ob IsCritical gesetzt ist oder nicht. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Liest einen Wert, der angibt, ob IsEffortDriven gesetzt ist oder nicht. |
| [get_IsEstimated](./get_isestimated/) | Liest einen Wert, der angibt, ob IsEstimated gesetzt ist oder nicht. |
| [get_IsExpanded](./get_isexpanded/) | Liest einen Wert, der angibt, ob IsExpanded gesetzt ist oder nicht. |
| [get_IsExternalTask](./get_isexternaltask/) | Liest einen Wert, der angibt, ob IsExternalTask gesetzt ist oder nicht. |
| [get_IsManual](./get_ismanual/) | Liest einen Wert, der angibt, ob IsManual gesetzt ist oder nicht. |
| [get_IsMarked](./get_ismarked/) | Liest einen Wert, der angibt, ob IsMarked gesetzt ist oder nicht. |
| [get_IsMilestone](./get_ismilestone/) | Liest einen Wert, der angibt, ob IsMilestone gesetzt ist oder nicht. |
| [get_IsNull](./get_isnull/) | Ruft einen Wert ab, der angibt, ob IsNull gesetzt ist oder nicht. |
| [get_IsOverallocated](./get_isoverallocated/) | Liest einen Wert, der angibt, ob IsOverallocated gesetzt ist oder nicht. |
| [get_IsPublished](./get_ispublished/) | Liest einen Wert, der angibt, ob IsPublished gesetzt ist oder nicht. |
| [get_IsRecurring](./get_isrecurring/) | Liest einen Wert, der angibt, ob IsRecurring gesetzt ist oder nicht. |
| [get_IsResumeValid](./get_isresumevalid/) | Liest einen Wert, der angibt, ob IsResumeValid gesetzt ist oder nicht. |
| [get_IsRollup](./get_isrollup/) | Gibt einen Wert zurück, der angibt, ob IsRollup gesetzt ist oder nicht. |
| [get_IsSubproject](./get_issubproject/) | Gibt einen Wert zurück, der angibt, ob IsSubproject gesetzt ist oder nicht. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Gibt einen Wert zurück, der angibt, ob IsSubprojectReadOnly gesetzt ist oder nicht. |
| [get_IsSummary](./get_issummary/) | Gibt einen Wert zurück, der angibt, ob IsSummary gesetzt ist oder nicht. |
| [get_LateFinish](./get_latefinish/) | Gibt einen Wert von LateFinish zurück. |
| [get_LateStart](./get_latestart/) | Gibt einen Wert von LateStart zurück. |
| [get_LevelAssignments](./get_levelassignments/) | Gibt einen Wert zurück, der angibt, ob LevelAssignments gesetzt ist oder nicht. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Gibt einen Wert zurück, der angibt, ob LevelingCanSplit gesetzt ist oder nicht. |
| [get_LevelingDelay](./get_levelingdelay/) | Ruft den Wert von LevelingDelay ab. |
| [get_ManualDuration](./get_manualduration/) | Gibt einen Wert von ManualDuration zurück. |
| [get_ManualFinish](./get_manualfinish/) | Gibt einen Wert von ManualFinish zurück. |
| [get_ManualStart](./get_manualstart/) | Gibt einen Wert von ManualStart zurück. |
| [get_Name](./get_name/) | Ruft den Wert von Name ab. |
| [get_NotesRTF](./get_notesrtf/) | Ruft den Wert von NotesRTF ab. |
| [get_NotesText](./get_notestext/) | Ruft den Wert von NotesText ab. |
| [get_OutlineCodes](./get_outlinecodes/) | Gibt das OutlineCodeCollection-Objekt zurück. |
| [get_OutlineLevel](./get_outlinelevel/) | Gibt einen Wert von OutlineLevel zurück. |
| [get_OutlineNumber](./get_outlinenumber/) | Gibt einen Wert von OutlineNumber zurück. |
| [get_OvertimeCost](./get_overtimecost/) | Ruft einen Wert von OvertimeCost ab. |
| [get_OvertimeWork](./get_overtimework/) | Ruft einen Wert von OvertimeWork ab. |
| [get_ParentProject](./get_parentproject/) | Gibt das übergeordnete Projekt einer Aufgabe zurück. |
| [get_ParentTask](./get_parenttask/) | Gibt die übergeordnete Aufgabe einer Aufgabe zurück. |
| [get_PercentComplete](./get_percentcomplete/) | Gibt einen Wert von PercentComplete zurück. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Ruft einen Wert von PercentWorkComplete ab. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Gibt einen Wert von PhysicalPercentComplete zurück. |
| [get_Predecessors](./get_predecessors/) | Gibt ein TaskCollection-Objekt zurück, das alle Vorgänger dieses Task-Objekts enthält. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Gibt einen Wert von PreleveledFinish zurück. |
| [get_PreleveledStart](./get_preleveledstart/) | Gibt einen Wert von PreleveledStart zurück. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Gibt ein Objekt zurück, das Primavera-spezifische Eigenschaften für eine Aufgabe enthält, die aus einer Primavera-Datei gelesen wurde. |
| [get_Priority](./get_priority/) | Gibt einen Wert von Priority zurück. |
| [get_RecurringInfo](./get_recurringinfo/) | Gibt die Instanz der RecurringTaskInfo-Klasse für die Aufgabe zurück, die eine wiederkehrende Aufgabe ist; wenn die Aufgabe keine wiederkehrende ist, wird null zurückgegeben; |
| [get_RegularWork](./get_regularwork/) | Ruft einen Wert von RegularWork ab. |
| [get_RemainingCost](./get_remainingcost/) | Ruft einen Wert von RemainingCost ab. |
| [get_RemainingDuration](./get_remainingduration/) | Gibt einen Wert von RemainingDuration zurück. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Ruft einen Wert von RemainingOvertimeCost ab. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Ruft einen Wert von RemainingOvertimeWork ab. |
| [get_RemainingWork](./get_remainingwork/) | Ruft einen Wert von RemainingWork ab. |
| [get_Resume](./get_resume/) | Ruft den Wert von Resume ab. |
| [get_SplitParts](./get_splitparts/) | Ruft eine SplitPart‑Sammlung ab, die die Teile einer Aufgabe darstellt. |
| [get_Start](./get_start/) | Ruft einen Wert von Start ab. |
| [get_StartSlack](./get_startslack/) | Ruft einen Wert von StartSlack ab. |
| [get_StartText](./get_starttext/) | Ruft einen Wert von StartText ab. |
| [get_StartVariance](./get_startvariance/) | Ruft den Wert von StartVariance ab. |
| [get_Status](./get_status/) | Ruft den Aufgabenstatus ab. |
| [get_StatusManager](./get_statusmanager/) | Ruft einen Wert von StatusManager ab. |
| [get_Stop](./get_stop/) | Ruft den Wert von Stop ab. |
| [get_SubprojectName](./get_subprojectname/) | Ruft einen Wert von SubprojectName ab. |
| [get_Successors](./get_successors/) | Ruft ein TaskCollection‑Objekt ab, das alle Nachfolger dieses Task‑Objekts enthält. |
| [get_SV](./get_sv/) | Die Earned-Value-Planabweichung bis zum Projektstatusdatum. Die Planabweichung (SV) ist die Differenz zwischen BCWP und BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Ruft ein TimephasedDataCollection‑Objekt dieser Aufgabe ab. Der zeitlich aufgeteilte Datenblock, der einer Aufgabe zugeordnet ist. |
| [get_TotalSlack](./get_totalslack/) | Ruft einen Wert von TotalSlack ab. |
| [get_Type](./get_type/) | Ruft einen Wert von Type ab. |
| [get_Uid](./get_uid/) | Ruft einen Wert von Uid ab. |
| [get_Warning](./get_warning/) | Ruft einen Wert ab, der angibt, ob Warning gesetzt ist oder nicht. |
| [get_WBS](./get_wbs/) | Ruft einen Wert von WBS ab. |
| [get_WBSLevel](./get_wbslevel/) | Ruft einen Wert von WBSLevel ab. |
| [get_Work](./get_work/) | Ruft einen Wert von Work ab. |
| [get_WorkVariance](./get_workvariance/) | Liest einen Wert von WorkVariance. |
| [GetHashCode](./gethashcode/) | Gibt einen Hashcode‑Wert für diese Task zurück. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Gibt ein TimephasedDataCollection‑Objekt mit TimephasedData‑Werten innerhalb der angegebenen Start‑ und Enddaten zurück. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Verschiebt die aktuelle Aufgabe auf derselben Outline‑Ebene vor die angegebene Aufgabe. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach Verwendung dieser Methode Project.Recalculate() aufrufen (dies wird alle Projektaufgaben neu planen (Start‑/Enddaten, setzt Früh‑/Spättermine) und die abhängigen Felder wie Puffer, Arbeits‑ und Kostenfelder sowie Outline‑Ebenen berechnen). Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur Aufgaben‑ID, Outline‑Ebene und Outline‑Nummern automatisch. Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Projektaufgaben automatisch neu (Start‑/Enddaten, setzt Früh‑/Spättermine, berechnet Puffer, Arbeits‑ und Kostenfelder, recalculates IDs und Outline‑Ebenen). |
| [OutlineIndent](./outlineindent/) | Rückt eine Aufgabe in der Gliederung ein. |
| [OutlineOutdent](./outlineoutdent/) | Hebt eine Aufgabe in der Gliederung hervor. |
| [SelectAllChildTasks](./selectallchildtasks/) | Sammelt rekursiv alle Unteraufgaben dieser Aufgabe. |
| [Set](./set/) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [set_ActivityId](./set_activityid/) | Stellt das Aktivitäts‑ID‑Feld dar – die eindeutige Kennung einer Aufgabe, die von Primavera verwendet wird. (nur für Primavera‑Projekte anwendbar). |
| [set_ActualCost](./set_actualcost/) | Setzt einen Wert von ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Setzt einen Wert von ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Setzt einen Wert für ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Setzt einen Wert von ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Setzt einen Wert von ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Setzt einen Wert von ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Setzt einen Wert für ActualStart. |
| [set_ActualWork](./set_actualwork/) | Setzt einen Wert von ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Setzt einen Wert von ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Setzt einen Wert von ACWP. |
| [set_Baselines](./set_baselines/) | Setzt die Sammlung von Basiswerten der Aufgabe. |
| [set_BCWP](./set_bcwp/) | Setzt einen Wert von BCWP. |
| [set_BCWS](./set_bcws/) | Setzt einen Wert von BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Setzt einen Wert von BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Setzt einen Wert von BudgetWork. |
| [set_Calendar](./set_calendar/) | Setzt einen Wert von Calendar. |
| [set_CommitmentFinish](./set_commitmentfinish/) | Setzt einen Wert von CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Setzt einen Wert von CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Setzt einen Wert von CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Setzt einen Wert von ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Setzt einen Wert von ConstraintType. |
| [set_Contact](./set_contact/) | Setzt einen Wert für Contact. |
| [set_Cost](./set_cost/) | Setzt einen Wert von Cost. |
| [set_CostVariance](./set_costvariance/) | Setzt einen Wert von CostVariance. |
| [set_Created](./set_created/) | Setzt einen Wert von Created. |
| [set_CV](./set_cv/) | Setzt einen Wert von CV. |
| [set_Deadline](./set_deadline/) | Setzt einen Wert für Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Setzt einen Wert, der angibt, ob DisplayAsSummary gesetzt ist oder nicht. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Setzt einen Wert, der angibt, ob DisplayOnTimeline gesetzt ist oder nicht. |
| [set_Duration](./set_duration/) | Setzt einen Wert für Duration. |
| [set_DurationFormat](./set_durationformat/) | Setzt einen Wert von DurationFormat. |
| [set_DurationText](./set_durationtext/) | Setzt einen Wert für DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Setzt einen Wert für DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Setzt einen Wert für EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Setzt einen Wert für EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Setzt einen Wert von EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Setzt einen Wert für ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Setzt einen Wert für ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Liest oder setzt die eindeutige Kennung der externen Aufgabe, wenn die Aufgabe extern ist. |
| [set_Finish](./set_finish/) | Setzt einen Wert von Finish. |
| [set_FinishSlack](./set_finishslack/) | Setzt einen Wert für FinishSlack. |
| [set_FinishText](./set_finishtext/) | Setzt einen Wert für FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Legt einen Wert für FinishVariance fest. |
| [set_FixedCost](./set_fixedcost/) | Setzt einen Wert für FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Setzt einen Wert für FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Setzt einen Wert für FreeSlack. |
| [set_Guid](./set_guid/) | Setzt einen Wert von Guid. |
| [set_HideBar](./set_hidebar/) | Setzt einen Wert, der angibt, ob HideBar gesetzt ist oder nicht. |
| [set_Hyperlink](./set_hyperlink/) | Setzt den Titel oder erläuternden Text für einen mit einer Aufgabe verknüpften Hyperlink. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Setzt die Adresse für einen mit einer Aufgabe verknüpften Hyperlink. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Setzt den spezifischen Ort in einem Dokument in einem mit einer Aufgabe verknüpften Hyperlink. |
| [set_Id](./set_id/) | Setzt einen Wert von Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Setzt einen Wert, der angibt, ob IgnoreResourceCalendar gesetzt ist oder nicht. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Setzt einen Wert, der angibt, ob IgnoreWarnings gesetzt ist oder nicht. |
| [set_IsActive](./set_isactive/) | Setzt einen Wert, der angibt, ob IsActive gesetzt ist oder nicht. |
| [set_IsCritical](./set_iscritical/) | Setzt einen Wert, der angibt, ob IsCritical gesetzt ist oder nicht. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Setzt einen Wert, der angibt, ob IsEffortDriven gesetzt ist oder nicht. |
| [set_IsEstimated](./set_isestimated/) | Legt einen Wert fest, der angibt, ob IsEstimated gesetzt ist oder nicht. |
| [set_IsExpanded](./set_isexpanded/) | Legt einen Wert fest, der angibt, ob IsExpanded gesetzt ist oder nicht. |
| [set_IsExternalTask](./set_isexternaltask/) | Legt einen Wert fest, der angibt, ob IsExternalTask gesetzt ist oder nicht. |
| [set_IsManual](./set_ismanual/) | Legt einen Wert fest, der angibt, ob IsManual gesetzt ist oder nicht. |
| [set_IsMarked](./set_ismarked/) | Legt einen Wert fest, der angibt, ob IsMarked gesetzt ist oder nicht. |
| [set_IsMilestone](./set_ismilestone/) | Legt einen Wert fest, der angibt, ob IsMilestone gesetzt ist oder nicht. |
| [set_IsNull](./set_isnull/) | Setzt einen Wert, der angibt, ob IsNull gesetzt ist oder nicht. |
| [set_IsOverallocated](./set_isoverallocated/) | Legt einen Wert fest, der angibt, ob IsOverallocated gesetzt ist oder nicht. |
| [set_IsPublished](./set_ispublished/) | Legt einen Wert fest, der angibt, ob IsPublished gesetzt ist oder nicht. |
| [set_IsRecurring](./set_isrecurring/) | Legt einen Wert fest, der angibt, ob IsRecurring gesetzt ist oder nicht. |
| [set_IsResumeValid](./set_isresumevalid/) | Legt einen Wert fest, der angibt, ob IsResumeValid gesetzt ist oder nicht. |
| [set_IsRollup](./set_isrollup/) | Legt einen Wert fest, der angibt, ob IsRollup gesetzt ist oder nicht. |
| [set_IsSubproject](./set_issubproject/) | Legt einen Wert fest, der angibt, ob IsSubproject gesetzt ist oder nicht. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Legt einen Wert fest, der angibt, ob IsSubprojectReadOnly gesetzt ist oder nicht. |
| [set_IsSummary](./set_issummary/) | Legt einen Wert fest, der angibt, ob IsSummary gesetzt ist oder nicht. |
| [set_LateFinish](./set_latefinish/) | Legt einen Wert für LateFinish fest. |
| [set_LateStart](./set_latestart/) | Legt einen Wert für LateStart fest. |
| [set_LevelAssignments](./set_levelassignments/) | Legt einen Wert fest, der angibt, ob LevelAssignments gesetzt ist oder nicht. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Legt einen Wert fest, der angibt, ob LevelingCanSplit gesetzt ist oder nicht. |
| [set_LevelingDelay](./set_levelingdelay/) | Legt einen Wert für LevelingDelay fest. |
| [set_ManualDuration](./set_manualduration/) | Legt einen Wert für ManualDuration fest. |
| [set_ManualFinish](./set_manualfinish/) | Legt einen Wert für ManualFinish fest. |
| [set_ManualStart](./set_manualstart/) | Legt einen Wert für ManualStart fest. |
| [set_Name](./set_name/) | Setzt einen Wert von Name. |
| [set_NotesRTF](./set_notesrtf/) | Setzt einen Wert von NotesRTF. |
| [set_NotesText](./set_notestext/) | Setzt einen Wert von NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Legt das OutlineCodeCollection-Objekt fest. |
| [set_OutlineLevel](./set_outlinelevel/) | Legt einen Wert für OutlineLevel fest. |
| [set_OutlineNumber](./set_outlinenumber/) | Legt einen Wert für OutlineNumber fest. |
| [set_OvertimeCost](./set_overtimecost/) | Setzt einen Wert von OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Setzt einen Wert von OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Legt einen Wert für PercentComplete fest. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Setzt einen Wert von PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Setzt einen Wert für PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Setzt einen Wert für PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Setzt einen Wert für PreleveledStart. |
| [set_Priority](./set_priority/) | Setzt einen Wert für Priority. |
| [set_RegularWork](./set_regularwork/) | Setzt einen Wert von RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Setzt einen Wert von RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Setzt einen Wert für RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Setzt einen Wert von RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Setzt einen Wert von RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Setzt einen Wert von RemainingWork. |
| [set_Resume](./set_resume/) | Legt einen Wert für Resume fest. |
| [set_Start](./set_start/) | Setzt einen Wert von Start. |
| [set_StartSlack](./set_startslack/) | Setzt einen Wert für StartSlack. |
| [set_StartText](./set_starttext/) | Setzt einen Wert für StartText. |
| [set_StartVariance](./set_startvariance/) | Legt einen Wert für StartVariance fest. |
| [set_StatusManager](./set_statusmanager/) | Setzt einen Wert für StatusManager. |
| [set_Stop](./set_stop/) | Legt einen Wert für Stop fest. |
| [set_SubprojectName](./set_subprojectname/) | Setzt einen Wert für SubprojectName. |
| [set_SV](./set_sv/) | Die Earned-Value-Planabweichung bis zum Projektstatusdatum. Die Planabweichung (SV) ist die Differenz zwischen BCWP und BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Setzt ein TimephasedDataCollection-Objekt für diese Aufgabe. Der zeitlich gestufte Datenblock, der mit einer Aufgabe verknüpft ist. |
| [set_TotalSlack](./set_totalslack/) | Setzt einen Wert für TotalSlack. |
| [set_Type](./set_type/) | Setzt einen Wert von Type. |
| [set_Uid](./set_uid/) | Setzt einen Wert von Uid. |
| [set_Warning](./set_warning/) | Setzt einen Wert, der angibt, ob Warning gesetzt ist oder nicht. |
| [set_WBS](./set_wbs/) | Setzt einen Wert für WBS. |
| [set_WBSLevel](./set_wbslevel/) | Setzt einen Wert für WBSLevel. |
| [set_Work](./set_work/) | Setzt einen Wert von Work. |
| [set_WorkVariance](./set_workvariance/) | Setzt einen Wert für WorkVariance. |
| [ToString](./tostring/) | Gibt eine kurze Zeichenkettenrepräsentation einer Aufgabe zurück. Die genauen Details der Darstellung sind nicht festgelegt und können sich ändern. |

