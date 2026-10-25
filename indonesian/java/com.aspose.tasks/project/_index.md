---
title: "Project"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili sebuah proyek."
type: docs
weight: 220
url: /id/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Mewakili sebuah proyek.

--------------------

**Project** adalah kelas pusat dalam pustaka Aspose.Tasks.

Seseorang dapat menggunakan **Project** untuk membaca salah satu format manajemen proyek yang didukung: MPP, MPT, MPX, XML.

Untuk memuat dokumen yang ada dalam salah satu format yang didukung, berikan nama file atau aliran ke salah satu konstruktor **Project**. Untuk membuat proyek kosong, panggil konstruktor tanpa parameter.

Gunakan salah satu overload metode Save untuk menyimpan proyek dalam salah satu format [SaveFileFormat](../../com.aspose.tasks/savefileformat): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Gambar: JPEG, PNG, BMP, TIFF, SVG; Teks: TXT; Lainnya: HTML.

Untuk mencetak proyek, gunakan salah satu overload metode [print()](../../com.aspose.tasks/project\#print--).

**Project** menyimpan informasi seluruh proyek seperti `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), dan `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). Sebagian besar objek ini dapat diakses melalui properti yang sesuai dari kelas **Project**.

**Project** adalah entitas akar yang berisi titik masuk untuk memanipulasi entitas proyek lainnya, seperti [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) dan [Calendar](../../com.aspose.tasks/calendar).

