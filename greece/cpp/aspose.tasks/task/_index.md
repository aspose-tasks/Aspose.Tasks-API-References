---
title: "Aspose::Tasks::Task κλάση"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks για C++"
description: "Αντιπροσωπεύει μια εργασία σε ένα έργο."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Αντιπροσωπεύει μια εργασία σε ένα έργο.

Η Task αντιπροσωπεύει ένα ενιαίο ατομικό τμήμα εργασίας.

Μπορεί κανείς να χρησιμοποιήσει την Task για να σχεδιάσει ένα έργο δημιουργώντας Tasks και αναθέτοντας κατάλληλους πόρους σε αυτές. Τα Tasks σε ένα έργο οργανώνονται ως μια ιεραρχική δομή δέντρου με ρίζα, με μια ριζική Task και υποδέντρα παιδικών Tasks.

Για να δημιουργήσετε ένα δέντρο εργασιών, μπορείτε να χρησιμοποιήσετε μια εξειδικευμένη συλλογή Aspose::Tasks::TaskCollection προσπελαύνοντας την ιδιότητα Project::RootTask, π.χ.:

```cpp
Project project = new Project();
 
// προσθέστε νέες εργασίες
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
 
// αποθηκεύστε το έργο σε μία από τις διαθέσιμες μορφές
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Clone](./clone/) | Δημιουργεί πλήρη αντίγραφο μιας εργασίας χωρίς υποεργασίες. |
| [Delete](./delete/) | Διαγράφει μια εργασία από τη συλλογή εργασιών του γονικού έργου και όλες τις αναθέσεις της. |
| [Equals (2 overloads)](./equals/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτό το αντίγραφο είναι ίσο με ένα καθορισμένο αντικείμενο. |
| [Get](./get/) | Επιστρέφει την τιμή στην οποία αντιστοιχεί η ιδιότητα σε αυτό το κοντέινερ. |
| [get_ActivityId](./get_activityid/) | Αντιπροσωπεύει το πεδίο αναγνωριστικού δραστηριότητας - το μοναδικό αναγνωριστικό μιας εργασίας που χρησιμοποιείται από το Primavera. (ισχύει μόνο για έργα Primavera). |
| [get_ActualCost](./get_actualcost/) | Λαμβάνει μια τιμή του ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Λαμβάνει μια τιμή του ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Λαμβάνει μια τιμή του ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Λαμβάνει μια τιμή του ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Λαμβάνει μια τιμή του ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Λαμβάνει μια τιμή του ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Λαμβάνει μια τιμή του ActualStart. |
| [get_ActualWork](./get_actualwork/) | Λαμβάνει μια τιμή του ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Λαμβάνει μια τιμή του ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Λαμβάνει μια τιμή του ACWP. |
| [get_Assignments](./get_assignments/) | Λαμβάνει μια συλλογή από αναθέσεις πόρων για αυτό το αντικείμενο. |
| [get_Baselines](./get_baselines/) | Λαμβάνει τη συλλογή των βασικών τιμών της εργασίας. |
| [get_BCWP](./get_bcwp/) | Λαμβάνει μια τιμή του BCWP. |
| [get_BCWS](./get_bcws/) | Λαμβάνει μια τιμή του BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Λαμβάνει μια τιμή του BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Λαμβάνει μια τιμή του BudgetWork. |
| [get_Calendar](./get_calendar/) | Λαμβάνει μια τιμή του Calendar. |
| [get_Children](./get_children/) | Λαμβάνει μια συλλογή υποεργασιών αυτού του αντικειμένου. Αντικείμενο TaskCollection που αντιπροσωπεύει τις υποεργασίες. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Λαμβάνει μια τιμή του CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Λαμβάνει μια τιμή του CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Λαμβάνει μια τιμή του CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Λαμβάνει μια τιμή του ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Λαμβάνει μια τιμή του ConstraintType. |
| [get_Contact](./get_contact/) | Λαμβάνει μια τιμή του Contact. |
| [get_Cost](./get_cost/) | Λαμβάνει μια τιμή του Cost. |
| [get_CostVariance](./get_costvariance/) | Λαμβάνει μια τιμή του CostVariance. |
| [get_Created](./get_created/) | Λαμβάνει μια τιμή του Created. |
| [get_CV](./get_cv/) | Λαμβάνει μια τιμή του CV. |
| [get_Deadline](./get_deadline/) | Λαμβάνει μια τιμή του Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το DisplayAsSummary είναι ορισμένο ή όχι. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το DisplayOnTimeline είναι ορισμένο ή όχι. |
| [get_Duration](./get_duration/) | Λαμβάνει μια τιμή του Duration. |
| [get_DurationFormat](./get_durationformat/) | Λαμβάνει τιμή του DurationFormat. |
| [get_DurationText](./get_durationtext/) | Λαμβάνει μια τιμή του DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Λαμβάνει μια τιμή του DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Λαμβάνει μια τιμή του EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Λαμβάνει μια τιμή του EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Λαμβάνει τιμή του EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Λαμβάνει το αντικείμενο ExtendedAttributeCollection που περιέχει τις τιμές μιας εκτεταμένης ιδιότητας. |
| [get_ExternalId](./get_externalid/) | Λαμβάνει μια τιμή του ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Λαμβάνει μια τιμή του ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό της εξωτερικής εργασίας όταν η εργασία είναι εξωτερική. |
| [get_Finish](./get_finish/) | Λαμβάνει μια τιμή του Finish. |
| [get_FinishSlack](./get_finishslack/) | Λαμβάνει μια τιμή του FinishSlack. |
| [get_FinishText](./get_finishtext/) | Λαμβάνει μια τιμή του FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Λαμβάνει μια τιμή του FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Λαμβάνει μια τιμή του FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Λαμβάνει μια τιμή του FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Λαμβάνει μια τιμή του FreeSlack. |
| [get_Guid](./get_guid/) | Λαμβάνει μια τιμή του Guid. |
| [get_HideBar](./get_hidebar/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το HideBar είναι ορισμένο ή όχι. |
| [get_Hyperlink](./get_hyperlink/) | Λαμβάνει τον τίτλο ή το επεξηγηματικό κείμενο για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Λαμβάνει τη διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Λαμβάνει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [get_Id](./get_id/) | Λαμβάνει μια τιμή του Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IgnoreResourceCalendar είναι ορισμένο ή όχι. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IgnoreWarnings είναι ορισμένο ή όχι. |
| [get_IsActive](./get_isactive/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsActive είναι ορισμένο ή όχι. |
| [get_IsCritical](./get_iscritical/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsCritical είναι ορισμένο ή όχι. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsEffortDriven είναι ορισμένο ή όχι. |
| [get_IsEstimated](./get_isestimated/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsEstimated είναι ορισμένο ή όχι. |
| [get_IsExpanded](./get_isexpanded/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsExpanded είναι ορισμένο ή όχι. |
| [get_IsExternalTask](./get_isexternaltask/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsExternalTask είναι ορισμένο ή όχι. |
| [get_IsManual](./get_ismanual/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsManual είναι ορισμένο ή όχι. |
| [get_IsMarked](./get_ismarked/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsMarked είναι ορισμένο ή όχι. |
| [get_IsMilestone](./get_ismilestone/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsMilestone είναι ορισμένο ή όχι. |
| [get_IsNull](./get_isnull/) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsNull είναι ορισμένο ή όχι. |
| [get_IsOverallocated](./get_isoverallocated/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsOverallocated είναι ορισμένο ή όχι. |
| [get_IsPublished](./get_ispublished/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsPublished είναι ορισμένο ή όχι. |
| [get_IsRecurring](./get_isrecurring/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsRecurring είναι ορισμένο ή όχι. |
| [get_IsResumeValid](./get_isresumevalid/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsResumeValid είναι ορισμένο ή όχι. |
| [get_IsRollup](./get_isrollup/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsRollup είναι ορισμένο ή όχι. |
| [get_IsSubproject](./get_issubproject/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsSubproject είναι ορισμένο ή όχι. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsSubprojectReadOnly είναι ορισμένο ή όχι. |
| [get_IsSummary](./get_issummary/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το IsSummary είναι ορισμένο ή όχι. |
| [get_LateFinish](./get_latefinish/) | Λαμβάνει μια τιμή του LateFinish. |
| [get_LateStart](./get_latestart/) | Λαμβάνει μια τιμή του LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το LevelAssignments έχει οριστεί ή όχι. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το LevelingCanSplit έχει οριστεί ή όχι. |
| [get_LevelingDelay](./get_levelingdelay/) | Λαμβάνει μια τιμή του LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Λαμβάνει μια τιμή του ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Λαμβάνει μια τιμή του ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Λαμβάνει μια τιμή του ManualStart. |
| [get_Name](./get_name/) | Λαμβάνει μια τιμή του Name. |
| [get_NotesRTF](./get_notesrtf/) | Λαμβάνει μια τιμή του NotesRTF. |
| [get_NotesText](./get_notestext/) | Λαμβάνει μια τιμή του NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Λαμβάνει το αντικείμενο OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Λαμβάνει μια τιμή του OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Λαμβάνει μια τιμή του OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Λαμβάνει μια τιμή του OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Λαμβάνει μια τιμή του OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Λαμβάνει το γονικό έργο μιας εργασίας. |
| [get_ParentTask](./get_parenttask/) | Λαμβάνει την γονική εργασία μιας εργασίας. |
| [get_PercentComplete](./get_percentcomplete/) | Λαμβάνει μια τιμή του PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Λαμβάνει μια τιμή του PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Λαμβάνει μια τιμή του PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Λαμβάνει ένα αντικείμενο TaskCollection που περιέχει όλους τους προκάτοχους αυτού του αντικειμένου Task. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Λαμβάνει μια τιμή του PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Λαμβάνει μια τιμή του PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για μια εργασία που διαβάστηκε από αρχείο Primavera. |
| [get_Priority](./get_priority/) | Λαμβάνει μια τιμή του Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Λαμβάνει την παρουσία της κλάσης RecurringTaskInfo για την εργασία που είναι επαναλαμβανόμενη εργασία· εάν η εργασία δεν είναι επαναλαμβανόμενη, τότε επιστρέφει null; |
| [get_RegularWork](./get_regularwork/) | Λαμβάνει μια τιμή του RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Λαμβάνει μια τιμή του RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Λαμβάνει μια τιμή του RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Λαμβάνει μια τιμή του RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Λαμβάνει μια τιμή του RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Λαμβάνει μια τιμή του RemainingWork. |
| [get_Resume](./get_resume/) | Λαμβάνει μια τιμή του Resume. |
| [get_SplitParts](./get_splitparts/) | Λαμβάνει μια συλλογή SplitPart που αντιπροσωπεύει τα τμήματα μιας εργασίας. |
| [get_Start](./get_start/) | Λαμβάνει μια τιμή του Start. |
| [get_StartSlack](./get_startslack/) | Λαμβάνει μια τιμή του StartSlack. |
| [get_StartText](./get_starttext/) | Λαμβάνει μια τιμή του StartText. |
| [get_StartVariance](./get_startvariance/) | Λαμβάνει μια τιμή του StartVariance. |
| [get_Status](./get_status/) | Λαμβάνει την κατάσταση της εργασίας. |
| [get_StatusManager](./get_statusmanager/) | Λαμβάνει μια τιμή του StatusManager. |
| [get_Stop](./get_stop/) | Λαμβάνει μια τιμή του Stop. |
| [get_SubprojectName](./get_subprojectname/) | Λαμβάνει μια τιμή του SubprojectName. |
| [get_Successors](./get_successors/) | Λαμβάνει ένα αντικείμενο TaskCollection που περιέχει όλους τους διαδόχους αυτού του αντικειμένου Task. |
| [get_SV](./get_sv/) | Η διαφορά προγράμματος αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Η διαφορά προγράμματος (SV) είναι η διαφορά μεταξύ των BCWP και BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Λαμβάνει ένα αντικείμενο TimephasedDataCollection για αυτήν την εργασία. Το μπλοκ δεδομένων χρονικής φάσης που σχετίζεται με μια εργασία. |
| [get_TotalSlack](./get_totalslack/) | Λαμβάνει μια τιμή του TotalSlack. |
| [get_Type](./get_type/) | Λαμβάνει μια τιμή του Type. |
| [get_Uid](./get_uid/) | Λαμβάνει μια τιμή του Uid. |
| [get_Warning](./get_warning/) | Λαμβάνει μια τιμή που υποδεικνύει αν το Warning έχει οριστεί ή όχι. |
| [get_WBS](./get_wbs/) | Λαμβάνει μια τιμή του WBS. |
| [get_WBSLevel](./get_wbslevel/) | Λαμβάνει μια τιμή του WBSLevel. |
| [get_Work](./get_work/) | Λαμβάνει μια τιμή του Work. |
| [get_WorkVariance](./get_workvariance/) | Λαμβάνει μια τιμή του WorkVariance. |
| [GetHashCode](./gethashcode/) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Επιστρέφει ένα αντικείμενο TimephasedDataCollection με τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Μετακινεί την τρέχουσα εργασία στο ίδιο επίπεδο περιγράμματος πριν από την καθορισμένη εργασία. Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει το Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργότερες ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως οι ελεύθεροι χρόνοι, τα πεδία εργασίας και κόστους, τα επίπεδα περιγράμματος). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το αναγνωριστικό εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργότερες ημερομηνίες, υπολογίζει ελεύθερους χρόνους, πεδία εργασίας και κόστους, επαναϋπολογίζει τα αναγνωριστικά και τα επίπεδα περιγράμματος). |
| [OutlineIndent](./outlineindent/) | Δημιουργεί εσοχή σε μια εργασία στο περίγραμμα. |
| [OutlineOutdent](./outlineoutdent/) | Αναβαθμίζει μια εργασία στο περίγραμμα. |
| [SelectAllChildTasks](./selectallchildtasks/) | Συλλέγει αναδρομικά όλες τις θυγατρικές εργασίες αυτής της εργασίας. |
| [Set](./set/) | Αντιστοιχεί την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [set_ActivityId](./set_activityid/) | Αντιπροσωπεύει το πεδίο αναγνωριστικού δραστηριότητας - το μοναδικό αναγνωριστικό μιας εργασίας που χρησιμοποιείται από το Primavera. (ισχύει μόνο για έργα Primavera). |
| [set_ActualCost](./set_actualcost/) | Ορίζει μια τιμή του ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Ορίζει μια τιμή του ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Ορίζει μια τιμή του ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Ορίζει μια τιμή του ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Ορίζει μια τιμή του ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Ορίζει μια τιμή του ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Ορίζει μια τιμή του ActualStart. |
| [set_ActualWork](./set_actualwork/) | Ορίζει μια τιμή του ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Ορίζει μια τιμή του ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Ορίζει μια τιμή του ACWP. |
| [set_Baselines](./set_baselines/) | Ορίζει τη συλλογή των τιμών βάσης της εργασίας. |
| [set_BCWP](./set_bcwp/) | Ορίζει μια τιμή του BCWP. |
| [set_BCWS](./set_bcws/) | Ορίζει μια τιμή του BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Ορίζει μια τιμή του BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Ορίζει μια τιμή του BudgetWork. |
| [set_Calendar](./set_calendar/) | Ορίζει μια τιμή του Calendar. |
| [set_CommitmentFinish](./set_commitmentfinish/) | Ορίζει μια τιμή του CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Ορίζει μια τιμή του CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Ορίζει μια τιμή του CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Ορίζει μια τιμή του ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Ορίζει μια τιμή του ConstraintType. |
| [set_Contact](./set_contact/) | Ορίζει μια τιμή του Contact. |
| [set_Cost](./set_cost/) | Ορίζει μια τιμή του Cost. |
| [set_CostVariance](./set_costvariance/) | Ορίζει μια τιμή του CostVariance. |
| [set_Created](./set_created/) | Ορίζει μια τιμή του Created. |
| [set_CV](./set_cv/) | Ορίζει μια τιμή του CV. |
| [set_Deadline](./set_deadline/) | Ορίζει μια τιμή του Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Ορίζει μια τιμή που υποδεικνύει αν το DisplayAsSummary είναι ορισμένο ή όχι. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Ορίζει μια τιμή που υποδεικνύει αν το DisplayOnTimeline είναι ορισμένο ή όχι. |
| [set_Duration](./set_duration/) | Ορίζει μια τιμή του Duration . |
| [set_DurationFormat](./set_durationformat/) | Ορίζει μια τιμή του DurationFormat. |
| [set_DurationText](./set_durationtext/) | Ορίζει μια τιμή του DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Ορίζει μια τιμή του DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Ορίζει μια τιμή του EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Ορίζει μια τιμή του EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Ορίζει μια τιμή του EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Ορίζει μια τιμή του ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Ορίζει μια τιμή του ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό της εξωτερικής εργασίας όταν η εργασία είναι εξωτερική. |
| [set_Finish](./set_finish/) | Ορίζει μια τιμή του Finish. |
| [set_FinishSlack](./set_finishslack/) | Ορίζει μια τιμή του FinishSlack. |
| [set_FinishText](./set_finishtext/) | Ορίζει μια τιμή του FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Ορίζει μια τιμή του FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Ορίζει μια τιμή του FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Ορίζει μια τιμή του FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Ορίζει μια τιμή του FreeSlack. |
| [set_Guid](./set_guid/) | Ορίζει μια τιμή του Guid. |
| [set_HideBar](./set_hidebar/) | Ορίζει μια τιμή που υποδεικνύει αν το HideBar είναι ορισμένο ή όχι. |
| [set_Hyperlink](./set_hyperlink/) | Ορίζει τον τίτλο ή το επεξηγηματικό κείμενο για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Ορίζει τη διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Ορίζει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [set_Id](./set_id/) | Ορίζει μια τιμή του Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Ορίζει μια τιμή που υποδεικνύει αν το IgnoreResourceCalendar είναι ορισμένο ή όχι. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Ορίζει μια τιμή που υποδεικνύει αν το IgnoreWarnings είναι ορισμένο ή όχι. |
| [set_IsActive](./set_isactive/) | Ορίζει μια τιμή που υποδεικνύει αν το IsActive είναι ορισμένο ή όχι. |
| [set_IsCritical](./set_iscritical/) | Ορίζει μια τιμή που υποδεικνύει αν το IsCritical είναι ορισμένο ή όχι. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Ορίζει μια τιμή που υποδεικνύει αν το IsEffortDriven είναι ορισμένο ή όχι. |
| [set_IsEstimated](./set_isestimated/) | Ορίζει μια τιμή που υποδεικνύει αν το IsEstimated είναι ορισμένο ή όχι. |
| [set_IsExpanded](./set_isexpanded/) | Ορίζει μια τιμή που υποδεικνύει αν το IsExpanded είναι ορισμένο ή όχι. |
| [set_IsExternalTask](./set_isexternaltask/) | Ορίζει μια τιμή που υποδεικνύει αν το IsExternalTask είναι ορισμένο ή όχι. |
| [set_IsManual](./set_ismanual/) | Ορίζει μια τιμή που υποδεικνύει αν το IsManual είναι ορισμένο ή όχι. |
| [set_IsMarked](./set_ismarked/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsMarked είναι ορισμένο ή όχι. |
| [set_IsMilestone](./set_ismilestone/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsMilestone είναι ορισμένο ή όχι. |
| [set_IsNull](./set_isnull/) | Ορίζει μια τιμή που υποδεικνύει αν το IsNull είναι ορισμένο ή όχι. |
| [set_IsOverallocated](./set_isoverallocated/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsOverallocated είναι ορισμένο ή όχι. |
| [set_IsPublished](./set_ispublished/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsPublished είναι ορισμένο ή όχι. |
| [set_IsRecurring](./set_isrecurring/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsRecurring είναι ορισμένο ή όχι. |
| [set_IsResumeValid](./set_isresumevalid/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsResumeValid είναι ορισμένο ή όχι. |
| [set_IsRollup](./set_isrollup/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsRollup είναι ορισμένο ή όχι. |
| [set_IsSubproject](./set_issubproject/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsSubproject είναι ορισμένο ή όχι. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsSubprojectReadOnly είναι ορισμένο ή όχι. |
| [set_IsSummary](./set_issummary/) | Ορίζει μια τιμή που υποδεικνύει εάν το IsSummary είναι ορισμένο ή όχι. |
| [set_LateFinish](./set_latefinish/) | Ορίζει μια τιμή του LateFinish. |
| [set_LateStart](./set_latestart/) | Ορίζει μια τιμή του LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Ορίζει μια τιμή που υποδεικνύει εάν το LevelAssignments είναι ορισμένο ή όχι. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Ορίζει μια τιμή που υποδεικνύει εάν το LevelingCanSplit είναι ορισμένο ή όχι. |
| [set_LevelingDelay](./set_levelingdelay/) | Ορίζει μια τιμή του LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Ορίζει μια τιμή του ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Ορίζει μια τιμή του ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Ορίζει μια τιμή του ManualStart. |
| [set_Name](./set_name/) | Ορίζει μια τιμή του Name. |
| [set_NotesRTF](./set_notesrtf/) | Ορίζει μια τιμή του NotesRTF. |
| [set_NotesText](./set_notestext/) | Ορίζει μια τιμή του NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Ορίζει το αντικείμενο OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Ορίζει μια τιμή του OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Ορίζει μια τιμή του OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Ορίζει μια τιμή του OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Ορίζει μια τιμή του OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Ορίζει μια τιμή του PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Ορίζει μια τιμή του PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Ορίζει μια τιμή του PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Ορίζει μια τιμή του PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Ορίζει μια τιμή του PreleveledStart. |
| [set_Priority](./set_priority/) | Ορίζει μια τιμή του Priority. |
| [set_RegularWork](./set_regularwork/) | Ορίζει μια τιμή του RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Ορίζει μια τιμή του RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Ορίζει μια τιμή του RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Ορίζει μια τιμή του RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Ορίζει μια τιμή του RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Ορίζει μια τιμή του RemainingWork. |
| [set_Resume](./set_resume/) | Ορίζει μια τιμή του Resume. |
| [set_Start](./set_start/) | Ορίζει μια τιμή του Start. |
| [set_StartSlack](./set_startslack/) | Ορίζει μια τιμή του StartSlack. |
| [set_StartText](./set_starttext/) | Ορίζει μια τιμή του StartText. |
| [set_StartVariance](./set_startvariance/) | Ορίζει μια τιμή του StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Ορίζει μια τιμή του StatusManager. |
| [set_Stop](./set_stop/) | Ορίζει μια τιμή του Stop. |
| [set_SubprojectName](./set_subprojectname/) | Ορίζει μια τιμή του SubprojectName. |
| [set_SV](./set_sv/) | Η διαφορά προγράμματος αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Η διαφορά προγράμματος (SV) είναι η διαφορά μεταξύ των BCWP και BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Ορίζει ένα αντικείμενο TimephasedDataCollection για αυτήν την εργασία. Το μπλοκ δεδομένων χρονικής φάσης που σχετίζεται με μια εργασία. |
| [set_TotalSlack](./set_totalslack/) | Ορίζει μια τιμή του TotalSlack. |
| [set_Type](./set_type/) | Ορίζει μια τιμή του Type. |
| [set_Uid](./set_uid/) | Ορίζει μια τιμή του Uid. |
| [set_Warning](./set_warning/) | Ορίζει μια τιμή που υποδεικνύει εάν το Warning είναι ορισμένο ή όχι. |
| [set_WBS](./set_wbs/) | Ορίζει μια τιμή του WBS. |
| [set_WBSLevel](./set_wbslevel/) | Ορίζει μια τιμή του WBSLevel. |
| [set_Work](./set_work/) | Ορίζει μια τιμή του Work. |
| [set_WorkVariance](./set_workvariance/) | Ορίζει μια τιμή του WorkVariance. |
| [ToString](./tostring/) | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς μιας εργασίας. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν έχουν οριστεί και ενδέχεται να αλλάξουν. |

