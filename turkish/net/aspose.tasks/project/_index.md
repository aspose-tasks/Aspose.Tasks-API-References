---
title: "Sınıf Project"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Project sınıfı. Bir projeyi temsil eder"
type: docs
weight: 1440
url: /tr/net/aspose.tasks/project/
---
## Project class

Bir projeyi temsil eder.

```csharp
public class Project
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Project](project/#constructor)() | `Project` sınıfının yeni bir örneğini başlatır. |
| [Project](project/#constructor_1)(DbSettings) | `Project` sınıfının yeni bir örneğini, [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/) sınıfının örneğiyle belirtilen bir veritabanından veri okumak için başlatır. |
| [Project](project/#constructor_2)(Stream) | `Project` sınıfının yeni bir örneğini bir akıştan başlatır. |
| [Project](project/#constructor_7)(StreamReader) | `Project` sınıfının yeni bir örneğini bir StreamReader örneğinden başlatır. |
| [Project](project/#constructor_8)(string) | `Project` sınıfının yeni bir örneğini bir şablondan (var olan mpp veya mpt dosyası) başlatır. |
| [Project](project/#constructor_3)(Stream, LoadOptions) | `Project` sınıfının yeni bir örneğini, belirtilen [`LoadOptions`](../loadoptions/) sınıfı örneğiyle Akıştan başlatır. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | `Project` sınıfının yeni bir örneğini bir şablondan(var olan mpp veya mpt dosyası) başlatır. |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | `Project` sınıfının yeni bir örneğini, belirtilen [`PrimaveraReadOptions`](../primaverareadoptions/) sınıfı örneğiyle Akıştan başlatır. |
| [Project](project/#constructor_6)(Stream, string) | `Project` sınıfının yeni bir örneğini bir şablondan(var olan mpp veya mpt dosyası) başlatır. |
| [Project](project/#constructor_9)(string, LoadOptions) | `Project` sınıfının yeni bir örneğini bir şablondan (var olan mpp veya mpt dosyası) belirtilen [`LoadOptions`](../loadoptions/) sınıfı örneğiyle başlatır. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | `Project` sınıfının yeni bir örneğini bir şablondan (var olan mpp veya mpt dosyası) başlatır. |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | `Project` sınıfının yeni bir örneğini bir şablondan (var olan MPP veya MPT dosyası) belirtilen [`PrimaveraReadOptions`](../primaverareadoptions/) sınıfı örneğiyle başlatır. |
| [Project](project/#constructor_12)(string, string) | Parola korumalı bir şablondan (var olan mpp veya mpt dosyası) `Project` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | AreEditableActualCosts'in ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Author değerini alır veya ayarlar. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | AutoAddNewResourcesAndTasks'in ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır veya ayarlar. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Autolink'in ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | BaselineForEarnedValue değerini alır veya ayarlar. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Projenin yerleşik özellikler koleksiyonunu alır. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Bir projenin hesaplama modunu alır veya ayarlar. [`CalculationMode`](./calculationmode/) enumarasyonunun değerlerinden biri olabilir. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Calendar değerini alır veya ayarlar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Bu `Project` örneğinin [`CalendarCollection`](../calendarcollection/) nesnesini alır. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Category değerini alır veya ayarlar. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Comments değerini alır veya ayarlar. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Company değerini alır veya ayarlar. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | CreationDate değerini alır veya ayarlar. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Bu projenin Kritik Yolunu oluşturan Kritik görevlerin bir listesini içeren bir koleksiyonu alır. Bu, projedeki görev sayısı n olduğunda O(n) bir işlemdir. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Toplam gecikme süresi bu gün sayısına eşit veya daha az ise MS Project görevleri kritik olarak kabul eder. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | CurrencyCode değerini alır veya ayarlar. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | CurrencyDigits değerini alır veya ayarlar. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | CurrencySymbol değerini alır veya ayarlar. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | CurrencySymbolPosition değerini alır veya ayarlar. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | CurrentDate değerini alır veya ayarlar. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | CustomDateFormat değerini alır veya ayarlar. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Projenin özel özellikler koleksiyonunu alır. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | DateFormat'in bir değerini alır veya ayarlar. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | DaysPerMonth'ın bir değerini alır veya ayarlar. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | DefaultFinishTime'ın bir değerini alır veya ayarlar. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | DefaultFixedCostAccrual'ın bir değerini alır veya ayarlar. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | DefaultOvertimeRate'ın bir değerini alır veya ayarlar. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | DefaultStandardRate'ın bir değerini alır veya ayarlar. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | DefaultStartTime'ın bir değerini alır veya ayarlar. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | DefaultTaskEVMethod'ın bir değerini alır veya ayarlar. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | DefaultTaskType'ın bir değerini alır veya ayarlar. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Projenin varsayılan görünümünü alır veya ayarlar. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | [`WeekDayCollection`](../weekdaycollection/) sınıfının bir örneğini alır; bu sınıf proje varsayılan hafta çalışma günleri ve çalışma saatlerinin bir koleksiyonunu temsil eder. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | [`ProjectDisplayOptions`](../projectdisplayoptions/) sınıfının bir örneğini alır. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | DurationFormat'ın bir değerini alır veya ayarlar. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | EarnedValueMethod'ın bir değerini alır veya ayarlar. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | ExtendedAttributeDefinitionCollection nesnesini alır. Bu nesne, bir proje ile ilişkili genişletilmiş öznitelik (özel alanlar) tanımlarının koleksiyonudur. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | ExtendedCreationDate'in bir değerini alır veya ayarlar. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | FinishDate'in bir değerini alır veya ayarlar. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | FiscalYearStart'ın ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | FyStartDate'in bir değerini alır veya ayarlar. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Projenin küreselleştirme (dile özgü) ayarlarını alır veya ayarlar. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Guid değerini alır veya ayarlar. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | HonorConstraints'ın ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | HyperlinkBase'in bir değerini alır veya ayarlar. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | InsertedProjectsLikeSummary'ın ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled'ın ayarlanıp ayarlanmadığını gösteren bir değeri alır veya ayarlar. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Keywords'in bir değerini alır veya ayarlar. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | LastAuthor değerini alır veya ayarlar. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | LastPrinted değerini alır veya ayarlar. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | LastSaved değerini alır veya ayarlar. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Manager değerini alır veya ayarlar. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | MicrosoftProjectServerURL'nin ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | MinutesPerDay değerini alır veya ayarlar. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | MinutesPerWeek değerini alır veya ayarlar. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | MoveCompletedEndsBack'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | MoveCompletedEndsForward'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | MoveRemainingStartsBack'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | MoveRemainingStartsForward'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | MultipleCriticalPaths'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Name değerini alır veya ayarlar. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | NewTasksAreManual'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | NewTasksEffortDriven'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | NewTasksEstimated'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | NewTaskStartDate değerini alır veya ayarlar. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Bu proje dosyasına bağlı veya gömülü olan [`OleObject`](../oleobject/) sınıfının örneklerini içeren bir koleksiyon alır. Yalnızca mpp dosya formatı için kullanılabilir. Bu koleksiyon, 'Clear' işlemi dışındakiler için yalnızca okunur. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | OutlineCodeDefinitionCollection nesnesini alır. Bir projeye ilişkin outline kod tanımlarının koleksiyonu. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Primavera dosyasından okunan bir proje için Primavera'ya özgü özellikleri içeren bir nesne alır. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | ProjectExternallyEdited'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | RemoveFileProperties'in ayarlanıp ayarlanmadığını gösteren bir değer alır veya ayarlar. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | ResourceAssignmentCollection nesnesini alır. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Kaynak tabanlı tüm filtre tanımlarını alır. ResourceFilters, [`Filter`](../filter/) nesnelerinden oluşan bir koleksiyondur. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Kaynak tabanlı tüm grup tanımlarını alır. ResourceGroups, [`Group`](../group/) nesnelerinden oluşan bir koleksiyondur. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | ResourceCollection nesnesini alır. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Revizyonun değerini alır veya ayarlar. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Görev ağacının kökünü alır. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | SaveVersion değerini alır veya ayarlar. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | ScheduleFromStart ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | ShowProjectSummaryTask ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | SplitsInProgressTasks ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | SpreadActualCost ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | SpreadPercentComplete ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | StartDate değerini alır veya ayarlar. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | StatusDate değerini alır veya ayarlar. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Subject değerini alır veya ayarlar. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | [`Table`](../table/) nesnelerinin bir listesini alır. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Görev tabanlı tüm filtre tanımlarını alır. TaskFilters, [`Filter`](../filter/) nesnelerinden oluşan bir koleksiyondur. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Görev tabanlı tüm grup tanımlarını alır. TaskGroups, [`Group`](../group/) nesnelerinden oluşan bir koleksiyondur. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | [`TaskLinkCollection`](../tasklinkcollection/) nesnesini alır. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | TaskUpdatesResource ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Template değerini alır veya ayarlar. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | TimescaleFinish değerini alır veya ayarlar. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | TimescaleStart değerini alır veya ayarlar. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Title değerini alır veya ayarlar. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Uid değerini alır veya ayarlar. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | UpdateManuallyScheduledTasksWhenEditingLinks ayarlı olup olmadığını gösteren değeri alır veya ayarlar. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | [`VbaProject`](./vbaproject/) sınıfının bir örneğini alır. |
| [Views](../../aspose.tasks/project/views/) { get; } | [`View`](../view/) nesnelerinin bir listesini alır. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Proje için WBS Kod Tanımını alır veya ayarlar. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | WeekStartDay değerini alır veya ayarlar. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | WorkFormat değerini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Kök görevi dahil olmak üzere projenin tüm görevlerini yinelemeli olarak listeler. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Bu kapsayıcıda özelliğin eşlendiği değeri döndürür. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Temel kaydetme zamanını döndürür. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | [`Duration`](../duration/) nesnesini belirtilen birim sayısı ve projenin ayarlarında tanımlı varsayılan süre biçimi olan [`DurationFormat`](../prj/durationformat/) ile alır. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | [`Duration`](../duration/) nesnesini belirtilen sayıdaki [`TimeUnitType`](../timeunittype/) birimleriyle alır. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | [`Duration`](../duration/) nesnesini belirtilen TimeSpan değeri ve belirtilen [`TimeUnitType`](../timeunittype/) değeriyle alır. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Varsayılan [`Timescale`](../../aspose.tasks.visualization/timescale/) (Gün) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Varsayılan [`Timescale`](../../aspose.tasks.visualization/timescale/) (Gün) ve verilen [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Verilen [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Verilen [`Timescale`](../../aspose.tasks.visualization/timescale/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Verilen [`Timescale`](../../aspose.tasks.visualization/timescale/) ve [`PageSize`](../../aspose.tasks.visualization/pagesize/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Verilen [`Timescale`](../../aspose.tasks.visualization/timescale/) ve [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Verilen [`Timescale`](../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) ve tarih aralığı kullanılarak oluşturulacak projenin sayfa sayısını döndürür. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Belirtilen görevin öncülleri olan görev bağlantılarının bir koleksiyonunu döndürür. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | [`Duration`](../duration/) nesnesini belirtilen Double değeri ve varsayılan iş biçimiyle alır. |
| [Print](../../aspose.tasks/project/print/#print)() | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin varsayılan yazıcıya, varsayılan yazıcı ayarlarıyla yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarlarına göre yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin varsayılan yazıcıya, varsayılan yazıcı ayarları ve özel kaydetme seçenekleriyle yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcıya, varsayılan yazıcı ayarlarıyla yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarları ve özel kaydetme seçeneklerine göre yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarlarına göre yazdırır. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak projenin belirtilen yazıcı ayarları, özel kaydetme seçenekleri ve belirtilen belge adıyla yazdırır. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | İsteğe bağlı doğrulama ile tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Kaynakların kimliğini, başlangıç ve bitiş tarihlerini yeniden hesaplar. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Proje kaynak atamaları listesinden geçersiz kaynak atamalarını ortadan kaldırır. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Tüm görevlerin WBS kodunu yeniden numaralandırır. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Geçmiş görevlerin WBS kodunu yeniden numaralandırır. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Tamamlanmamış proje işini belirtilen tarihten sonra başlayacak şekilde yeniden zamanlar. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Belirtilen görev listesi için tamamlanmamış işi, belirtilen tarihten sonra başlayacak şekilde yeniden zamanlar. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Proje verilerini mpp formatında dosyaya kaydeder. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Proje verilerini akışa kaydeder. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak projeyi akışa kaydeder. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Proje verilerini dosyaya kaydeder. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak belgeyi dosyaya kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Projeyi şablon olarak belirtilen akışa kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Projeyi şablon olarak belirtilen dosya yoluna kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Projeyi şablon olarak belirtilen akışa kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Projeyi şablon olarak kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Proje genel bakış raporunu akışa kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Proje genel bakış raporunu PDF dosyasına kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Belirtilen türdeki proje raporunu belirtilen akışa kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Belirtilen türdeki proje raporunu PDF formatında belirtilen dosya yoluna kaydeder. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Kök görevin tüm alt görevlerini özyinelemeli olarak toplar. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Tüm proje için belirtilen temel çizgiye temel alan alanlarını kaydeder. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Seçilen görevler için belirtilen temel çizgiye temel alan alanlarını kaydeder. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Temel çizgi kaydetme zamanını ayarlar. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Tüm proje için belirtilen tarihe kadar tüm işi tamamlanmış olarak günceller. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Belirtilen görev listesi için belirtilen tarihe kadar tüm işi tamamlanmış olarak günceller. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Akıştan proje dosyası bilgilerini alır. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Dosyadan proje dosyası bilgilerini okur. |

## Açıklamalar

Bu **Project**, Aspose.Tasks kitaplığında merkezi bir sınıftır.

Birisi **Project**'i kullanarak desteklenen proje yönetimi formatlarından birini okuyabilir: MPP, MPT, MPX, XML.

Desteklenen formatların herhangi birinde mevcut bir belgeyi yüklemek için, bir dosya adı veya akışı **Project** yapıcılarından birine aktarın. Boş bir proje oluşturmak için, parametresiz yapıcıyı çağırın.

Projeyi herhangi bir [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) formatında kaydetmek için Save metodunun aşırı yüklemelerinden birini kullanın: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Sabit Düzen: PDF; Görüntüler: JPEG, PNG, BMP, TIFF, SVG; Metin: TXT; Diğerleri: HTML.

**Project**, proje genelindeki bilgileri saklar, örneğin [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), ve [`ExtendedAttributes`](./extendedattributes/). Bu nesnelerin çoğu, **Project** sınıfının ilgili özellikleri aracılığıyla erişilebilir.

**Project**, diğer proje varlıklarını manipüle etmek için giriş noktaları içeren bir kök varlıktır, örneğin [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) ve [`Calendar`](../calendar/).

**Project** varlıklarına tiplenmiş koleksiyonlar aracılığıyla erişilebilir, örneğin [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), vb.

## Örnekler

Bir &lt;see cref="Aspose.Tasks.Project"/&gt; örneğiyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// yeni görevler ekleyerek istenen özellikleri ayarlama
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// yeni kaynaklar ekleme
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// yeni kaynak atamaları ekleme
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// projeyi mevcut formatlardan birinde kaydet
// burada projeyi Microsoft Project XML dosya formatında kaydediyoruz.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


