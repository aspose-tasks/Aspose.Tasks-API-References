---
title: "Kelas Tsk"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Tsk kelas. Mewakili properti dari objek Task"
type: docs
weight: 2620
url: /id/net/aspose.tasks/tsk/
---
## Tsk class

Mewakili properti dari objek [`Task`](../task/).

```csharp
public static class Tsk
```

## Bidang

| Nama | Deskripsi |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | Mewakili bidang id aktivitas - pengidentifikasi unik sebuah tugas yang digunakan oleh Primavera. (hanya berlaku untuk proyek Primavera). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | Biaya yang dikeluarkan untuk pekerjaan yang sudah dilakukan oleh sumber daya pada tugas mereka, bersama dengan biaya lain yang tercatat terkait dengan tugas tersebut. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | Rentang waktu kerja aktual untuk sebuah tugas, berdasarkan durasi terjadwal dan pekerjaan yang tersisa saat ini atau persentase penyelesaian. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | Tanggal ketika sebuah tugas selesai. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | Biaya yang timbul untuk pekerjaan lembur yang sudah dilakukan pada tugas oleh sumber daya yang ditugaskan. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | Jumlah aktual pekerjaan lembur yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | Durasi di mana pekerjaan lembur aktual dilindungi. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | Tanggal dan waktu ketika sebuah tugas sebenarnya dimulai. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | Jumlah pekerjaan yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | Durasi di mana pekerjaan aktual dilindungi.  Pembacaan hanya didukung untuk format XML. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | Biaya yang dikeluarkan untuk pekerjaan yang sudah selesai pada sebuah tugas, hingga tanggal status proyek atau tanggal hari ini. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | Nilai kumulatif persentase penyelesaian tugas dikalikan dengan biaya baseline berjangka waktu. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | Biaya baseline berjangka waktu kumulatif hingga tanggal status atau tanggal hari ini. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | Biaya anggaran untuk sumber daya biaya anggaran. Sumber daya anggaran hanya ditugaskan ke tugas rangkuman proyek. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | Pekerjaan anggaran untuk pekerjaan anggaran dan sumber daya material. Sumber daya anggaran hanya ditugaskan ke tugas ringkasan proyek. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | Kalender tugas. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | Tanggal selesai pengiriman.  Pembacaan hanya didukung untuk format XML. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | Tanggal mulai pengiriman. Pembacaan hanya didukung untuk format XML. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | Menentukan apakah sebuah tugas memiliki pengiriman terkait atau ketergantungan pada pengiriman terkait.  Pembacaan hanya didukung untuk format XML. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | Tanggal spesifik yang terkait dengan tipe kendala. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | Menyediakan pilihan untuk tipe kendala yang dapat diterapkan untuk penjadwalan sebuah tugas. |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | Nama individu yang bertanggung jawab atas sebuah tugas. |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | Total biaya yang dijadwalkan atau diproyeksikan untuk sebuah tugas berdasarkan biaya yang sudah dikeluarkan untuk pekerjaan yang dilakukan oleh sumber daya yang ditugaskan ke tugas, serta biaya yang direncanakan untuk pekerjaan yang tersisa. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | Selisih antara biaya dasar dan total biaya untuk sebuah tugas, sumber daya, atau penugasan. |
| static readonly [Created](../../aspose.tasks/tsk/created/) | Tanggal ketika sebuah tugas dibuat. |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | Selisih antara biaya dasar dan total biaya untuk sebuah tugas. Variansi Biaya = Biaya - Biaya Dasar |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | Tanggal target yang menunjukkan kapan sebuah tugas harus diselesaikan. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | Menentukan apakah tugas harus ditampilkan sebagai tugas ringkasan. Pembacaan hanya didukung untuk format XML. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | Menentukan apakah tugas harus ditampilkan pada tampilan garis waktu. |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | Rentang total waktu kerja aktif untuk sebuah tugas sebagaimana dimasukkan atau dihitung oleh Microsoft Project berdasarkan tanggal mulai, tanggal selesai, kalender, dan faktor penjadwalan lainnya. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | Mengembalikan teks durasi tugas. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | Selisih antara durasi dasar sebuah tugas dan total durasi (perkiraan saat ini) sebuah tugas. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | Tanggal terawal yang mungkin selesai untuk sebuah tugas, berdasarkan tanggal selesai awal dari tugas pendahulu dan penerus, batasan lainnya, serta penundaan leveling apa pun. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | Tanggal terawal yang mungkin dimulai untuk sebuah tugas, berdasarkan tanggal mulai awal dari tugas pendahulu dan penerus serta batasan lainnya. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | Menentukan apakah bidang % Selesai atau % Selesai Fisik yang harus digunakan untuk menghitung biaya anggaran kerja yang dilakukan (BCWP). |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | Jika sebuah tugas adalah tugas eksternal, ia berisi Id eksternal tugas tersebut. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | Lokasi sumber dan pengidentifikasi tugas dari tugas eksternal. |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | Berisi pengidentifikasi unik tugas eksternal ketika tugas tersebut bersifat eksternal. |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | Tanggal selesai yang dijadwalkan untuk sebuah tugas. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | Durasi antara tanggal Selesai Awal dan Selesai Akhir. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | Mengembalikan teks selesai tugas. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | Waktu yang mewakili selisih antara tanggal selesai dasar sebuah tugas atau penugasan dan tanggal selesai saat ini. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | Menampilkan biaya tugas non-sumber daya apa pun. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | Menentukan pilihan tentang bagaimana dan kapan biaya tetap harus dibebankan, atau diakumulasi, ke biaya sebuah tugas. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | Waktu yang dapat ditunda sebuah tugas tanpa menunda tugas penerus apa pun. |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | Kode identifikasi unik yang dihasilkan untuk sebuah tugas. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | Menunjukkan apakah tugas memiliki sumber daya yang ditugaskan yang memiliki pekerjaan lebih pada tugas yang ditugaskan daripada yang dapat diselesaikan dalam kapasitas kerja normal. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | Menentukan apakah bar Gantt dari sebuah tugas disembunyikan saat ditampilkan di Microsoft Project. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | Judul atau teks penjelasan untuk hyperlink yang terkait dengan sebuah tugas. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | Alamat untuk hyperlink yang terkait dengan sebuah tugas. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | Lokasi spesifik dalam dokumen pada tautan yang terkait dengan tugas. |
| static readonly [Id](../../aspose.tasks/tsk/id/) | Pengidentifikasi posisi sebuah tugas dalam daftar tugas. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | Menentukan apakah penjadwalan tugas mempertimbangkan kalender sumber daya yang ditugaskan ke tugas tersebut. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | Menunjukkan apakah harus menyembunyikan indikator peringatan konflik jadwal di Microsoft Project. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | Menentukan apakah sebuah tugas aktif. Tugas tidak aktif tidak lagi memengaruhi tugas lain atau jadwal Proyek secara keseluruhan. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | Menentukan apakah sebuah tugas berada pada jalur kritis. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | Menentukan apakah penjadwalan tugas menggunakan penjadwalan berbasis upaya. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | Menentukan apakah sebuah tugas diperkirakan. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | Menentukan apakah tugas ringkasan diperluas atau tidak dalam tampilan GanttChart. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | Menentukan apakah sebuah tugas eksternal. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | Menentukan apakah sebuah tugas dijadwalkan secara manual. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | Menampilkan apakah sebuah tugas ditandai untuk tindakan lanjutan atau identifikasi jenis tertentu. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | Menentukan apakah sebuah tugas merupakan tonggak. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | Menentukan apakah sebuah tugas adalah tugas null. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | Menunjukkan apakah salah satu sumber daya yang ditugaskan pada sebuah tugas memiliki pekerjaan lebih pada tugas tersebut daripada yang dapat dilakukan dalam kapasitas kerja normal. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | Menentukan apakah tugas saat ini harus dipublikasikan ke Project Server bersama dengan seluruh proyek. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | Menentukan apakah sebuah tugas merupakan bagian dari serangkaian tugas berulang. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | Menentukan apakah sebuah tugas dapat dilanjutkan. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | Menentukan apakah informasi tentang bar Gantt subtugas akan digabungkan ke bar tugas ringkasan. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | Menentukan apakah sebuah tugas adalah proyek yang disisipkan. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | Menentukan apakah subproyek bersifat hanya-baca. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | Menentukan apakah sebuah tugas adalah tugas ringkasan. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | Tanggal terakhir yang dapat diselesaikan oleh tugas tanpa menunda penyelesaian proyek. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | Tanggal terakhir yang dapat dimulai oleh tugas tanpa menunda penyelesaian proyek. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | Menentukan apakah fungsi leveling dapat menunda dan membagi penugasan individu untuk menyelesaikan alokasi berlebih. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | Menentukan apakah fungsi leveling sumber daya dapat menyebabkan pemisahan pada pekerjaan yang tersisa pada tugas ini. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | Waktu yang harus ditunda dari tanggal mulai awal tugas karena leveling sumber daya. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | Mendefinisikan durasi yang dijadwalkan secara manual untuk sebuah tugas. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | Mendefinisikan penyelesaian yang dijadwalkan secara manual untuk sebuah tugas. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | Mendefinisikan mulai yang dijadwalkan secara manual untuk sebuah tugas. |
| static readonly [Name](../../aspose.tasks/tsk/name/) | Nama tugas. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | Catatan teks dalam format RTF. Hanya didukung untuk format MPP. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | Teks polos catatan yang diekstrak dari data RTF. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | Tingkat outline tugas. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | Angka yang mewakili posisi tugas dalam struktur outline hierarkis. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | Total biaya lembur untuk sebuah tugas, untuk sebuah sumber daya pada semua tugas yang ditugaskan, atau untuk penugasan sumber daya. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | Jumlah lembur yang dijadwalkan untuk dilakukan oleh semua sumber daya yang ditugaskan ke sebuah tugas. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | Status terkini tugas, dinyatakan sebagai persentase durasi tugas yang telah selesai. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | Status terkini tugas dinyatakan sebagai persentase pekerjaan yang telah selesai. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | Nilai persentase selesai yang dapat digunakan sebagai alternatif untuk menghitung biaya anggaran pekerjaan yang dilakukan (BCWP). |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | Tanggal selesai tugas seperti sebelum leveling sumber daya dilakukan. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | Tanggal mulai tugas seperti sebelum leveling sumber daya dilakukan. |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | Tingkat pentingnya sebuah tugas, yang pada gilirannya menunjukkan seberapa mudah tugas atau penugasan dapat ditunda atau dibagi selama leveling sumber daya. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | Total jumlah pekerjaan non-lembur yang dijadwalkan untuk dilakukan oleh sumber daya. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | Biaya terjadwal yang tersisa yang akan timbul dalam menyelesaikan pekerjaan terjadwal yang tersisa. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | Waktu yang diperlukan untuk menyelesaikan bagian tugas yang belum selesai. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | Biaya lembur terjadwal yang tersisa untuk sebuah tugas. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | Jumlah waktu lembur terjadwal yang tersisa. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | Waktu yang masih diperlukan untuk menyelesaikan sebuah tugas atau sekumpulan tugas. |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | Tanggal bagian tersisa tugas dijadwalkan untuk dilanjutkan setelah ada kemajuan. |
| static readonly [Start](../../aspose.tasks/tsk/start/) | Tanggal mulai terjadwal sebuah tugas. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | Durasi antara tanggal Early Start dan Late Start. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | Mengembalikan teks mulai tugas. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | Waktu yang mewakili selisih antara tanggal mulai baseline sebuah tugas atau penugasan dan tanggal mulai yang dijadwalkan saat ini. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | Nama sumber daya perusahaan yang akan menerima pembaruan status untuk tugas saat ini dari sumber daya. |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | Tanggal yang mewakili akhir bagian aktual dari sebuah tugas. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | Lokasi sumber dari subproyek. |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | Variansi jadwal nilai yang diperoleh, hingga tanggal status proyek. Variansi jadwal (SV) adalah selisih antara BCWP dan BCWS. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | Waktu tanggal selesai tugas dapat ditunda tanpa menunda tanggal selesai proyek. |
| static readonly [Type](../../aspose.tasks/tsk/type/) | Tipe tugas. |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | Id unik dari tugas. |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | Mewakili flag yang menunjukkan bahwa tugas memiliki ketidaksesuaian jadwal. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | Kode struktur rincian kerja (WBS). |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | Level WBS paling kanan dari tugas. |
| static readonly [Work](../../aspose.tasks/tsk/work/) | Total waktu yang dijadwalkan pada tugas untuk semua sumber daya yang ditugaskan. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | Selisih antara pekerjaan baseline sebuah tugas dan pekerjaan yang dijadwalkan saat ini. |

## Contoh

Menampilkan cara membaca/menulis properti tugas.

```csharp
var project = new Project();

// Tambahkan tugas dan atur properti tugas
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


