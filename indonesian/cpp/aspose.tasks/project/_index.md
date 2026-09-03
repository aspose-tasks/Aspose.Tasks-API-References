---
title: "Kelas Aspose::Tasks::Project"
linktitle: "Proyek"
articleTitle: "Proyek"
second_title: "Aspose.Tasks untuk C++"
description: "Mewakili sebuah proyek."
type: docs
weight: 10
url: /id/cpp/aspose.tasks/project/
---

## Project class

Mewakili sebuah proyek.

Proyek adalah kelas pusat dalam pustaka Aspose.Tasks.

Anda dapat menggunakan Project untuk membaca salah satu format manajemen proyek yang didukung: MPP, MPT, MPX, XML.

Untuk memuat dokumen yang ada dalam salah satu format yang didukung, berikan nama file atau aliran ke salah satu konstruktor Project. Untuk membuat proyek kosong, panggil konstruktor tanpa parameter.

Gunakan salah satu overload metode Save untuk menyimpan proyek dalam format Aspose::Tasks::Saving::SaveFileFormat apa pun: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Tata Letak Tetap: PDF; Gambar: JPEG, PNG, BMP, TIFF, SVG; Teks: TXT; Lainnya: HTML.

Project menyimpan informasi seluruh proyek seperti Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps, dan Aspose::Tasks::Project::ExtendedAttributes. Sebagian besar objek ini dapat diakses melalui properti yang sesuai pada kelas Project.

Project adalah entitas akar yang berisi titik masuk untuk memanipulasi entitas proyek lainnya, seperti Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute, dan Aspose::Tasks::Calendar.

