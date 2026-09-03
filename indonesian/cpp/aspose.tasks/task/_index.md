---
title: "Aspose::Tasks::Task kelas"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks untuk C++"
description: "Mewakili sebuah tugas dalam sebuah proyek."
type: docs
weight: 10
url: /id/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Mewakili sebuah tugas dalam sebuah proyek.

Task mewakili satu potongan kerja atomik.

Seseorang dapat menggunakan Task untuk merencanakan proyek dengan membuat tugas dan menugaskan sumber daya yang sesuai ke dalamnya. Tugas dalam sebuah proyek diatur sebagai struktur pohon hierarki berakar, dengan tugas akar dan subpohon tugas anak.

Untuk membangun pohon tugas, Anda dapat menggunakan koleksi khusus Aspose::Tasks::TaskCollection dengan mengakses properti Project::RootTask, misalnya:

```cpp
Project project = new Project();
 
// tambahkan tugas baru
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
 
// simpan proyek dalam salah satu format yang tersedia
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Clone](./clone/) | Membuat salinan lengkap dari sebuah tugas tanpa subtugas. |
| [Delete](./delete/) | Menghapus tugas dari koleksi tugas proyek induk dan semua penugasannya. |
| [Equals (2 overloads)](./equals/) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [Get](./get/) | Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini. |
| [get_ActivityId](./get_activityid/) | Mewakili field id aktivitas - pengidentifikasi unik sebuah tugas yang digunakan oleh Primavera. (hanya berlaku untuk proyek Primavera). |
| [get_ActualCost](./get_actualcost/) | Mendapatkan nilai ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Mendapatkan nilai ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Mengambil nilai ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Mendapatkan nilai ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Mendapatkan nilai ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Mendapatkan nilai ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Mengambil nilai ActualStart. |
| [get_ActualWork](./get_actualwork/) | Mendapatkan nilai ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Mendapatkan nilai ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Mendapatkan nilai ACWP. |
| [get_Assignments](./get_assignments/) | Mendapatkan koleksi penugasan sumber daya untuk objek ini. |
| [get_Baselines](./get_baselines/) | Mendapatkan koleksi nilai baseline dari tugas. |
| [get_BCWP](./get_bcwp/) | Mendapatkan nilai BCWP. |
| [get_BCWS](./get_bcws/) | Mendapatkan nilai BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Mendapatkan nilai BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Mendapatkan nilai BudgetWork. |
| [get_Calendar](./get_calendar/) | Mendapatkan nilai Calendar. |
| [get_Children](./get_children/) | Mendapatkan koleksi tugas anak dari objek ini. Objek TaskCollection yang mewakili tugas-tugas anak. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Mendapatkan nilai CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Mendapatkan nilai CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Mendapatkan nilai CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Mendapatkan nilai ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Mendapatkan nilai ConstraintType. |
| [get_Contact](./get_contact/) | Mendapatkan nilai Contact. |
| [get_Cost](./get_cost/) | Mendapatkan nilai Cost. |
| [get_CostVariance](./get_costvariance/) | Mendapatkan nilai CostVariance. |
| [get_Created](./get_created/) | Mendapatkan nilai Created. |
| [get_CV](./get_cv/) | Mendapatkan nilai CV. |
| [get_Deadline](./get_deadline/) | Mendapatkan nilai Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Mendapatkan nilai yang menunjukkan apakah DisplayAsSummary diatur atau tidak. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Mendapatkan nilai yang menunjukkan apakah DisplayOnTimeline diatur atau tidak. |
| [get_Duration](./get_duration/) | Mendapatkan nilai Duration. |
| [get_DurationFormat](./get_durationformat/) | Mendapatkan nilai dari DurationFormat. |
| [get_DurationText](./get_durationtext/) | Mendapatkan nilai DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Mendapatkan nilai DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Mendapatkan nilai EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Mendapatkan nilai EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Mendapatkan nilai dari EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Mendapatkan objek ExtendedAttributeCollection yang berisi nilai-nilai atribut tambahan. |
| [get_ExternalId](./get_externalid/) | Mendapatkan nilai ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Mendapatkan nilai ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Mendapatkan atau mengatur pengidentifikasi unik tugas eksternal ketika tugas tersebut eksternal. |
| [get_Finish](./get_finish/) | Mendapatkan nilai Finish. |
| [get_FinishSlack](./get_finishslack/) | Mendapatkan nilai FinishSlack. |
| [get_FinishText](./get_finishtext/) | Mendapatkan nilai FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Mengambil nilai FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Mendapatkan nilai FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Mendapatkan nilai FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Mendapatkan nilai FreeSlack. |
| [get_Guid](./get_guid/) | Mendapatkan nilai Guid. |
| [get_HideBar](./get_hidebar/) | Mendapatkan nilai yang menunjukkan apakah HideBar diatur atau tidak. |
| [get_Hyperlink](./get_hyperlink/) | Mendapatkan judul atau teks penjelasan untuk hyperlink yang terkait dengan tugas. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Mendapatkan alamat untuk hyperlink yang terkait dengan tugas. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Mendapatkan lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan tugas. |
| [get_Id](./get_id/) | Mendapatkan nilai Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Mendapatkan nilai yang menunjukkan apakah IgnoreResourceCalendar diatur atau tidak. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Mendapatkan nilai yang menunjukkan apakah IgnoreWarnings diatur atau tidak. |
| [get_IsActive](./get_isactive/) | Mendapatkan nilai yang menunjukkan apakah IsActive diatur atau tidak. |
| [get_IsCritical](./get_iscritical/) | Mendapatkan nilai yang menunjukkan apakah IsCritical diatur atau tidak. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Mendapatkan nilai yang menunjukkan apakah IsEffortDriven diatur atau tidak. |
| [get_IsEstimated](./get_isestimated/) | Mendapatkan nilai yang menunjukkan apakah IsEstimated diatur atau tidak. |
| [get_IsExpanded](./get_isexpanded/) | Mendapatkan nilai yang menunjukkan apakah IsExpanded diatur atau tidak. |
| [get_IsExternalTask](./get_isexternaltask/) | Mendapatkan nilai yang menunjukkan apakah IsExternalTask diatur atau tidak. |
| [get_IsManual](./get_ismanual/) | Mendapatkan nilai yang menunjukkan apakah IsManual diatur atau tidak. |
| [get_IsMarked](./get_ismarked/) | Mendapatkan nilai yang menunjukkan apakah IsMarked diatur atau tidak. |
| [get_IsMilestone](./get_ismilestone/) | Mendapatkan nilai yang menunjukkan apakah IsMilestone diatur atau tidak. |
| [get_IsNull](./get_isnull/) | Mendapatkan nilai yang menunjukkan apakah IsNull diatur atau tidak. |
| [get_IsOverallocated](./get_isoverallocated/) | Mendapatkan nilai yang menunjukkan apakah IsOverallocated diatur atau tidak. |
| [get_IsPublished](./get_ispublished/) | Mendapatkan nilai yang menunjukkan apakah IsPublished diatur atau tidak. |
| [get_IsRecurring](./get_isrecurring/) | Mendapatkan nilai yang menunjukkan apakah IsRecurring diatur atau tidak. |
| [get_IsResumeValid](./get_isresumevalid/) | Mendapatkan nilai yang menunjukkan apakah IsResumeValid diatur atau tidak. |
| [get_IsRollup](./get_isrollup/) | Mendapatkan nilai yang menunjukkan apakah IsRollup diatur atau tidak. |
| [get_IsSubproject](./get_issubproject/) | Mendapatkan nilai yang menunjukkan apakah IsSubproject diatur atau tidak. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Mendapatkan nilai yang menunjukkan apakah IsSubprojectReadOnly diatur atau tidak. |
| [get_IsSummary](./get_issummary/) | Mendapatkan nilai yang menunjukkan apakah IsSummary diatur atau tidak. |
| [get_LateFinish](./get_latefinish/) | Mendapatkan nilai LateFinish. |
| [get_LateStart](./get_latestart/) | Mendapatkan nilai LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Mendapatkan nilai yang menunjukkan apakah LevelAssignments diatur atau tidak. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Mendapatkan nilai yang menunjukkan apakah LevelingCanSplit diatur atau tidak. |
| [get_LevelingDelay](./get_levelingdelay/) | Mendapatkan nilai LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Mendapatkan nilai ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Mendapatkan nilai ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Mendapatkan nilai ManualStart. |
| [get_Name](./get_name/) | Mendapatkan nilai Name. |
| [get_NotesRTF](./get_notesrtf/) | Mendapatkan nilai NotesRTF. |
| [get_NotesText](./get_notestext/) | Mendapatkan nilai NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Mendapatkan objek OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Mendapatkan nilai OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Mendapatkan nilai OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Mendapatkan nilai OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Mendapatkan nilai OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Mendapatkan proyek induk dari sebuah tugas. |
| [get_ParentTask](./get_parenttask/) | Mendapatkan tugas induk dari sebuah tugas. |
| [get_PercentComplete](./get_percentcomplete/) | Mendapatkan nilai PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Mendapatkan nilai PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Mendapatkan nilai PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Mendapatkan objek TaskCollection yang berisi semua pendahulu dari objek Task ini. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Mendapatkan nilai PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Mendapatkan nilai PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Mendapatkan objek yang berisi properti khusus Primavera untuk sebuah tugas yang dibaca dari file Primavera. |
| [get_Priority](./get_priority/) | Mendapatkan nilai Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Mendapatkan instance kelas RecurringTaskInfo untuk tugas yang merupakan tugas berulang; jika tugas bukan tugas berulang maka mengembalikan null; |
| [get_RegularWork](./get_regularwork/) | Mendapatkan nilai RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Mendapatkan nilai RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Mendapatkan nilai RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Mendapatkan nilai RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Mendapatkan nilai RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Mendapatkan nilai RemainingWork. |
| [get_Resume](./get_resume/) | Mendapatkan nilai Resume. |
| [get_SplitParts](./get_splitparts/) | Mendapatkan koleksi SplitPart yang mewakili bagian-bagian dari sebuah tugas. |
| [get_Start](./get_start/) | Mendapatkan nilai Start. |
| [get_StartSlack](./get_startslack/) | Mendapatkan nilai StartSlack. |
| [get_StartText](./get_starttext/) | Mendapatkan nilai StartText. |
| [get_StartVariance](./get_startvariance/) | Mendapatkan nilai StartVariance. |
| [get_Status](./get_status/) | Mendapatkan status tugas. |
| [get_StatusManager](./get_statusmanager/) | Mendapatkan nilai StatusManager. |
| [get_Stop](./get_stop/) | Mendapatkan nilai Stop. |
| [get_SubprojectName](./get_subprojectname/) | Mendapatkan nilai SubprojectName. |
| [get_Successors](./get_successors/) | Mendapatkan objek TaskCollection yang berisi semua penerus dari objek Task ini. |
| [get_SV](./get_sv/) | Variansi jadwal nilai yang diperoleh, hingga tanggal status proyek. Variansi jadwal (SV) adalah selisih antara BCWP dan BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Mendapatkan objek TimephasedDataCollection dari tugas ini. Blok data berjangka waktu yang terkait dengan sebuah tugas. |
| [get_TotalSlack](./get_totalslack/) | Mendapatkan nilai TotalSlack. |
| [get_Type](./get_type/) | Mendapatkan nilai Type. |
| [get_Uid](./get_uid/) | Mendapatkan nilai Uid. |
| [get_Warning](./get_warning/) | Mendapatkan nilai yang menunjukkan apakah Warning diatur atau tidak. |
| [get_WBS](./get_wbs/) | Mendapatkan nilai WBS. |
| [get_WBSLevel](./get_wbslevel/) | Mendapatkan nilai WBSLevel. |
| [get_Work](./get_work/) | Mendapatkan nilai Work. |
| [get_WorkVariance](./get_workvariance/) | Mendapatkan nilai WorkVariance. |
| [GetHashCode](./gethashcode/) | Mengembalikan nilai kode hash untuk Task ini. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Mengembalikan objek TimephasedDataCollection dengan nilai TimephasedData dalam rentang tanggal mulai dan selesai yang diberikan. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwal ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwal ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline). |
| [OutlineIndent](./outlineindent/) | Memberi indentasi pada tugas dalam outline. |
| [OutlineOutdent](./outlineoutdent/) | Menaikkan tingkat tugas dalam outline. |
| [SelectAllChildTasks](./selectallchildtasks/) | Mengumpulkan secara rekursif semua tugas anak dari tugas ini. |
| [Set](./set/) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [set_ActivityId](./set_activityid/) | Mewakili field id aktivitas - pengidentifikasi unik sebuah tugas yang digunakan oleh Primavera. (hanya berlaku untuk proyek Primavera). |
| [set_ActualCost](./set_actualcost/) | Mengatur nilai ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Mengatur nilai ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Mengatur nilai ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Mengatur nilai ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Mengatur nilai ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Mengatur nilai ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Mengatur nilai ActualStart. |
| [set_ActualWork](./set_actualwork/) | Mengatur nilai ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Mengatur nilai ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Mengatur nilai ACWP. |
| [set_Baselines](./set_baselines/) | Mengatur koleksi nilai baseline dari tugas. |
| [set_BCWP](./set_bcwp/) | Mengatur nilai BCWP. |
| [set_BCWS](./set_bcws/) | Mengatur nilai BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Mengatur nilai BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Mengatur nilai BudgetWork. |
| [set_Calendar](./set_calendar/) | Mengatur nilai Calendar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | Mengatur nilai CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Mengatur nilai CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Mengatur nilai CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Mengatur nilai ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Mengatur nilai ConstraintType. |
| [set_Contact](./set_contact/) | Mengatur nilai Contact. |
| [set_Cost](./set_cost/) | Mengatur nilai Cost. |
| [set_CostVariance](./set_costvariance/) | Mengatur nilai CostVariance. |
| [set_Created](./set_created/) | Mengatur nilai Created. |
| [set_CV](./set_cv/) | Mengatur nilai CV. |
| [set_Deadline](./set_deadline/) | Mengatur nilai Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Mengatur nilai yang menunjukkan apakah DisplayAsSummary diatur atau tidak. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Mengatur nilai yang menunjukkan apakah DisplayOnTimeline diatur atau tidak. |
| [set_Duration](./set_duration/) | Mengatur nilai Duration. |
| [set_DurationFormat](./set_durationformat/) | Mengatur nilai DurationFormat. |
| [set_DurationText](./set_durationtext/) | Mengatur nilai DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Mengatur nilai DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Mengatur nilai EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Mengatur nilai EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Mengatur nilai EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Mengatur nilai ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Mengatur nilai ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Mendapatkan atau mengatur pengidentifikasi unik tugas eksternal ketika tugas tersebut eksternal. |
| [set_Finish](./set_finish/) | Mengatur nilai Finish. |
| [set_FinishSlack](./set_finishslack/) | Mengatur nilai FinishSlack. |
| [set_FinishText](./set_finishtext/) | Mengatur nilai FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Menetapkan nilai FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Mengatur nilai FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Mengatur nilai FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Mengatur nilai FreeSlack. |
| [set_Guid](./set_guid/) | Mengatur nilai Guid. |
| [set_HideBar](./set_hidebar/) | Mengatur nilai yang menunjukkan apakah HideBar diatur atau tidak. |
| [set_Hyperlink](./set_hyperlink/) | Mengatur judul atau teks penjelas untuk hyperlink yang terkait dengan tugas. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Mengatur alamat untuk hyperlink yang terkait dengan tugas. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Mengatur lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan tugas. |
| [set_Id](./set_id/) | Mengatur nilai Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Mengatur nilai yang menunjukkan apakah IgnoreResourceCalendar diatur atau tidak. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Mengatur nilai yang menunjukkan apakah IgnoreWarnings diatur atau tidak. |
| [set_IsActive](./set_isactive/) | Mengatur nilai yang menunjukkan apakah IsActive diatur atau tidak. |
| [set_IsCritical](./set_iscritical/) | Mengatur nilai yang menunjukkan apakah IsCritical diatur atau tidak. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Mengatur nilai yang menunjukkan apakah IsEffortDriven diatur atau tidak. |
| [set_IsEstimated](./set_isestimated/) | Mengatur nilai yang menunjukkan apakah IsEstimated diatur atau tidak. |
| [set_IsExpanded](./set_isexpanded/) | Mengatur nilai yang menunjukkan apakah IsExpanded diatur atau tidak. |
| [set_IsExternalTask](./set_isexternaltask/) | Mengatur nilai yang menunjukkan apakah IsExternalTask diatur atau tidak. |
| [set_IsManual](./set_ismanual/) | Mengatur nilai yang menunjukkan apakah IsManual diatur atau tidak. |
| [set_IsMarked](./set_ismarked/) | Mengatur nilai yang menunjukkan apakah IsMarked diatur atau tidak. |
| [set_IsMilestone](./set_ismilestone/) | Mengatur nilai yang menunjukkan apakah IsMilestone diatur atau tidak. |
| [set_IsNull](./set_isnull/) | Mengatur nilai yang menunjukkan apakah IsNull diatur atau tidak. |
| [set_IsOverallocated](./set_isoverallocated/) | Mengatur nilai yang menunjukkan apakah IsOverallocated diatur atau tidak. |
| [set_IsPublished](./set_ispublished/) | Mengatur nilai yang menunjukkan apakah IsPublished diatur atau tidak. |
| [set_IsRecurring](./set_isrecurring/) | Mengatur nilai yang menunjukkan apakah IsRecurring diatur atau tidak. |
| [set_IsResumeValid](./set_isresumevalid/) | Mengatur nilai yang menunjukkan apakah IsResumeValid diatur atau tidak. |
| [set_IsRollup](./set_isrollup/) | Mengatur nilai yang menunjukkan apakah IsRollup diatur atau tidak. |
| [set_IsSubproject](./set_issubproject/) | Mengatur nilai yang menunjukkan apakah IsSubproject diatur atau tidak. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Mengatur nilai yang menunjukkan apakah IsSubprojectReadOnly diatur atau tidak. |
| [set_IsSummary](./set_issummary/) | Mengatur nilai yang menunjukkan apakah IsSummary diatur atau tidak. |
| [set_LateFinish](./set_latefinish/) | Mengatur nilai LateFinish. |
| [set_LateStart](./set_latestart/) | Mengatur nilai LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Mengatur nilai yang menunjukkan apakah LevelAssignments diatur atau tidak. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Mengatur nilai yang menunjukkan apakah LevelingCanSplit diatur atau tidak. |
| [set_LevelingDelay](./set_levelingdelay/) | Menetapkan nilai LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Mengatur nilai ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Mengatur nilai ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Mengatur nilai ManualStart. |
| [set_Name](./set_name/) | Mengatur nilai Name. |
| [set_NotesRTF](./set_notesrtf/) | Mengatur nilai NotesRTF. |
| [set_NotesText](./set_notestext/) | Mengatur nilai NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Mengatur objek OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Mengatur nilai OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Mengatur nilai OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Mengatur nilai OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Mengatur nilai OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Mengatur nilai PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Mengatur nilai PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Mengatur nilai PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Mengatur nilai PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Mengatur nilai PreleveledStart. |
| [set_Priority](./set_priority/) | Mengatur nilai Priority. |
| [set_RegularWork](./set_regularwork/) | Mengatur nilai RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Mengatur nilai RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Mengatur nilai RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Mengatur nilai RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Mengatur nilai RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Mengatur nilai RemainingWork. |
| [set_Resume](./set_resume/) | Menetapkan nilai Resume. |
| [set_Start](./set_start/) | Mengatur nilai Start. |
| [set_StartSlack](./set_startslack/) | Mengatur nilai StartSlack. |
| [set_StartText](./set_starttext/) | Mengatur nilai StartText. |
| [set_StartVariance](./set_startvariance/) | Menetapkan nilai StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Mengatur nilai StatusManager. |
| [set_Stop](./set_stop/) | Menetapkan nilai Stop. |
| [set_SubprojectName](./set_subprojectname/) | Mengatur nilai SubprojectName. |
| [set_SV](./set_sv/) | Variansi jadwal nilai yang diperoleh, hingga tanggal status proyek. Variansi jadwal (SV) adalah selisih antara BCWP dan BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Mengatur objek TimephasedDataCollection dari tugas ini. Blok data berwaktu yang terkait dengan sebuah tugas. |
| [set_TotalSlack](./set_totalslack/) | Mengatur nilai TotalSlack. |
| [set_Type](./set_type/) | Mengatur nilai Type. |
| [set_Uid](./set_uid/) | Mengatur nilai Uid. |
| [set_Warning](./set_warning/) | Mengatur nilai yang menunjukkan apakah Warning diatur atau tidak. |
| [set_WBS](./set_wbs/) | Mengatur nilai WBS. |
| [set_WBSLevel](./set_wbslevel/) | Mengatur nilai WBSLevel. |
| [set_Work](./set_work/) | Mengatur nilai Work. |
| [set_WorkVariance](./set_workvariance/) | Mengatur nilai WorkVariance. |
| [ToString](./tostring/) | Mengembalikan representasi string singkat dari sebuah tugas. Detail tepat dari representasi tersebut tidak ditentukan dan dapat berubah. |

