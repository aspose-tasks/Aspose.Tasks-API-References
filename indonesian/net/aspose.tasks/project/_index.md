---
title: "Kelas Project"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Project. Mewakili sebuah proyek"
type: docs
weight: 1440
url: /id/net/aspose.tasks/project/
---
## Project class

Mewakili sebuah proyek.

```csharp
public class Project
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Project](project/#constructor)() | Menginisialisasi instance baru dari kelas `Project`. |
| [Project](project/#constructor_1)(DbSettings) | Menginisialisasi instance baru dari kelas `Project` untuk membaca data dari basis data yang ditentukan oleh instance dari kelas [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/). |
| [Project](project/#constructor_2)(Stream) | Menginisialisasi instance baru dari kelas `Project` dari sebuah stream. |
| [Project](project/#constructor_7)(StreamReader) | Menginisialisasi instance baru dari kelas `Project` dari sebuah instance StreamReader. |
| [Project](project/#constructor_8)(string) | Menginisialisasi instance baru dari kelas `Project` dari templat (file mpp atau mpt yang ada). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Menginisialisasi instance baru dari kelas `Project` dari Stream dengan instance [`LoadOptions`](../loadoptions/) yang ditentukan. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Menginisialisasi instance baru dari kelas `Project` dari templat (file mpp atau mpt yang ada). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Menginisialisasi instance baru dari kelas `Project` dari Stream dengan instance [`PrimaveraReadOptions`](../primaverareadoptions/) yang ditentukan. |
| [Project](project/#constructor_6)(Stream, string) | Menginisialisasi instance baru dari kelas `Project` dari templat (file mpp atau mpt yang ada). |
| [Project](project/#constructor_9)(string, LoadOptions) | Menginisialisasi instance baru dari kelas `Project` dari templat (file mpp atau mpt yang ada) dengan instance [`LoadOptions`](../loadoptions/) yang ditentukan. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Menginisialisasi instance baru dari kelas `Project` dari templat (file mpp atau mpt yang ada). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Menginisialisasi instance baru dari kelas `Project` dari templat (file MPP atau MPT yang ada) dengan instance [`PrimaveraReadOptions`](../primaverareadoptions/) yang ditentukan. |
| [Project](project/#constructor_12)(string, string) | Menginisialisasi instance baru dari kelas `Project` dari templat yang dilindungi kata sandi (file mpp atau mpt yang ada). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Menampilkan atau mengatur nilai yang menunjukkan apakah ActualsInSync diatur atau tidak. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Menampilkan atau mengatur nilai yang menunjukkan apakah AdminProject diatur atau tidak. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Menampilkan atau mengatur nilai yang menunjukkan apakah AreEditableActualCosts diatur atau tidak. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Menampilkan atau mengatur nilai Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Menampilkan atau mengatur nilai yang menunjukkan apakah AutoAddNewResourcesAndTasks diatur atau tidak. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Menampilkan atau mengatur apakah biaya penugasan dan biaya sisa harus dihitung otomatis menggunakan pekerjaan penugasan dan tarif sumber daya. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Menampilkan atau mengatur nilai yang menunjukkan apakah Autolink diatur atau tidak. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Menampilkan atau mengatur nilai BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Menampilkan koleksi properti bawaan proyek. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Menampilkan atau mengatur mode perhitungan proyek. Dapat berupa salah satu nilai dari enumerasi [`CalculationMode`](./calculationmode/). |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Mendapatkan atau mengatur nilai Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Menampilkan objek [`CalendarCollection`](../calendarcollection/) dari instance Project ini. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Menampilkan atau mengatur nilai Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Menampilkan atau mengatur nilai Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Menampilkan atau mengatur nilai Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Menampilkan atau mengatur nilai CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Menampilkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path proyek ini. Ini adalah operasi O(n), di mana n adalah jumlah tugas dalam proyek. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Menampilkan atau mengatur nilai CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Menampilkan atau mengatur nilai CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Menampilkan atau mengatur nilai CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Menampilkan atau mengatur nilai CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Menampilkan atau mengatur nilai CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Menampilkan atau mengatur nilai CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Menampilkan koleksi properti khusus proyek. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Mendapatkan atau mengatur nilai DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Mendapatkan atau mengatur nilai DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Mendapatkan atau mengatur nilai DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Mendapatkan atau mengatur nilai DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Mendapatkan atau mengatur nilai DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Mendapatkan atau mengatur nilai DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Mendapatkan atau mengatur nilai DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Mendapatkan atau mengatur nilai DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Mendapatkan atau mengatur nilai DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Mendapatkan atau mengatur tampilan default proyek. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Mendapatkan instance dari kelas [`WeekDayCollection`](../weekdaycollection/) yang mewakili koleksi hari kerja minggu default proyek dan waktu kerja. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Mendapatkan sebuah instance dari kelas [`ProjectDisplayOptions`](../projectdisplayoptions/). |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Mendapatkan atau mengatur nilai DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Mendapatkan atau mengatur nilai EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Mendapatkan objek ExtendedAttributeDefinitionCollection. Koleksi definisi atribut tambahan (field khusus) yang terkait dengan sebuah proyek. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Mendapatkan atau mengatur nilai ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Mendapatkan atau mengatur nilai FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah FiscalYearStart diatur atau tidak. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Mendapatkan atau mengatur nilai FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Mendapatkan atau mengatur pengaturan globalisasi (spesifik bahasa) proyek. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Mendapatkan atau mengatur nilai Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah HonorConstraints diatur atau tidak. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Mendapatkan atau mengatur nilai HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah InsertedProjectsLikeSummary diatur atau tidak. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled diatur atau tidak. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Mendapatkan atau mengatur nilai Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Mendapatkan atau mengatur nilai LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Mendapatkan atau mengatur nilai LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Mendapatkan atau mengatur nilai LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Mendapatkan atau mengatur nilai Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MicrosoftProjectServerURL diatur atau tidak. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Mendapatkan atau mengatur nilai MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Mendapatkan atau mengatur nilai MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MoveCompletedEndsBack diatur atau tidak. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MoveCompletedEndsForward diatur atau tidak. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MoveRemainingStartsBack diatur atau tidak. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MoveRemainingStartsForward diatur atau tidak. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah MultipleCriticalPaths diatur atau tidak. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Mendapatkan atau mengatur nilai Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah NewTasksAreManual diatur atau tidak. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah NewTasksEffortDriven diatur atau tidak. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah NewTasksEstimated diatur atau tidak. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Mendapatkan atau mengatur nilai NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Mendapatkan koleksi yang berisi instance kelas [`OleObject`](../oleobject/) yang terhubung atau disematkan ke file proyek ini. Hanya tersedia untuk format file mpp. Koleksi ini bersifat read-only kecuali untuk operasi 'Clear'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Mendapatkan objek OutlineCodeDefinitionCollection. Koleksi definisi kode outline yang terkait dengan sebuah proyek. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Mendapatkan objek yang berisi properti khusus Primavera untuk sebuah proyek yang dibaca dari file Primavera. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah ProjectExternallyEdited diatur atau tidak. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah RemoveFileProperties diatur atau tidak. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Mendapatkan objek ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Mendapatkan semua definisi filter berbasis sumber daya. ResourceFilters adalah koleksi objek [`Filter`](../filter/). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Mendapatkan semua definisi grup berbasis sumber daya. ResourceGroups adalah koleksi objek [`Group`](../group/). |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Mendapatkan objek ResourceCollection. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Mendapatkan atau mengatur nilai Revision. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Mendapatkan akar dari pohon tugas. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Mendapatkan atau mengatur nilai SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah ScheduleFromStart diatur atau tidak. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah ShowProjectSummaryTask diatur atau tidak. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah SplitsInProgressTasks diatur atau tidak. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah SpreadActualCost diatur atau tidak. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah SpreadPercentComplete diatur atau tidak. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Mendapatkan atau mengatur nilai StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Mendapatkan atau mengatur nilai StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Mendapatkan atau mengatur nilai Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Mendapatkan daftar objek [`Table`](../table/). |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Mendapatkan semua definisi filter berbasis tugas. TaskFilters adalah koleksi objek [`Filter`](../filter/). |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Mendapatkan semua definisi grup berbasis tugas. TaskGroups adalah koleksi objek [`Group`](../group/). |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Mendapatkan objek [`TaskLinkCollection`](../tasklinkcollection/). |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah TaskUpdatesResource diatur atau tidak. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Mendapatkan atau mengatur nilai Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Mendapatkan atau mengatur nilai TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Mendapatkan atau mengatur nilai TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Mendapatkan atau mengatur nilai Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Mendapatkan atau mengatur nilai dari Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah UpdateManuallyScheduledTasksWhenEditingLinks diatur atau tidak. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Mendapatkan sebuah instance kelas [`VbaProject`](./vbaproject/). |
| [Views](../../aspose.tasks/project/views/) { get; } | Mendapatkan daftar objek [`View`](../view/). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Mendapatkan atau mengatur Definisi Kode WBS untuk proyek. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Mendapatkan atau mengatur nilai WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Mendapatkan atau mengatur nilai WorkFormat. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Menyalin data utama dan properti proyek ke proyek lain. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Menyalin data utama dan properti proyek ke proyek lain. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Menumerasi semua tugas proyek secara rekursif termasuk tugas root. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Mengembalikan waktu penyimpanan baseline. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Mendapatkan objek [`Duration`](../duration/) dengan jumlah unit yang ditentukan dan format durasi default yang didefinisikan dalam pengaturan proyek [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Mendapatkan objek [`Duration`](../duration/) dengan jumlah unit [`TimeUnitType`](../timeunittype/) yang ditentukan. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Mendapatkan objek [`Duration`](../duration/) dengan nilai TimeSpan yang ditentukan dan nilai [`TimeUnitType`](../timeunittype/) yang ditentukan. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/) default (Hari). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/) default (Hari) dan [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) yang diberikan. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/) yang diberikan. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/) dan [`PageSize`](../../aspose.tasks.visualization/pagesize/) yang diberikan. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/) dan [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) yang diberikan. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) dan rentang tanggal. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Mengembalikan koleksi tautan tugas yang merupakan pendahulu tugas yang ditentukan. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Mendapatkan objek [`Duration`](../duration/) dengan nilai Double yang ditentukan dan format kerja default. |
| [Print](../../aspose.tasks/project/print/#print)() | Mencetak proyek ke printer default dengan pengaturan printer default menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Mencetak proyek ke printer default dengan pengaturan printer default dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Mencetak proyek ke printer yang ditentukan dengan pengaturan printer default menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Mencetak proyek sesuai dengan pengaturan printer yang ditentukan, opsi penyimpanan khusus, dan nama dokumen yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna). |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan bidang biaya. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan bidang biaya dengan validasi opsional. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Menghitung ulang Id, Start, dan Finish sumber daya. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Menghapus penugasan sumber daya yang tidak valid dari daftar penugasan sumber daya proyek. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Menomori ulang kode WBS semua tugas. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Menomori ulang kode WBS tugas yang telah selesai. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Menjadwalkan ulang pekerjaan proyek yang belum selesai untuk mulai setelah tanggal yang ditentukan. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Menjadwalkan ulang pekerjaan yang belum selesai untuk daftar tugas tertentu agar mulai setelah tanggal yang ditentukan. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Menyimpan data proyek ke file dalam format mpp. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Menyimpan data proyek ke aliran. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Menyimpan proyek ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Menyimpan data proyek ke file. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Menyimpan dokumen ke file menggunakan opsi penyimpanan yang ditentukan. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Menyimpan proyek sebagai templat ke aliran yang ditentukan. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Menyimpan proyek sebagai templat ke jalur file yang ditentukan. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Menyimpan proyek sebagai templat ke aliran yang ditentukan. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Menyimpan proyek sebagai templat. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Menyimpan laporan ikhtisar proyek ke aliran. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Menyimpan laporan ikhtisar proyek ke file PDF. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Menyimpan laporan proyek tipe yang ditentukan ke aliran yang ditentukan. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Menyimpan laporan proyek tipe yang ditentukan dalam format PDF ke jalur file yang ditentukan. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Mengumpulkan secara rekursif semua tugas anak dari tugas akar. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Menyimpan bidang baseline ke baseline yang ditentukan untuk seluruh proyek. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Menyimpan bidang baseline ke baseline yang ditentukan untuk tugas yang dipilih. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Mengatur waktu penyimpanan baseline. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk seluruh proyek. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk daftar tugas yang ditentukan. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Mengambil info file proyek dari aliran. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Membaca info file proyek dari file. |

## Catatan

**Project** adalah kelas pusat dalam pustaka Aspose.Tasks.

Seseorang dapat menggunakan **Project** untuk membaca salah satu format manajemen proyek yang didukung: MPP, MPT, MPX, XML.

Untuk memuat dokumen yang ada dalam salah satu format yang didukung, berikan nama file atau aliran ke salah satu konstruktor **Project**. Untuk membuat proyek kosong, panggil konstruktor tanpa parameter.

Gunakan salah satu overload metode Save untuk menyimpan proyek dalam salah satu format [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Gambar: JPEG, PNG, BMP, TIFF, SVG; Teks: TXT; Lainnya: HTML.

**Project** menyimpan informasi seluruh proyek seperti [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), dan [`ExtendedAttributes`](./extendedattributes/). Sebagian besar objek ini dapat diakses melalui properti yang sesuai dari kelas **Project**.

**Project** adalah entitas akar yang berisi titik masuk untuk memanipulasi entitas proyek lainnya, seperti [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) dan [`Calendar`](../calendar/).

Entitas **Project** dapat diakses melalui koleksi bertipe, misalnya [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), dll.

## Contoh

Menampilkan cara bekerja dengan instance &lt;see cref=\"Aspose.Tasks.Project\"/&gt;.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// menambahkan tugas baru dan mengatur properti yang diinginkan
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// menambahkan sumber daya baru
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// menambahkan penugasan sumber daya baru
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// simpan proyek dalam salah satu format yang tersedia
// di sini kami menyimpannya dalam format file Microsoft Project XML.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