Entitas Project dapat diakses melalui koleksi bertipe, misalnya Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments, dll.

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Project (13 overloads)](./project/) | Menginisialisasi instance baru dari kelas Project. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Menyalin data utama dan properti proyek ke proyek lain. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Mengeumerasi secara rekursif semua tugas proyek termasuk tugas akar. |
| [Get](./get/) | Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini. |
| [get_ActualsInSync](./get_actualsinsync/) | Mendapatkan nilai yang menunjukkan apakah ActualsInSync diatur atau tidak. |
| [get_AdminProject](./get_adminproject/) | Mendapatkan nilai yang menunjukkan apakah AdminProject diatur atau tidak. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Mendapatkan nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak. |
| [get_Author](./get_author/) | Mendapatkan nilai Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Mendapatkan nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Mendapatkan apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya. |
| [get_Autolink](./get_autolink/) | Mendapatkan nilai yang menunjukkan apakah Autolink diatur atau tidak. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Mendapatkan nilai BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Mendapatkan koleksi properti bawaan proyek. |
| [get_CalculationMode](./get_calculationmode/) | Mendapatkan mode perhitungan sebuah proyek. Dapat berupa salah satu nilai dari enumerasi CalculationMode. |
| [get_Calendar](./get_calendar/) | Mendapatkan nilai Calendar. |
| [get_Calendars](./get_calendars/) | Mendapatkan objek CalendarCollection dari instance Project ini. |
| [get_Category](./get_category/) | Mendapatkan nilai Category. |
| [get_Comments](./get_comments/) | Mendapatkan nilai Comments. |
| [get_Company](./get_company/) | Mendapatkan nilai Company. |
| [get_CreationDate](./get_creationdate/) | Mendapatkan nilai CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Mendapatkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path proyek ini. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Mendapatkan nilai dari CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Mendapatkan nilai dari CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Mendapatkan nilai dari CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Mendapatkan nilai dari CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Mendapatkan nilai dari CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Mendapatkan nilai dari CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Mendapatkan nilai dari CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Mendapatkan koleksi properti khusus proyek. |
| [get_DateFormat](./get_dateformat/) | Mendapatkan nilai dari DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Mendapatkan nilai dari DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Mendapatkan nilai dari DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Mendapatkan nilai dari DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Mendapatkan nilai dari DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Mendapatkan nilai dari DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Mendapatkan nilai dari DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Mendapatkan nilai dari DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Mendapatkan nilai dari DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Mendapatkan tampilan default proyek. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Mendapatkan instance dari kelas WeekDayCollection yang mewakili koleksi hari kerja minggu default proyek dan jam kerja. |
| [get_DisplayOptions](./get_displayoptions/) | Mendapatkan instance dari kelas ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Mendapatkan nilai dari DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Mendapatkan nilai dari EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Mendapatkan objek ExtendedAttributeDefinitionCollection. Koleksi definisi atribut ekstensi (field khusus) yang terkait dengan sebuah proyek. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Mendapatkan nilai dari ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Mendapatkan nilai dari FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Mendapatkan nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak. |
| [get_FyStartDate](./get_fystartdate/) | Mendapatkan nilai FyStartDate. |
| [get_Guid](./get_guid/) | Mendapatkan nilai Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Mendapatkan nilai yang menunjukkan apakah HonorConstraints diatur atau tidak. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Mendapatkan nilai HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Mendapatkan nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Mendapatkan nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak. |
| [get_Keywords](./get_keywords/) | Mendapatkan nilai Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Mendapatkan nilai LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Mendapatkan nilai LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Mendapatkan nilai LastSaved. |
| [get_Manager](./get_manager/) | Mendapatkan nilai Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Mendapatkan nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak. |
| [get_MinutesPerDay](./get_minutesperday/) | Mendapatkan nilai MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Mendapatkan nilai MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Mendapatkan nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak. |
| [get_Name](./get_name/) | Mendapatkan nilai Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Mendapatkan nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Mendapatkan nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Mendapatkan nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Mendapatkan nilai NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Mendapatkan koleksi yang berisi instance kelas OleObject yang ditautkan atau disematkan ke file proyek ini. |
| [get_OutlineCodes](./get_outlinecodes/) | Mendapatkan objek OutlineCodeDefinitionCollection. Koleksi definisi kode outline yang terkait dengan sebuah proyek. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Mendapatkan objek yang berisi properti khusus Primavera untuk proyek yang dibaca dari file Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Mendapatkan nilai yang menunjukkan apakah ProjectExternallyEdited diatur atau tidak. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Mendapatkan nilai yang menunjukkan apakah RemoveFileProperties diatur atau tidak. |
| [get_ResourceAssignments](./get_resourceassignments/) | Mendapatkan objek ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Mendapatkan semua definisi filter berbasis sumber daya. ResourceFilters adalah koleksi objek Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Mendapatkan semua definisi grup berbasis sumber daya. ResourceGroups adalah koleksi objek Group. |
| [get_Resources](./get_resources/) | Mendapatkan objek ResourceCollection. |
| [get_Revision](./get_revision/) | Mendapatkan nilai Revision. |
| [get_RootTask](./get_roottask/) | Mendapatkan akar dari pohon tugas. |
| [get_SaveVersion](./get_saveversion/) | Mendapatkan nilai SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Mendapatkan nilai yang menunjukkan apakah ScheduleFromStart diatur atau tidak. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Mendapatkan nilai yang menunjukkan apakah ShowProjectSummaryTask diatur atau tidak. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Mendapatkan nilai yang menunjukkan apakah SplitsInProgressTasks diatur atau tidak. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Mendapatkan nilai yang menunjukkan apakah SpreadActualCost diatur atau tidak. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Mendapatkan nilai yang menunjukkan apakah SpreadPercentComplete diatur atau tidak. |
| [get_StartDate](./get_startdate/) | Mendapatkan nilai StartDate. |
| [get_StatusDate](./get_statusdate/) | Mendapatkan nilai StatusDate. |
| [get_Subject](./get_subject/) | Mendapatkan nilai Subject. |
| [get_Tables](./get_tables/) | Mendapatkan daftar objek Table. |
| [get_TaskFilters](./get_taskfilters/) | Mendapatkan semua definisi filter berbasis tugas. TaskFilters adalah koleksi objek Filter. |
| [get_TaskGroups](./get_taskgroups/) | Mendapatkan semua definisi grup berbasis tugas. TaskGroups adalah koleksi objek Group. |
| [get_TaskLinks](./get_tasklinks/) | Mendapatkan objek TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Mendapatkan nilai yang menunjukkan apakah TaskUpdatesResource diatur atau tidak. |
| [get_Template](./get_template/) | Mendapatkan nilai Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Mendapatkan nilai TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Mendapatkan nilai TimescaleStart. |
| [get_Title](./get_title/) | Mendapatkan nilai Title. |
| [get_Uid](./get_uid/) | Mendapatkan nilai Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Mendapatkan nilai yang menunjukkan apakah UpdateManuallyScheduledTasksWhenEditingLinks diatur atau tidak. |
| [get_VbaProject](./get_vbaproject/) | Mendapatkan instance kelas VbaProject. |
| [get_Views](./get_views/) | Mendapatkan daftar objek View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Mendapatkan Definisi Kode WBS untuk proyek. |
| [get_WeekStartDay](./get_weekstartday/) | Mendapatkan nilai WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Mendapatkan nilai WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Mengembalikan waktu penyimpanan baseline. |
| [GetDuration (3 overloads)](./getduration/) | Mendapatkan objek Duration dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale default (Hari). |
| [GetPredecessors](./getpredecessors/) | Mengembalikan koleksi tautan tugas yang merupakan pendahulu tugas yang ditentukan. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Mendapatkan info file proyek dari aliran. |
| [GetWork](./getwork/) | Mendapatkan objek Duration dengan nilai double yang ditentukan dan format kerja default. |
| [Recalculate (2 overloads)](./recalculate/) | Menjadwalkan ulang semua ids tugas proyek, level outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Menghitung ulang Id, Start, dan Finish sumber daya. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Menghitung ulang Start dan Finish sumber daya. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Menghilangkan penugasan sumber daya yang tidak valid dari daftar penugasan sumber daya proyek. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Menomori ulang kode WBS semua tugas. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Menjadwalkan ulang pekerjaan proyek yang belum selesai untuk mulai setelah tanggal tertentu. |
| [Save (5 overloads)](./save/) | Menyimpan proyek ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Menyimpan proyek sebagai templat ke aliran yang ditentukan. |
| [SaveReport (4 overloads)](./savereport/) | Menyimpan laporan ikhtisar proyek ke aliran. |
| [SelectAllChildTasks](./selectallchildtasks/) | Mengumpulkan secara rekursif semua tugas anak dari tugas root. |
| [Set (2 overloads)](./set/) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [set_ActualsInSync](./set_actualsinsync/) | Mengatur nilai yang menunjukkan apakah ActualsInSync diatur atau tidak. |
| [set_AdminProject](./set_adminproject/) | Mengatur nilai yang menunjukkan apakah AdminProject diatur atau tidak. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Mengatur nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak. |
| [set_Author](./set_author/) | Mengatur nilai Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Mengatur nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Mengatur apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya. |
| [set_Autolink](./set_autolink/) | Mengatur nilai yang menunjukkan apakah Autolink diatur atau tidak. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Mengatur nilai BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Mengatur mode perhitungan proyek. Dapat berupa salah satu nilai dari enumerasi CalculationMode. |
| [set_Calendar](./set_calendar/) | Mengatur nilai Calendar . |
| [set_Category](./set_category/) | Mengatur nilai Category. |
| [set_Comments](./set_comments/) | Mengatur nilai Comments. |
| [set_Company](./set_company/) | Mengatur nilai Company. |
| [set_CreationDate](./set_creationdate/) | Mengatur nilai CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Mengatur nilai CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Mengatur nilai CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Mengatur nilai CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Mengatur nilai CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Mengatur nilai CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Mengatur nilai CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Mengatur nilai CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Mengatur nilai DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Mengatur nilai DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Mengatur nilai DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Mengatur nilai DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Mengatur nilai DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Mengatur nilai DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Mengatur nilai DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Mengatur nilai DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Mengatur nilai DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Mengatur tampilan default proyek. |
| [set_DurationFormat](./set_durationformat/) | Mengatur nilai DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Mengatur nilai EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Mengatur nilai ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Mengatur nilai FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Mengatur nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak. |
| [set_FyStartDate](./set_fystartdate/) | Mengatur nilai FyStartDate. |
| [set_Guid](./set_guid/) | Mengatur nilai Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Mengatur nilai yang menunjukkan apakah HonorConstraints diatur atau tidak. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Mengatur nilai HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Mengatur nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Mengatur nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak. |
| [set_Keywords](./set_keywords/) | Mengatur nilai Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Mengatur nilai LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Mengatur nilai LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Mengatur nilai LastSaved. |
| [set_Manager](./set_manager/) | Mengatur nilai Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Mengatur nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak. |
| [set_MinutesPerDay](./set_minutesperday/) | Mengatur nilai MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Mengatur nilai MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Mengatur nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Mengatur nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Mengatur nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Mengatur nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Mengatur nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak. |
| [set_Name](./set_name/) | Mengatur nilai Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Mengatur nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Mengatur nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Mengatur nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Mengatur nilai NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Mengatur nilai yang menunjukkan apakah ProjectExternallyEdited diatur atau tidak. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Mengatur nilai yang menunjukkan apakah RemoveFileProperties diatur atau tidak. |
| [set_Revision](./set_revision/) | Mengatur nilai Revision. |
| [set_SaveVersion](./set_saveversion/) | Mengatur nilai SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Mengatur nilai yang menunjukkan apakah ScheduleFromStart diatur atau tidak. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Mengatur nilai yang menunjukkan apakah ShowProjectSummaryTask diatur atau tidak. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Mengatur nilai yang menunjukkan apakah SplitsInProgressTasks diatur atau tidak. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Mengatur nilai yang menunjukkan apakah SpreadActualCost diatur atau tidak. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Mengatur nilai yang menunjukkan apakah SpreadPercentComplete diatur atau tidak. |
| [set_StartDate](./set_startdate/) | Mengatur nilai StartDate. |
| [set_StatusDate](./set_statusdate/) | Mengatur nilai StatusDate. |
| [set_Subject](./set_subject/) | Mengatur nilai Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Mengatur nilai yang menunjukkan apakah TaskUpdatesResource diatur atau tidak. |
| [set_Template](./set_template/) | Mengatur nilai Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Mengatur nilai TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Mengatur nilai TimescaleStart. |
| [set_Title](./set_title/) | Mengatur nilai Title. |
| [set_Uid](./set_uid/) | Mengatur nilai Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Mengatur nilai yang menunjukkan apakah UpdateManuallyScheduledTasksWhenEditingLinks diatur atau tidak. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Mengatur Definisi Kode WBS untuk proyek. |
| [set_WeekStartDay](./set_weekstartday/) | Mengatur nilai WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Mengatur nilai WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Mengatur waktu penyimpanan baseline. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk seluruh proyek. |

