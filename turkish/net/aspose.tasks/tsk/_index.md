---
title: Tsk
second_title: Aspose.Tasks for .NET API Referansı
description: Şunların özelliklerini temsil ederTask./task nesne.
type: docs
weight: 2290
url: /tr/net/aspose.tasks/tsk/
---
## Tsk class

Şunların özelliklerini temsil eder:[`Task`](../task) nesne.

```csharp
public static class Tsk
```

## Alanlar

| İsim | Tanım |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid) | Etkinlik kimliği alanını temsil eder - Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı. (yalnızca Primavera projeleri için geçerlidir). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost) | Görevle ilişkili diğer kayıtlı maliyetlerle birlikte, kaynaklar tarafından görevlerinde halihazırda gerçekleştirilen çalışma için katlanılan maliyetler. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration) | Planlanan süreye ve mevcut kalan çalışmaya veya tamamlanma yüzdesine dayalı olarak bir görevin fiili çalışma süresinin kapsamı. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish) | Bir görevin tamamlandığı tarih. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost) | Atanan kaynaklar tarafından görevlerde gerçekleştirilen fazla mesai için katlanılan maliyetler. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework) | Görevlere atanan kaynaklar tarafından halihazırda gerçekleştirilmiş fazla mesai miktarı. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected) | Gerçek fazla mesai çalışmasının korunduğu süre.  Yalnızca XML biçimi için desteklenen okuma. [`Duration`](./duration) type. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart) | Bir görevin fiilen başladığı tarih ve saat. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork) | Görevlere atanan kaynaklar tarafından halihazırda yapılmış olan çalışma miktarı. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected) | Gerçek çalışmanın korunduğu süre.  Yalnızca XML biçimi için desteklenen okuma. [`Duration`](./duration) type. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp) | Proje durumu tarihine veya bugünün tarihine kadar, bir görev üzerinde halihazırda yapılmış olan çalışmalar için katlanılan maliyetler. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp) | Zaman aşamalı temel maliyetlerle çarpılan görevin tamamlanma yüzdesinin kümülatif değeri. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws) | Durum tarihine veya bugünün tarihine kadar kümülatif zaman aşamalı temel maliyetler. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost) | Bütçe maliyet kaynakları için bütçe maliyetleri. Bütçe kaynakları yalnızca proje özet görevine atanır. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork) | Bütçe çalışması ve malzeme kaynakları için bütçe çalışması. Bütçe kaynakları yalnızca proje özet görevine atanır. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar) | Görev takvimi. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish) | Teslimatın bitiş tarihi.  Okuma yalnızca XML biçimi için desteklenir. DateTime tip. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart) | Teslimatın başlangıç tarihi.  Okuma yalnızca XML biçimi için desteklenir. DateTime tip. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype) | Bir görevin ilişkili bir teslimatı olup olmadığını veya ilişkili bir teslimata bağımlı olup olmadığını belirler.  Okuma yalnızca XML biçimi için desteklenir. Int32 type. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate) | Kısıtlama türüyle ilişkili belirli tarih. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype) | Bir görevi zamanlamak için uygulanabilecek kısıtlama türü için seçenekler sunar. |
| static readonly [Contact](../../aspose.tasks/tsk/contact) | Bir görevden sorumlu kişinin adı. |
| static readonly [Cost](../../aspose.tasks/tsk/cost) | Kalan çalışma için planlanan maliyetlere ek olarak, görevlere atanan kaynaklar tarafından gerçekleştirilen çalışma için halihazırda katlanılan maliyetlere dayalı olarak bir görevin toplam zamanlanan veya öngörülen maliyeti. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance) | Bir görev, kaynak veya atama için temel maliyet ile toplam maliyet arasındaki fark. |
| static readonly [Created](../../aspose.tasks/tsk/created) | Görevin oluşturulduğu tarih. |
| static readonly [CV](../../aspose.tasks/tsk/cv) | Bir görevin temel maliyeti ile toplam maliyeti arasındaki fark. Maliyet Farkı = Maliyet - Temel Maliyet |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline) | Bir görevin ne zaman tamamlanacağını gösteren bir hedef tarih. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary) | Görevin özet görev olarak görüntülenip görüntülenmeyeceğini belirler.  Okuma yalnızca XML biçimi için desteklenir. Boolean tip. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline) | Bir görevin zaman çizelgesi görünümünde görüntülenip görüntülenmeyeceğini belirtir. |
| static readonly [Duration](../../aspose.tasks/tsk/duration) | Başlangıç tarihi, bitiş tarihi, takvimler ve diğer zamanlama faktörlerine göre girilen veya Microsoft Project tarafından hesaplandığı şekliyle bir görev için etkin çalışma süresinin toplam aralığı. |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat) | Görev süresi biçimi. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext) | Görevin süre metnini döndürür. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance) | Bir görevin temel süresi ile bir görevin toplam süresi (geçerli tahmin) arasındaki fark. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish) | Önceki ve sonraki görevlerin erken bitiş tarihlerine, diğer kısıtlamalara ve herhangi bir seviyelendirme gecikmesine bağlı olarak, bir görevin bitebileceği en erken tarih. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart) | Öncel ve ardıl görevlerin erken başlangıç tarihlerine ve diğer kısıtlamalara bağlı olarak, bir görevin başlayabileceği en erken tarih. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod) | Gerçekleştirilen işin bütçelenmiş maliyetini (BCWP) hesaplamak için Tamamlanma Yüzdesi veya Fiziksel Tamamlanma Yüzdesi alanının kullanılması gerektiğini belirler. |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid) | Bir görev harici bir görevse, görevin harici kimliğini içerir. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject) | Harici bir görevin kaynak konumu ve görev tanımlayıcısı. |
| static readonly [Finish](../../aspose.tasks/tsk/finish) | Bir görevin planlanan bitiş tarihi. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan) | Erken Bitirme ve Geç Bitirme tarihleri arasındaki süre. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext) | Görevin bitiş metnini döndürür. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance) | Bir görevin veya atamanın temel bitiş tarihi ile geçerli bitiş tarihi arasındaki farkı temsil eden saat. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost) | Herhangi bir kaynak dışı görev masrafını gösterir. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual) | Sabit maliyetlerin nasıl ve ne zaman bir görevin maliyetine yansıtılacağına veya tahakkuk ettirileceğine ilişkin seçenekleri belirler. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan) | Bir görevin ardıl görevleri geciktirmeden geciktirilebileceği süre. |
| static readonly [Guid](../../aspose.tasks/tsk/guid) | Bir görev için oluşturulan benzersiz tanımlama kodları. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource) | Görevin atanan görevler üzerinde normal çalışma kapasitesi dahilinde tamamlanabilecekten daha fazla işi olan bir kaynağa sahip olup olmadığını gösterir. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar) | Microsoft Project'te görüntülendiğinde bir görevin Gantt çubuğunun gizlenip gizlenmeyeceğini belirler. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink) | Bir görevle ilişkili bir köprünün başlığı veya açıklayıcı metni. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress) | Bir görevle ilişkili köprünün adresi. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress) | Bir görevle ilişkili bir köprüdeki belgedeki belirli konum. |
| static readonly [Id](../../aspose.tasks/tsk/id) | Görevler listesindeki bir görevin konum tanımlayıcısı. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar) | Görev zamanlamasının göreve atanan kaynakların takvimlerini dikkate alıp almayacağını belirler. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings) | Microsoft Project'te zamanlama çakışması uyarı göstergesinin gizlenip gizlenmeyeceğini belirtir. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive) | Bir görevin etkin olup olmadığını belirler. Etkin olmayan görevler artık diğer görevleri veya genel Proje zamanlamasını etkilemez. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical) | Bir görevin kritik yolda olup olmadığını belirler. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven) | Görev için zamanlamanın çabaya dayalı zamanlama olup olmadığını belirler. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated) | Bir görevin tahmin edilip edilmediğini belirler. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded) | Bir özet görevin GanttChart görünümünde genişletilip genişletilmediğini belirler. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask) | Bir görevin harici olup olmadığını belirler. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual) | Bir görevin manuel olarak zamanlanıp zamanlanmadığını belirler. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked) | Bir görevin daha fazla eylem veya bir tür tanımlama için işaretlenip işaretlenmediğini gösterir. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone) | Bir görevin bir dönüm noktası olup olmadığını belirler. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull) | Bir görevin boş bir görev olup olmadığını belirler. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated) | Bir göreve atanan kaynaklardan herhangi birinin, görev üzerinde normal çalışma kapasitesiyle yapılabilecekten daha fazla çalışmaya atanıp atanmadığını gösterir. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished) | Geçerli görevin projenin geri kalanıyla birlikte Project Server'da yayımlanıp yayımlanmayacağını belirler. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring) | Bir görevin bir dizi yinelenen görevin parçası olup olmadığını belirler. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid) | Bir görevin devam ettirilip sürdürülemeyeceğini belirler. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup) | Alt görev Gantt çubukları hakkındaki bilgilerin özet görev çubuğuna toplanıp toplanamayacağını belirler. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject) | Görevin eklenmiş bir proje olup olmadığını belirler. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly) | Bir alt projenin salt okunur olup olmadığını belirler. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary) | Bir görevin özet görev olup olmadığını belirler. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish) | Bir görevin projenin bitişini geciktirmeden bitirebileceği en son tarih. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart) | Bir görevin projenin bitişini geciktirmeden başlayabileceği en son tarih. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments) | Seviyelendirme işlevinin, fazla tahsisleri çözmek için ayrı atamaları geciktirip bölemeyeceğini belirler. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit) | Kaynak seviyelendirme işlevinin bu görevde kalan iş üzerinde bölünmelere neden olup olmayacağını belirler. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay) | Kaynak seviyelendirme nedeniyle bir görevin erken başlangıç tarihinden itibaren ertelenmesi gereken süre. |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat) | Gecikme süresini ifade etme biçimi. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration) | Bir görevin manuel olarak zamanlanan süresini tanımlar. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish) | Bir görevin manuel olarak zamanlanmış bitişini tanımlar. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart) | Bir görevin manuel olarak zamanlanmış başlangıcını tanımlar. |
| static readonly [Name](../../aspose.tasks/tsk/name) | Bir görevin adı. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf) | RTF biçiminde metin notları. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext) | Notes'un RTF verilerinden çıkarılan düz metni. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel) | Bir görevin anahat düzeyi. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber) | Bir görevin hiyerarşik anahat yapısındaki konumunu temsil eden sayı. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost) | Bir görevin, atanan tüm görevlerdeki bir kaynağın veya bir kaynak atamasının toplam fazla mesai maliyeti. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework) | Bir göreve atanan tüm kaynaklar tarafından gerçekleştirilmesi planlanan fazla mesai miktarı. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete) | Görevin tamamlanan süresinin yüzdesi olarak ifade edilen, görevin mevcut durumu. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete) | Tamamlanan işin yüzdesi olarak ifade edilen bir görevin mevcut durumu. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete) | Gerçekleştirilen işin bütçelenmiş maliyetini (GÇBM) hesaplamak için alternatif olarak kullanılabilecek tam değer yüzdesi. |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish) | Bir görevin kaynak seviyelendirme yapılmadan önceki bitiş tarihi. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart) | Bir görevin kaynak seviyelendirme yapılmadan önceki başlangıç tarihi. |
| static readonly [Priority](../../aspose.tasks/tsk/priority) | Bir göreve verilen önem düzeyi, bu da kaynak seviyelendirme sırasında bir görevin veya atamanın ne kadar kolaylıkla ertelenebileceğini veya bölünebileceğini gösterir. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork) | Kaynaklar tarafından gerçekleştirilmesi planlanan toplam fazla mesai dışı çalışma miktarı. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost) | Kalan zamanlanmış işin tamamlanması için katlanılacak kalan zamanlanmış gider. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration) | Bir görevin tamamlanmamış kısmını tamamlamak için gereken süre. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost) | Bir görev için kalan zamanlanmış fazla mesai gideri. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework) | Kalan programlanmış fazla mesai miktarı. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork) | Bir görevi veya bir dizi görevi tamamlamak için gereken süre. |
| static readonly [Resume](../../aspose.tasks/tsk/resume) | Herhangi bir ilerleme girdikten sonra görevin kalan bölümünün devam etmesi için programlandığı tarih. |
| static readonly [Start](../../aspose.tasks/tsk/start) | Bir görevin planlanan başlangıç tarihi. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan) | Erken Başlangıç ve Geç Başlangıç tarihleri arasındaki süre. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext) | Görevin başlangıç metnini döndürür. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance) | Bir görevin veya atamanın temel başlangıç tarihi ile şu anda zamanlanan başlangıç tarihi arasındaki farkı temsil eden saat. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager) | Mevcut görev için durum güncellemelerini kaynaklardan alacak olan kurumsal kaynağın adı. |
| static readonly [Stop](../../aspose.tasks/tsk/stop) | Bir görevin fiili bölümünün sonunu temsil eden tarih. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname) | Bir alt projenin kaynak konumu. |
| static readonly [SV](../../aspose.tasks/tsk/sv) | Proje durum tarihi boyunca kazanılan değer zaman çizelgesi farkı. Zaman çizelgesi farkı (SV), GÇBM ile GÇBM arasındaki farktır. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan) | Bir görevin bitiş tarihinin, projenin bitiş tarihini geciktirmeden ertelenebileceği saat. |
| static readonly [Type](../../aspose.tasks/tsk/type) | Görev türü. |
| static readonly [Uid](../../aspose.tasks/tsk/uid) | Bir görevin benzersiz kimliği. |
| static readonly [Warning](../../aspose.tasks/tsk/warning) | Görevin zamanlama tutarsızlıkları olduğunu gösteren bayrağı temsil eder. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs) | İş kırılım yapısı (WBS) kodları. |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel) | Bir görevin en sağdaki İKY düzeyi. |
| static readonly [Work](../../aspose.tasks/tsk/work) | Atanan tüm kaynaklar için bir görevde zamanlanan toplam süre. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance) | Bir görevin temel çalışması ile mevcut zamanlanmış çalışma arasındaki fark. |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