**Project** entitas dapat diakses melalui koleksi bertipe, misalnya `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), dll.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Project()](#Project--) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat yang dilindungi kata sandi (file mpp atau mpt yang ada). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file mpp atau mpt yang ada). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) dari Stream dengan instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file mpp atau mpt yang ada). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) dari sebuah stream. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file MPP atau MPT yang ada) dengan instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) untuk membaca data dari basis data yang ditentukan oleh instance dari kelas [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada) dengan instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari Stream dengan instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Menyalin data utama dan properti proyek ke proyek lain. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Menyalin data utama dan properti proyek ke proyek lain. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Mengeumerasi secara rekursif semua tugas proyek termasuk tugas root. |
| [getActualsInSync()](#getActualsInSync--) | Mendapatkan nilai yang menunjukkan apakah ActualsInSync diatur atau tidak. |
| [getAdminProject()](#getAdminProject--) | Mendapatkan nilai yang menunjukkan apakah AdminProject diatur atau tidak. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Mendapatkan nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak. |
| [getAuthor()](#getAuthor--) | Mendapatkan nilai Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Mendapatkan nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Mendapatkan apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya. |
| [getAutolink()](#getAutolink--) | Mendapatkan nilai yang menunjukkan apakah Autolink diatur atau tidak. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Mendapatkan nilai BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Mengembalikan waktu penyimpanan baseline. |
| [getBuiltInProps()](#getBuiltInProps--) | Mendapatkan koleksi properti bawaan proyek. |
| [getCalculationMode()](#getCalculationMode--) | Mendapatkan mode perhitungan proyek. |
| [getCalendar()](#getCalendar--) | Memperoleh nilai Calendar. |
| [getCalendars()](#getCalendars--) | Mendapatkan objek [CalendarCollection](../../com.aspose.tasks/calendarcollection) dari instance Project ini. |
| [getCategory()](#getCategory--) | Mendapatkan nilai Category. |
| [getComments()](#getComments--) | Mendapatkan nilai Comments. |
| [getCompany()](#getCompany--) | Mendapatkan nilai Company. |
| [getCreationDate()](#getCreationDate--) | Mendapatkan nilai CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | Mendapatkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path proyek ini. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini. |
| [getCurrencyCode()](#getCurrencyCode--) | Mendapatkan nilai CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Mendapatkan nilai CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Mendapatkan nilai CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Mendapatkan nilai CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Mendapatkan nilai CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Mendapatkan nilai CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Mendapatkan koleksi properti khusus proyek. |
| [getDateFormat()](#getDateFormat--) | Mendapatkan nilai DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Mendapatkan nilai DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Mendapatkan nilai DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Mendapatkan nilai DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Mendapatkan nilai DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Mendapatkan nilai DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Mendapatkan nilai DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Mendapatkan nilai DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Mendapatkan nilai DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Mendapatkan tampilan default proyek. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Mendapatkan instance kelas [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) yang mewakili koleksi hari kerja minggu default proyek dan jam kerja. |
| [getDisplayOptions()](#getDisplayOptions--) | Mendapatkan sebuah instance dari kelas [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Mendapatkan objek [Duration](../../com.aspose.tasks/duration) dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Mendapatkan objek [Duration](../../com.aspose.tasks/duration) dengan jumlah unit [TimeUnitType](../../com.aspose.tasks/timeunittype) yang ditentukan. |
| [getDurationFormat()](#getDurationFormat--) | Mendapatkan nilai DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Mendapatkan nilai EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Mendapatkan objek ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Mendapatkan nilai ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Mendapatkan nilai FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Mendapatkan nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak. |
| [getFyStartDate()](#getFyStartDate--) | Mendapatkan nilai FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Mendapatkan pengaturan globalisasi (spesifik bahasa) proyek. |
| [getGuid()](#getGuid--) | Mendapatkan nilai Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Mendapatkan nilai yang menunjukkan apakah HonorConstraints diatur atau tidak. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Mendapatkan nilai HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Mendapatkan nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Mendapatkan nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak. |
| [getKeywords()](#getKeywords--) | Mendapatkan nilai Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Mendapatkan nilai LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Mendapatkan nilai LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Mendapatkan nilai LastSaved. |
| [getManager()](#getManager--) | Mendapatkan nilai Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Mendapatkan nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Mendapatkan nilai MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Mendapatkan nilai MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Mendapatkan nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak. |
| [getName()](#getName--) | Mendapatkan nilai Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Mendapatkan nilai NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Mendapatkan nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Mendapatkan nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Mendapatkan nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak. |
| [getOleObjects()](#getOleObjects--) | Mendapatkan koleksi yang berisi instance kelas [OleObject](../../com.aspose.tasks/oleobject) yang ditautkan atau disematkan ke file proyek ini. |
| [getOutlineCodes()](#getOutlineCodes--) | Mendapatkan objek OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) default (Hari). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [SaveOptions](../../com.aspose.tasks/saveoptions) yang diberikan. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) dan [PresentationFormat](../../com.aspose.tasks/presentationformat) yang diberikan. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) dan [PageSize](../../com.aspose.tasks/pagesize) yang diberikan. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) dan rentang tanggal yang diberikan. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) default (Hari) dan [PresentationFormat](../../com.aspose.tasks/presentationformat) yang diberikan. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) yang diberikan. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Mengembalikan koleksi tautan tugas yang merupakan pendahulu dari tugas yang ditentukan. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Mendapatkan objek yang berisi properti khusus Primavera untuk proyek yang dibaca dari file Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Mendapatkan nilai yang menunjukkan apakah ProjectExternallyEdited diatur atau tidak. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Mendapatkan info file proyek dari aliran. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Membaca info file proyek dari file. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Mendapatkan nilai yang menunjukkan apakah RemoveFileProperties diatur atau tidak. |
| [getResourceAssignments()](#getResourceAssignments--) | Mendapatkan objek ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | Mendapatkan semua definisi filter berbasis sumber daya. |
| [getResourceGroups()](#getResourceGroups--) | Mendapatkan semua definisi grup berbasis sumber daya. |
| [getResources()](#getResources--) | Mendapatkan objek ResourceCollection. |
| [getRevision()](#getRevision--) | Mendapatkan nilai Revision. |
| [getRootTask()](#getRootTask--) | Mendapatkan akar pohon tugas. |
| [getSaveVersion()](#getSaveVersion--) | Mendapatkan nilai SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Mendapatkan nilai yang menunjukkan apakah ScheduleFromStart diatur atau tidak. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Mendapatkan nilai yang menunjukkan apakah ShowProjectSummaryTask diatur atau tidak. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Mendapatkan nilai yang menunjukkan apakah SplitsInProgressTasks diatur atau tidak. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Mendapatkan nilai yang menunjukkan apakah SpreadActualCost diatur atau tidak. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Mendapatkan nilai yang menunjukkan apakah SpreadPercentComplete telah diatur atau tidak. |
| [getStartDate()](#getStartDate--) | Mendapatkan nilai StartDate. |
| [getStatusDate()](#getStatusDate--) | Mendapatkan nilai StatusDate. |
| [getSubject()](#getSubject--) | Mendapatkan nilai Subject. |
| [getTables()](#getTables--) | Mendapatkan daftar objek [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | Mendapatkan semua definisi filter berbasis tugas. |
| [getTaskGroups()](#getTaskGroups--) | Mendapatkan semua definisi grup berbasis tugas. |
| [getTaskLinks()](#getTaskLinks--) | Mendapatkan objek [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Mendapatkan nilai yang menunjukkan apakah TaskUpdatesResource telah diatur atau tidak. |
| [getTemplate()](#getTemplate--) | Mendapatkan nilai Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Mendapatkan nilai TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Mendapatkan nilai TimescaleStart. |
| [getTitle()](#getTitle--) | Mendapatkan nilai Title. |
| [getUid()](#getUid--) | Mendapatkan nilai Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Mendapatkan nilai yang menunjukkan apakah UpdateManuallyScheduledTasksWhenEditingLinks telah diatur atau tidak. |
| [getVbaProject()](#getVbaProject--) | Mendapatkan sebuah instance kelas `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | Mendapatkan daftar objek [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Mendapatkan Definisi Kode WBS untuk proyek. |
| [getWeekStartDay()](#getWeekStartDay--) | Mendapatkan nilai WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Mendapatkan objek [Duration](../../com.aspose.tasks/duration) dengan nilai `double` yang ditentukan dan format kerja default. |
| [getWorkFormat()](#getWorkFormat--) | Mendapatkan nilai WorkFormat. |
| [print()](#print--) | Mencetak proyek ke printer default dengan pengaturan printer default menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Mencetak proyek ke printer default dengan pengaturan printer default dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan, opsi penyimpanan khusus, dan nama dokumen yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [print(String printerName)](#print-java.lang.String-) | Mencetak proyek ke printer yang ditentukan dengan pengaturan printer default menggunakan pengontrol cetak standar (tanpa Antarmuka Pengguna). |
| [recalculate()](#recalculate--) | Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, menetapkan tanggal awal/akhir, menghitung kelonggaran, pekerjaan, dan bidang biaya. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, menetapkan tanggal awal/akhir, menghitung kelonggaran, pekerjaan, dan bidang biaya dengan validasi opsional. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Menghitung ulang ID, Mulai, dan Selesai sumber daya. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Menghitung ulang Mulai dan Selesai sumber daya. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Menghilangkan penugasan sumber daya yang tidak valid dari daftar penugasan sumber daya proyek. |
| [renumberWBSCode()](#renumberWBSCode--) | Menomori ulang kode WBS semua tugas. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Menomori ulang kode WBS tugas yang dilewati. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Menjadwalkan ulang pekerjaan proyek yang belum selesai untuk mulai setelah tanggal tertentu. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Menjadwalkan ulang pekerjaan yang belum selesai untuk daftar tugas tertentu agar mulai setelah tanggal tertentu. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Menyimpan proyek ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Menyimpan data proyek ke aliran. |
| [save(String filename)](#save-java.lang.String-) | Menyimpan data proyek ke file dalam format mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Menyimpan dokumen ke file menggunakan opsi penyimpanan yang ditentukan. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Menyimpan data proyek ke file. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Menyimpan proyek sebagai templat ke aliran yang ditentukan. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Menyimpan proyek sebagai templat ke aliran yang ditentukan. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Menyimpan proyek sebagai templat ke jalur file yang ditentukan. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Menyimpan proyek sebagai templat. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Menyimpan laporan ikhtisar proyek ke aliran. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Menyimpan laporan proyek tipe yang ditentukan ke aliran yang ditentukan. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Menyimpan laporan ikhtisar proyek ke file PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Menyimpan laporan proyek tipe yang ditentukan dalam format PDF ke jalur file yang ditentukan. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Mengumpulkan secara rekursif semua tugas anak dari tugas akar. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Menetapkan nilai yang menunjukkan apakah ActualsInSync diatur atau tidak. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Menetapkan nilai yang menunjukkan apakah AdminProject diatur atau tidak. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Mengatur nilai Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Mengatur apakah biaya penugasan dan biaya yang tersisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah Autolink diatur atau tidak. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Menyimpan bidang baseline ke baseline yang ditentukan untuk tugas yang dipilih. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Mengatur nilai BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Mengatur waktu penyimpanan baseline. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Mengatur mode perhitungan sebuah proyek. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Mengatur nilai Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Mengatur nilai Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Mengatur nilai Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Mengatur nilai Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Mengatur nilai CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Mengatur nilai CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Mengatur nilai CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Mengatur nilai CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Mengatur nilai CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Mengatur nilai CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Mengatur nilai CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Mengatur nilai DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Mengatur nilai DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Mengatur nilai DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Mengatur nilai DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Mengatur nilai DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Mengatur nilai DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Mengatur nilai DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Mengatur nilai DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Mengatur nilai DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Mengatur tampilan default proyek. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Mengatur nilai DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Mengatur nilai EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Mengatur nilai ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Mengatur nilai FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Mengatur nilai FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Mengatur pengaturan globalisasi (spesifik bahasa) proyek. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Mengatur nilai Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah HonorConstraints diatur atau tidak. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Mengatur nilai HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Mengatur nilai Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Mengatur nilai LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Mengatur nilai LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Mengatur nilai LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Mengatur nilai Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Mengatur nilai MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Mengatur nilai MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nilai Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Mengatur nilai NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah ProjectExternallyEdited diatur atau tidak. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah RemoveFileProperties diatur atau tidak. |
| [setRevision(int value)](#setRevision-int-) | Mengatur nilai Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Mengatur nilai SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah ScheduleFromStart diatur atau tidak. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Mengatur nilai yang menunjukkan apakah ShowProjectSummaryTask diatur atau tidak. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah SplitsInProgressTasks diatur atau tidak. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah SpreadActualCost diatur atau tidak. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah SpreadPercentComplete diatur atau tidak. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Mengatur nilai StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Mengatur nilai StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Mengatur nilai Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah TaskUpdatesResource diatur atau tidak. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Mengatur nilai Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Mengatur nilai TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Mengatur nilai TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Mengatur nilai Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Mengatur nilai dari Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah UpdateManuallyScheduledTasksWhenEditingLinks diatur atau tidak. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Menetapkan Definisi Kode WBS untuk proyek. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Menetapkan nilai WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Menetapkan nilai WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Memperbarui semua pekerjaan menjadi selesai hingga tanggal tertentu untuk seluruh proyek. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Memperbarui semua pekerjaan menjadi selesai hingga tanggal tertentu untuk daftar tugas yang ditentukan. |
### Project() {#Project--}
```
public Project()
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat yang dilindungi kata sandi (file mpp atau mpt yang ada).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | java.lang.String | Jalur ke templat untuk membuat proyek dari. |
|  | protectionPassword | java.lang.String | Kata sandi perlindungan. |

--------------------

Membaca file yang dilindungi kata sandi saat ini hanya didukung untuk format file MSP 2003. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file mpp atau mpt yang ada).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | java.lang.String | Jalur ke templat untuk membuat proyek dari. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) dari Stream dengan instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran dari Proyek java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)class yang memungkinkan menyesuaikan pembacaan format Primavera (XER atau XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file mpp atau mpt yang ada).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | java.lang.String | Jalur ke templat untuk membuat proyek dari. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | metode callback yang ditentukan untuk menangani kesalahan parsing xml. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) dari sebuah stream.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream untuk memuat templat dari. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Menginisialisasi instance baru dari kelas [Project](../../com.aspose.tasks/project) menggunakan templat (file MPP atau MPT yang ada) dengan instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | java.lang.String | Jalur ke templat untuk membuat proyek dari |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | instance yang ditentukan dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) untuk membaca data dari basis data yang ditentukan oleh instance dari kelas [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | instance yang ditentukan dari kelas [DbSettings](../../com.aspose.tasks/dbsettings) class. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream untuk memuat templat dari. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | metode callback yang ditentukan untuk menangani kesalahan parsing xml. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream untuk memuat templat dari. |
|  | protectionPassword | java.lang.String | Kata sandi perlindungan. |

--------------------

Membaca file yang dilindungi kata sandi saat ini hanya didukung untuk format file MSP 2003. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari templat (file mpp atau mpt yang ada) dengan instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectTemplate | java.lang.String | Jalur ke templat untuk membuat proyek dari |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions) class. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Menginisialisasi sebuah instance baru dari kelas [Project](../../com.aspose.tasks/project) dari Stream dengan instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran dari Proyek java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | instance yang ditentukan dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Prj](../../com.aspose.tasks/prj) untuk mendapatkan kunci properti. |

**Returns:**
T - nilai yang dipetakan ke properti ini dalam kontainer ini.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Prj](../../com.aspose.tasks/prj) untuk mendapatkan kunci properti. |
| val | T | nilai. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Menyalin data utama dan properti proyek ke proyek lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Proyek lain untuk menyalin data ke. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Menyalin data utama dan properti proyek ke proyek lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Proyek lain untuk menyalin data ke. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Opsi salin untuk mengontrol proses penyalinan. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Mengeumerasi secara rekursif semua tugas proyek termasuk tugas root.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable yang dapat digunakan untuk mengiterasi semua tugas proyek.

--------------------

Menyediakan cara yang lebih ringan untuk mengiterasi tugas dibandingkan metode [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) karena tidak mengalokasikan memori untuk semua tugas.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Mendapatkan nilai yang menunjukkan apakah ActualsInSync diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Mendapatkan nilai yang menunjukkan apakah AdminProject diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Mendapatkan nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Mendapatkan nilai Author.

**Returns:**
java.lang.String - nilai dari Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Mendapatkan nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Mendapatkan apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya.

**Returns:**
boolean - apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Mendapatkan nilai yang menunjukkan apakah Autolink diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Mendapatkan nilai BaselineForEarnedValue.

**Returns:**
int - nilai dari BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Mengembalikan waktu penyimpanan baseline. Mengembalikan DateTime.MinValue (00:00:00.0000000 UTC, 1 Januari 0001) jika baseline tidak disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| baselineNumber | int | Nomor baseline [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - Tanggal dan waktu penyimpanan terakhir baseline.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Mendapatkan koleksi properti bawaan proyek.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Mendapatkan mode perhitungan sebuah proyek. Dapat berupa salah satu nilai dari enumerasi `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - mode perhitungan sebuah proyek.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Memperoleh nilai Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Mendapatkan objek [CalendarCollection](../../com.aspose.tasks/calendarcollection) dari instance Project ini.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Mendapatkan nilai Category.

**Returns:**
java.lang.String - nilai dari Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Mendapatkan nilai Comments.

**Returns:**
java.lang.String - nilai dari Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Mendapatkan nilai Company.

**Returns:**
java.lang.String - nilai dari Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Mendapatkan nilai CreationDate.

**Returns:**
java.util.Date - nilai dari CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Mendapatkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path proyek ini.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Ini adalah operasi O(n), di mana n adalah jumlah tugas dalam proyek.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini.

**Returns:**
int - nilai maksimum total slack time (dalam hari) di mana sebuah tugas dianggap kritis
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Mendapatkan nilai CurrencyCode.

**Returns:**
java.lang.String - nilai dari CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Mendapatkan nilai CurrencyDigits.

**Returns:**
int - nilai dari CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Mendapatkan nilai CurrencySymbol.

**Returns:**
java.lang.String - nilai dari CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Mendapatkan nilai CurrencySymbolPosition.

**Returns:**
int - nilai dari CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Mendapatkan nilai CurrentDate.

**Returns:**
java.util.Date - nilai dari CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Mendapatkan nilai CustomDateFormat.

**Returns:**
java.lang.String - nilai dari CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Mendapatkan koleksi properti khusus proyek.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Mendapatkan nilai DateFormat.

**Returns:**
int - nilai dari DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Mendapatkan nilai DaysPerMonth.

**Returns:**
int - nilai dari DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Mendapatkan nilai DefaultFinishTime.

**Returns:**
java.util.Date - nilai dari DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Mendapatkan nilai DefaultFixedCostAccrual.

**Returns:**
int - nilai dari DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Mendapatkan nilai DefaultOvertimeRate.

**Returns:**
double - nilai dari DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Mendapatkan nilai DefaultStandardRate.

**Returns:**
double - nilai dari DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Mendapatkan nilai DefaultStartTime.

**Returns:**
java.util.Date - nilai dari DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Mendapatkan nilai DefaultTaskEVMethod.

**Returns:**
int - nilai dari DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Mendapatkan nilai DefaultTaskType.

**Returns:**
int - nilai dari DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Mendapatkan tampilan default proyek.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Mendapatkan instance kelas [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) yang mewakili koleksi hari kerja minggu default proyek dan jam kerja.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Data hanya terdapat dalam file mpp (bukan dalam xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Mendapatkan sebuah instance dari kelas [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Mendapatkan objek [Duration](../../com.aspose.tasks/duration) dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | val | double | jumlah unit yang ditentukan. |

--------------------

Metode ini harus digunakan dengan hati-hati karena mengembalikan durasi yang berbeda tergantung pada pengaturan Project.DurationFormat. Misalnya, GetWork(1.0) akan mengembalikan 1 jam ketika Project.DurationFormat adalah TimeUnitType.Hour atau 1 hari jika Project.DurationFormat adalah TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Mendapatkan objek [Duration](../../com.aspose.tasks/duration) dengan jumlah unit [TimeUnitType](../../com.aspose.tasks/timeunittype) yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | double | jumlah unit yang ditentukan. |
| timeUnit | byte | nilai TimeUnitType yang ditentukan. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Mendapatkan nilai DurationFormat.

**Returns:**
byte - nilai dari DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Mendapatkan nilai EarnedValueMethod.

**Returns:**
int - nilai dari EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Mendapatkan objek ExtendedAttributeDefinitionCollection. Koleksi definisi atribut ekstensi (field khusus) yang terkait dengan sebuah proyek.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Mendapatkan nilai ExtendedCreationDate.

**Returns:**
java.util.Date - nilai dari ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Mendapatkan nilai FinishDate.

**Returns:**
java.util.Date - nilai dari FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Mendapatkan nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Mendapatkan nilai FyStartDate.

**Returns:**
int - nilai dari FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Mendapatkan pengaturan globalisasi (spesifik bahasa) proyek.

Cara yang disarankan adalah menggunakan literal atau format yang tidak tergantung pada budaya di seluruh proyek. Namun, jika sebuah proyek menggunakan literal yang spesifik budaya, kelas ini dapat digunakan untuk membantu mesin perhitungan mengurai literal tersebut.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Mendapatkan nilai Guid.

**Returns:**
java.util.UUID - nilai dari Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Mendapatkan nilai yang menunjukkan apakah HonorConstraints diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Mendapatkan nilai HyperlinkBase.

**Returns:**
java.lang.String - nilai dari HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Mendapatkan nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Mendapatkan nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Mendapatkan nilai Keywords.

**Returns:**
java.lang.String - nilai dari Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Mendapatkan nilai LastAuthor.

**Returns:**
java.lang.String - nilai dari LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Mendapatkan nilai LastPrinted.

**Returns:**
java.util.Date - nilai dari LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Mendapatkan nilai LastSaved.

**Returns:**
java.util.Date - nilai dari LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Mendapatkan nilai Manager.

**Returns:**
java.lang.String - nilai dari Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Mendapatkan nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Mendapatkan nilai MinutesPerDay.

**Returns:**
int - nilai MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Mendapatkan nilai MinutesPerWeek.

**Returns:**
int - nilai MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Mendapatkan nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Mendapatkan nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Mendapatkan nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nilai Name.

**Returns:**
java.lang.String - sebuah nilai Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Mendapatkan nilai NewTaskStartDate.

**Returns:**
int - nilai NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Mendapatkan nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Mendapatkan nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Mendapatkan nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Mendapatkan koleksi yang berisi instance kelas [OleObject](../../com.aspose.tasks/oleobject) yang ditautkan atau disematkan ke file proyek ini.

--------------------

Hanya tersedia untuk format file mpp. Koleksi ini bersifat read-only kecuali untuk operasi 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Mendapatkan objek OutlineCodeDefinitionCollection. Koleksi definisi kode outline yang terkait dengan proyek.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [Timescale](../../com.aspose.tasks/timescale) default (Hari).

**Returns:**
int - Jumlah halaman yang akan dirender.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [SaveOptions](../../com.aspose.tasks/saveoptions) yang diberikan.

--------------------

&gt; ```
&gt; Dalam contoh ini instance HtmlSaveOptions dan jumlah halaman dalam HTML yang dihasilkan ditulis ke konsol.
&gt; ``````

  [C#]
Project project = new Project(@"test.mpp");
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

