---
title: "Proje"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir projeyi temsil eder."
type: docs
weight: 220
url: /tr/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Bir projeyi temsil eder.

--------------------

Bu **Project**, Aspose.Tasks kütüphanesinde merkezi bir sınıftır.

Birisi **Project**'i desteklenen proje yönetimi formatlarından birini okumak için kullanabilir: MPP, MPT, MPX, XML.

Desteklenen formatlardan herhangi birinde mevcut bir belgeyi yüklemek için, bir dosya adı ya da akışı **Project** yapıcılarından birine geçirin. Boş bir proje oluşturmak için, parametresiz yapıcıyı çağırın.

Projeyi herhangi bir [SaveFileFormat](../../com.aspose.tasks/savefileformat) formatında kaydetmek için Save yöntemi aşırı yüklemelerinden birini kullanın: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Sabit Düzen: PDF; Görseller: JPEG, PNG, BMP, TIFF, SVG; Metin: TXT; Diğerleri: HTML.

Projeyi yazdırmak için, [print()](../../com.aspose.tasks/project\#print--) yöntemi aşırı yüklemelerinden birini kullanın.

Bu **Project**, proje genelinde `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), ve `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)) gibi bilgileri saklar. Bu nesnelerin çoğu **Project** sınıfının ilgili özellikleri aracılığıyla erişilebilir.

Bu **Project**, diğer proje varlıklarını manipüle etmek için giriş noktaları içeren bir kök varlıktır; örnek olarak [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) ve [Calendar](../../com.aspose.tasks/calendar) bulunur.

Bu **Project** varlıklarına tiplenmiş koleksiyonlar aracılığıyla erişilebilir; örneğin `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), vb.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Project()](#Project--) | [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Şifre korumalı bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğiyle akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Bir akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğiyle bir şablondan (var olan MPP veya MPT dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Veritabanından veri okumak için, [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini, [DbSettings](../../com.aspose.tasks/dbsettings) sınıfının örneğiyle belirtilen bir veritabanı kullanarak başlatır. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneğiyle, mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneğiyle, akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Bu konteynerde özelliğin eşlendiği değeri döndürür. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Belirtilen özelliği bu konteynerde belirtilen değere eşler. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Kök görevi dahil olmak üzere projenin tüm görevlerini özyinelemeli olarak listeler. |
| [getActualsInSync()](#getActualsInSync--) | ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getAdminProject()](#getAdminProject--) | AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | AreEditableActualCosts'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getAuthor()](#getAuthor--) | Author değerini alır. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | AutoAddNewResourcesAndTasks'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır. |
| [getAutolink()](#getAutolink--) | Autolink'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | BaselineForEarnedValue değerini alır. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Temel çizgi kaydetme zamanını döndürür. |
| [getBuiltInProps()](#getBuiltInProps--) | Projenin yerleşik özellikler koleksiyonunu alır. |
| [getCalculationMode()](#getCalculationMode--) | Bir projenin hesaplama modunu alır. |
| [getCalendar()](#getCalendar--) | Calendar değerini alır. |
| [getCalendars()](#getCalendars--) | Bu Project örneğinin [CalendarCollection](../../com.aspose.tasks/calendarcollection) nesnesini alır. |
| [getCategory()](#getCategory--) | Category değerini alır. |
| [getComments()](#getComments--) | Comments değerini alır. |
| [getCompany()](#getCompany--) | Company değerini alır. |
| [getCreationDate()](#getCreationDate--) | CreationDate değerini alır. |
| [getCriticalPath()](#getCriticalPath--) | Bu projenin Kritik Yolunu oluşturan Kritik görevlerin listesini içeren bir koleksiyon alır. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | MS Project'e göre, toplam boşluk bu gün sayısına eşit veya daha az ise görevler kritik kabul edilir. |
| [getCurrencyCode()](#getCurrencyCode--) | CurrencyCode değerini alır. |
| [getCurrencyDigits()](#getCurrencyDigits--) | CurrencyDigits değerini alır. |
| [getCurrencySymbol()](#getCurrencySymbol--) | CurrencySymbol değerini alır. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | CurrencySymbolPosition değerini alır. |
| [getCurrentDate()](#getCurrentDate--) | CurrentDate değerini alır. |
| [getCustomDateFormat()](#getCustomDateFormat--) | CustomDateFormat değerini alır. |
| [getCustomProps()](#getCustomProps--) | Projenin özel özellikler koleksiyonunu alır. |
| [getDateFormat()](#getDateFormat--) | DateFormat değerini alır. |
| [getDaysPerMonth()](#getDaysPerMonth--) | DaysPerMonth değerini alır. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | DefaultFinishTime değerini alır. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | DefaultFixedCostAccrual değerini alır. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | DefaultOvertimeRate değerini alır. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | DefaultStandardRate değerini alır. |
| [getDefaultStartTime()](#getDefaultStartTime--) | DefaultStartTime değerini alır. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | DefaultTaskEVMethod değerini alır. |
| [getDefaultTaskType()](#getDefaultTaskType--) | DefaultTaskType değerini alır. |
| [getDefaultView()](#getDefaultView--) | Projenin varsayılan görünümünü alır. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Projede varsayılan hafta çalışma günleri ve çalışma saatlerini temsil eden [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) sınıfının örneğini alır. |
| [getDisplayOptions()](#getDisplayOptions--) | [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) sınıfının bir örneğini alır. |
| [getDuration(double val)](#getDuration-double-) | Projede ayarların [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) içinde tanımlanan varsayılan süre biçimi ve belirtilen birim sayısı ile [Duration](../../com.aspose.tasks/duration) nesnesini alır. |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Belirtilen sayıda [TimeUnitType](../../com.aspose.tasks/timeunittype) birimiyle [Duration](../../com.aspose.tasks/duration) nesnesini alır. |
| [getDurationFormat()](#getDurationFormat--) | DurationFormat değerini alır. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | EarnedValueMethod değerini alır. |
| [getExtendedAttributes()](#getExtendedAttributes--) | ExtendedAttributeDefinitionCollection nesnesini alır. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | ExtendedCreationDate değerini alır. |
| [getFinishDate()](#getFinishDate--) | FinishDate değerini alır. |
| [getFiscalYearStart()](#getFiscalYearStart--) | FiscalYearStart'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getFyStartDate()](#getFyStartDate--) | FyStartDate değerini alır. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Projenin küreselleştirme (dile özgü) ayarlarını alır. |
| [getGuid()](#getGuid--) | Guid değerini alır. |
| [getHonorConstraints()](#getHonorConstraints--) | HonorConstraints'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getHyperlinkBase()](#getHyperlinkBase--) | HyperlinkBase değerini alır. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | InsertedProjectsLikeSummary'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getKeywords()](#getKeywords--) | Keywords değerini alır. |
| [getLastAuthor()](#getLastAuthor--) | LastAuthor değerini alır. |
| [getLastPrinted()](#getLastPrinted--) | LastPrinted değerini alır. |
| [getLastSaved()](#getLastSaved--) | LastSaved değerini alır. |
| [getManager()](#getManager--) | Manager değerini alır. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | MicrosoftProjectServerURL'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getMinutesPerDay()](#getMinutesPerDay--) | MinutesPerDay değerini alır. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | MinutesPerWeek değerini alır. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | MoveCompletedEndsBack'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | MoveCompletedEndsForward'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | MoveRemainingStartsBack'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | MoveRemainingStartsForward'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | MultipleCriticalPaths'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getName()](#getName--) | Name değerini alır. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | NewTaskStartDate değerini alır. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | NewTasksAreManual'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | NewTasksEffortDriven'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | NewTasksEstimated'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getOleObjects()](#getOleObjects--) | Bu proje dosyasına bağlanmış veya gömülmüş [OleObject](../../com.aspose.tasks/oleobject) sınıfının örneklerini içeren bir koleksiyon alır. |
| [getOutlineCodes()](#getOutlineCodes--) | OutlineCodeDefinitionCollection nesnesini alır. |
| [getPageCount()](#getPageCount--) | Varsayılan [Timescale](../../com.aspose.tasks/timescale)(Gün) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Verilen [SaveOptions](../../com.aspose.tasks/saveoptions) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Verilen [Timescale](../../com.aspose.tasks/timescale) ve [PresentationFormat](../../com.aspose.tasks/presentationformat) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Verilen [Timescale](../../com.aspose.tasks/timescale) ve [PageSize](../../com.aspose.tasks/pagesize) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Verilen [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) ve tarih aralığı kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Varsayılan [Timescale](../../com.aspose.tasks/timescale)(Gün) ve verilen [PresentationFormat](../../com.aspose.tasks/presentationformat) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Verilen [Timescale](../../com.aspose.tasks/timescale) kullanılarak işlenecek proje için sayfa sayısını döndürür. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Belirtilen görevin öncülleri olan görev bağlantılarının bir koleksiyonunu döndürür. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Primavera dosyasından okunan bir proje için Primavera'ya özgü özellikleri içeren bir nesneyi alır. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | ProjectExternallyEdited'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Akıştan proje dosyası bilgilerini alır. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Dosyadan proje dosyası bilgilerini okur. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | RemoveFileProperties'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getResourceAssignments()](#getResourceAssignments--) | ResourceAssignmentCollection nesnesini alır. |
| [getResourceFilters()](#getResourceFilters--) | Kaynak tabanlı tüm filtre tanımlarını alır. |
| [getResourceGroups()](#getResourceGroups--) | Kaynak tabanlı tüm grup tanımlarını alır. |
| [getResources()](#getResources--) | ResourceCollection nesnesini alır. |
| [getRevision()](#getRevision--) | Revision değerini alır. |
| [getRootTask()](#getRootTask--) | Görev ağacının kökünü alır. |
| [getSaveVersion()](#getSaveVersion--) | SaveVersion değerini alır. |
| [getScheduleFromStart()](#getScheduleFromStart--) | ScheduleFromStart'ın ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | ShowProjectSummaryTask'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | SplitsInProgressTasks'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getSpreadActualCost()](#getSpreadActualCost--) | SpreadActualCost'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | SpreadPercentComplete'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getStartDate()](#getStartDate--) | StartDate değerini alır. |
| [getStatusDate()](#getStatusDate--) | StatusDate değerini alır. |
| [getSubject()](#getSubject--) | Subject değerini alır. |
| [getTables()](#getTables--) | [Table](../../com.aspose.tasks/table) nesnelerinin bir listesini alır. |
| [getTaskFilters()](#getTaskFilters--) | Görev tabanlı tüm filtre tanımlarını alır. |
| [getTaskGroups()](#getTaskGroups--) | Görev tabanlı tüm grup tanımlarını alır. |
| [getTaskLinks()](#getTaskLinks--) | [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) nesnesini alır. |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | TaskUpdatesResource'un ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getTemplate()](#getTemplate--) | Template değerini alır. |
| [getTimescaleFinish()](#getTimescaleFinish--) | TimescaleFinish değerini alır. |
| [getTimescaleStart()](#getTimescaleStart--) | TimescaleStart değerini alır. |
| [getTitle()](#getTitle--) | Title değerini alır. |
| [getUid()](#getUid--) | Uid değerini alır. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | UpdateManuallyScheduledTasksWhenEditingLinks'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getVbaProject()](#getVbaProject--) | `VbaProject` sınıfının bir örneğini alır ([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | [View](../../com.aspose.tasks/view) nesnelerinin bir listesini alır. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Proje için WBS Kod Tanımını alır. |
| [getWeekStartDay()](#getWeekStartDay--) | WeekStartDay değerini alır. |
| [getWork(double val)](#getWork-double-) | Belirtilen `double` değer ve varsayılan iş formatı ile [Duration](../../com.aspose.tasks/duration) nesnesini alır. |
| [getWorkFormat()](#getWorkFormat--) | WorkFormat değerini alır. |
| [print()](#print--) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje varsayılan yazıcıya varsayılan yazıcı ayarlarıyla yazdırır. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje varsayılan yazıcıya varsayılan yazıcı ayarları ve özel kaydetme seçenekleriyle yazdırır. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje belirtilen yazıcı ayarlarına göre yazdırır. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje belirtilen yazıcı ayarları ve özel kaydetme seçenekleriyle yazdırır. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje belirtilen yazıcı ayarları, özel kaydetme seçenekleri ve belirtilen belge adıyla yazdırır. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak proje belirtilen yazıcı ayarlarına göre yazdırır. |
| [print(String printerName)](#print-java.lang.String-) | Projeyi belirtilen yazıcıya, varsayılan yazıcı ayarlarıyla, standart (kullanıcı arayüzü olmadan) yazdırma denetleyicisini kullanarak yazdırır. |
| [recalculate()](#recalculate--) | Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihlerini ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihlerini ayarlar, gecikmeleri, işi ve maliyet alanlarını isteğe bağlı doğrulama ile hesaplar. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Kaynakların kimliğini, başlangıç ve bitiş tarihlerini yeniden hesaplar. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Kaynakların başlangıç ve bitiş tarihlerini yeniden hesaplar. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Proje kaynak atamaları listesinden geçersiz kaynak atamalarını ortadan kaldırır. |
| [renumberWBSCode()](#renumberWBSCode--) | Tüm görevlerin WBS kodunu yeniden numaralar. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Geçilen görevlerin WBS kodunu yeniden numaralar. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Tamamlanmamış proje işini belirtilen bir tarihten sonra başlayacak şekilde yeniden planlar. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Belirtilen görev listesi için tamamlanmamış işi, belirtilen bir tarihten sonra başlayacak şekilde yeniden planlar. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Projeyi belirtilen kaydetme seçeneklerini kullanarak bir akışa kaydeder. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Proje verilerini akışa kaydeder. |
| [save(String filename)](#save-java.lang.String-) | Proje verilerini mpp formatında dosyaya kaydeder. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Belgeyi belirtilen kaydetme seçeneklerini kullanarak bir dosyaya kaydeder. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Proje verilerini dosyaya kaydeder. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Projeyi bir şablon olarak belirtilen akışa kaydeder. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Projeyi bir şablon olarak belirtilen akışa kaydeder. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Projeyi bir şablon olarak belirtilen dosya yoluna kaydeder. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Projeyi bir şablon olarak kaydeder. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Proje genel bakış raporunu akışa kaydeder. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Belirtilen türde proje raporunu belirtilen akışa kaydeder. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Proje genel bakış raporunu PDF dosyasına kaydeder. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Belirtilen türde proje raporunu PDF formatında belirtilen dosya yoluna kaydeder. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Kök görevin tüm alt görevlerini yinelemeli olarak toplar. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Belirtilen özelliği bu konteynerde belirtilen değere eşler. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değer belirler. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değer belirler. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | AreEditableActualCosts ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Yazar değerini ayarlar. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | AutoAddNewResourcesAndTasks ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik hesaplanıp hesaplanmayacağını ayarlar. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Autolink ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Temel çizgi alanlarını tüm proje için belirtilen temel çizgiye kaydeder. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Temel çizgi alanlarını seçilen görevler için belirtilen temel çizgiye kaydeder. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | BaselineForEarnedValue değerini ayarlar. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Temel çizgi kaydetme zamanını ayarlar. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Bir projenin hesaplama modunu ayarlar. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar'ın değerini ayarlar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Kategori değerini ayarlar. |
| [setComments(String value)](#setComments-java.lang.String-) | Yorumlar değerini ayarlar. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Şirket değerini ayarlar. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | OluşturmaTarihi değerini ayarlar. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | MS Project'e göre, toplam boşluk bu gün sayısına eşit veya daha az ise görevler kritik kabul edilir. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | ParaBirimiKodu değerini ayarlar. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | ParaBirimiRakamları değerini ayarlar. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | ParaBirimiSembolü değerini ayarlar. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | ParaBirimiSembolüKonumu değerini ayarlar. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | GeçerliTarih değerini ayarlar. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | ÖzelTarihBiçimi değerini ayarlar. |
| [setDateFormat(int value)](#setDateFormat-int-) | TarihBiçimi değerini ayarlar. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | DaysPerMonth değerini ayarlar. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | VarsayılanBitişZamanı değerini ayarlar. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | VarsayılanSabitMaliyetTahakkuku değerini ayarlar. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | VarsayılanFazlaMesaiOranı değerini ayarlar. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | DefaultStandardRate'in değerini ayarlar. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | DefaultStartTime'in değerini ayarlar. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | DefaultTaskEVMethod'in değerini ayarlar. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | DefaultTaskType'in değerini ayarlar. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Projenin varsayılan görünümünü ayarlar. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | DurationFormat'in değerini ayarlar. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | EarnedValueMethod'in değerini ayarlar. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | ExtendedCreationDate'in değerini ayarlar. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | FinishDate'in değerini ayarlar. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | FiscalYearStart'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | FyStartDate'in değerini ayarlar. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Projenin küreselleştirme (dile özgü) ayarlarını ayarlar. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Guid'in değerini ayarlar. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | HonorConstraints'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | HyperlinkBase'in değerini ayarlar. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | InsertedProjectsLikeSummary'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Keywords'in değerini ayarlar. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | LastAuthor'in değerini ayarlar. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | LastPrinted'in değerini ayarlar. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | LastSaved'in değerini ayarlar. |
| [setManager(String value)](#setManager-java.lang.String-) | Manager'in değerini ayarlar. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | MicrosoftProjectServerURL'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | MinutesPerDay'in değerini ayarlar. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | MinutesPerWeek'in değerini ayarlar. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | MoveCompletedEndsBack'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | MoveCompletedEndsForward'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | MoveRemainingStartsBack'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | MoveRemainingStartsForward'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | MultipleCriticalPaths'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Name'in değerini ayarlar. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | NewTaskStartDate değerini ayarlar. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | NewTasksAreManual'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | NewTasksEffortDriven'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | NewTasksEstimated'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | ProjectExternallyEdited'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | RemoveFileProperties'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setRevision(int value)](#setRevision-int-) | Revision değerini ayarlar. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | SaveVersion değerini ayarlar. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | ScheduleFromStart'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | ShowProjectSummaryTask'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | SplitsInProgressTasks'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | SpreadActualCost'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | SpreadPercentComplete'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | StartDate değerini ayarlar. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | StatusDate değerini ayarlar. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Subject değerini ayarlar. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | TaskUpdatesResource'ın ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Template değerini ayarlar. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | TimescaleFinish değerini ayarlar. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | TimescaleStart değerini ayarlar. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Title değerini ayarlar. |
| [setUid(String value)](#setUid-java.lang.String-) | Uid değerini ayarlar. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | UpdateManuallyScheduledTasksWhenEditingLinks'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Proje için WBS Kod Tanımını ayarlar. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | WeekStartDay değerini ayarlar. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | WorkFormat değerini ayarlar. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Tüm proje için belirtilen tarihe kadar tüm işi tamamlanmış olarak günceller. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Belirtilen görev listesi için belirtilen tarihe kadar tüm işi tamamlanmış olarak günceller. |
### Project() {#Project--}
```
public Project()
```


[Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Şifre korumalı bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | java.lang.String | Projeyi oluşturmak için şablonun yolu. |
|  | protectionPassword | java.lang.String | Koruma parolası. |

--------------------

Şu anda yalnızca MSP 2003 dosya formatı için parola korumalı dosyaların okunması desteklenmektedir. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | java.lang.String | Projeyi oluşturmak için şablonun yolu. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğiyle akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Project java.io.InputStreamclass akışı. |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneği, Primavera formatlarının (XER veya XML) okunmasını özelleştirmeye izin verir. |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Bir şablondan (var olan mpp veya mpt dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | java.lang.String | Projeyi oluşturmak için şablonun yolu. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Bir akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Şablon yüklemek için java.io.InputStream. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğiyle bir şablondan (var olan MPP veya MPT dosyası) [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | java.lang.String | Projeyi oluşturmak için şablonun yolu |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Belirtilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneği. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Veritabanından veri okumak için, [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini, [DbSettings](../../com.aspose.tasks/dbsettings) sınıfının örneğiyle belirtilen bir veritabanı kullanarak başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | Belirtilen [DbSettings](../../com.aspose.tasks/dbsettings) sınıfı örneği. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Şablon yüklemek için java.io.InputStream. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Şablon yüklemek için java.io.InputStream. |
|  | protectionPassword | java.lang.String | Koruma parolası. |

--------------------

Şu anda yalnızca MSP 2003 dosya formatı için parola korumalı dosyaların okunması desteklenmektedir. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneğiyle, mevcut mpp veya mpt dosyası şablonundan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | java.lang.String | Projeyi oluşturmak için şablonun yolu |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneği. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneğiyle, akıştan [Project](../../com.aspose.tasks/project) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Project java.io.InputStreamclass akışı. |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | Belirtilen [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfı örneği |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Bu konteynerde özelliğin eşlendiği değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | Belirtilen özellik anahtarı. Özellik anahtarını almak için [Prj](../../com.aspose.tasks/prj). |

**Returns:**
T - bu kapsayıcıda özelliğin eşlendiği değer.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Belirtilen özelliği bu konteynerde belirtilen değere eşler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | Belirtilen özellik anahtarı. Özellik anahtarını almak için [Prj](../../com.aspose.tasks/prj). |
| değer. | T | değer. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Verilerin kopyalanacağı başka bir proje. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Verilerin kopyalanacağı başka bir proje. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Kopyalama sürecini kontrol etmek için kopyalama seçenekleri. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Kök görevi dahil olmak üzere projenin tüm görevlerini özyinelemeli olarak listeler.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - Projenin tüm görevleri üzerinde yineleme yapmak için kullanılabilen IEnumerable.

--------------------

Tüm görevler için bellek ayırmadığından, [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) yöntemine kıyasla görevler üzerinde yineleme yapmak için daha hafif bir yol sağlar.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


AreEditableActualCosts'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Author değerini alır.

**Returns:**
java.lang.String - Author değerinin bir değeri.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


AutoAddNewResourcesAndTasks'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır.

**Returns:**
boolean - atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını belirler.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Autolink'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


BaselineForEarnedValue değerini alır.

**Returns:**
int - BaselineForEarnedValue değerinin bir değeri.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Temel çizgi kaydetme zamanını döndürür. Temel çizgi kaydedilmemişse DateTime.MinValue (00:00:00.0000000 UTC, 1 Ocak 0001) değerini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baselineNumber | int | Temel çizginin numarası [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - Temel çizginin son kaydetme tarihi ve saati.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Projenin yerleşik özellikler koleksiyonunu alır.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Bir projenin hesaplama modunu alır. `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enum değerlerinden biri olabilir.

**Returns:**
int - bir projenin hesaplama modu.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar değerini alır.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Bu Project örneğinin [CalendarCollection](../../com.aspose.tasks/calendarcollection) nesnesini alır.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Category değerini alır.

**Returns:**
java.lang.String - Category değerinin bir değeri.
### getComments() {#getComments--}
```
public final String getComments()
```


Comments değerini alır.

**Returns:**
java.lang.String - Comments değerinin bir değeri.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Company değerini alır.

**Returns:**
java.lang.String - Company değerinin bir değeri.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


CreationDate değerini alır.

**Returns:**
java.util.Date - CreationDate değerinin bir değeri.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Bu projenin Kritik Yolunu oluşturan Kritik görevlerin listesini içeren bir koleksiyon alır.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Bu, O(n) bir işlemdir; burada n, projedeki görev sayısını ifade eder.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


MS Project'e göre, toplam boşluk bu gün sayısına eşit veya daha az ise görevler kritik kabul edilir.

**Returns:**
int - bir görevin kritik kabul edildiği toplam gecikme süresinin (gün cinsinden) maksimum değeri.
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


CurrencyCode değerini alır.

**Returns:**
java.lang.String - CurrencyCode değerinin bir değeri.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


CurrencyDigits değerini alır.

**Returns:**
int - CurrencyDigits değerinin bir değeri.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


CurrencySymbol değerini alır.

**Returns:**
java.lang.String - CurrencySymbol değerinin bir değeri.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


CurrencySymbolPosition değerini alır.

**Returns:**
int - CurrencySymbolPosition değerinin bir değeri.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


CurrentDate değerini alır.

**Returns:**
java.util.Date - CurrentDate değerinin bir değeri.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


CustomDateFormat değerini alır.

**Returns:**
java.lang.String - CustomDateFormat değerinin bir değeri.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Projenin özel özellikler koleksiyonunu alır.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


DateFormat değerini alır.

**Returns:**
int - DateFormat değerinin bir değeri.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


DaysPerMonth değerini alır.

**Returns:**
int - DaysPerMonth değerinin bir değeri.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


DefaultFinishTime değerini alır.

**Returns:**
java.util.Date - DefaultFinishTime değerinin bir değeri.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


DefaultFixedCostAccrual değerini alır.

**Returns:**
int - DefaultFixedCostAccrual değerinin bir değeri.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


DefaultOvertimeRate değerini alır.

**Returns:**
double - DefaultOvertimeRate değerinin bir değeri.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


DefaultStandardRate değerini alır.

**Returns:**
double - DefaultStandardRate değerinin bir değeri.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


DefaultStartTime değerini alır.

**Returns:**
java.util.Date - DefaultStartTime değerinin bir değeri.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


DefaultTaskEVMethod değerini alır.

**Returns:**
int - DefaultTaskEVMethod değerinin bir değeri.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


DefaultTaskType değerini alır.

**Returns:**
int - DefaultTaskType değerinin bir değeri.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Projenin varsayılan görünümünü alır.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Projede varsayılan hafta çalışma günleri ve çalışma saatlerini temsil eden [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) sınıfının örneğini alır.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Veri yalnızca mpp dosyalarında bulunur (xml'de değil).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) sınıfının bir örneğini alır.

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Projede ayarların [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) içinde tanımlanan varsayılan süre biçimi ve belirtilen birim sayısı ile [Duration](../../com.aspose.tasks/duration) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer. | double | belirtilen birim sayısı. |

--------------------

Bu yöntem, Project.DurationFormat ayarına bağlı olarak farklı süreler döndürdüğü için dikkatli kullanılmalıdır. Örneğin, Project.DurationFormat TimeUnitType.Hour olduğunda GetWork(1.0) 1 saat, Project.DurationFormat TimeUnitType.Day olduğunda ise 1 gün döndürür. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Belirtilen sayıda [TimeUnitType](../../com.aspose.tasks/timeunittype) birimiyle [Duration](../../com.aspose.tasks/duration) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer. | double | belirtilen birim sayısı. |
| timeUnit | byte | belirtilen TimeUnitType değeri. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


DurationFormat değerini alır.

**Returns:**
byte - DurationFormat değerinin bir değeri.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


EarnedValueMethod değerini alır.

**Returns:**
int - EarnedValueMethod değerinin bir değeri.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


ExtendedAttributeDefinitionCollection nesnesini alır. Bir projeyle ilişkili genişletilmiş öznitelik (özel alanlar) tanımlarının koleksiyonu.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


ExtendedCreationDate değerini alır.

**Returns:**
java.util.Date - ExtendedCreationDate değerinin bir değeri.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


FinishDate değerini alır.

**Returns:**
java.util.Date - FinishDate değerinin bir değeri.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


FiscalYearStart'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


FyStartDate değerini alır.

**Returns:**
int - FyStartDate değerinin bir değeri.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Projenin küreselleştirme (dile özgü) ayarlarını alır.

Önerilen yöntem, proje boyunca kültürden bağımsız sabit değerler veya biçimler kullanmaktır. Ancak, bir proje kültüre özgü sabit değerler kullanıyorsa, bu sınıf hesaplama motorunun bu sabit değerleri ayrıştırmasına yardımcı olmak için kullanılabilir.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Guid değerini alır.

**Returns:**
java.util.UUID - Guid değerinin bir değeri.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


HonorConstraints'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


HyperlinkBase değerini alır.

**Returns:**
java.lang.String - HyperlinkBase değerinin bir değeri.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


InsertedProjectsLikeSummary'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Keywords değerini alır.

**Returns:**
java.lang.String - Keywords değerinin bir değeri.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


LastAuthor değerini alır.

**Returns:**
java.lang.String - LastAuthor değerinin bir değeri.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


LastPrinted değerini alır.

**Returns:**
java.util.Date - LastPrinted değerinin bir değeri.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


LastSaved değerini alır.

**Returns:**
java.util.Date - LastSaved değerinin bir değeri.
### getManager() {#getManager--}
```
public final String getManager()
```


Manager değerini alır.

**Returns:**
java.lang.String - Manager değerinin bir değeri.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


MicrosoftProjectServerURL'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


MinutesPerDay değerini alır.

**Returns:**
int - MinutesPerDay değerinin.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


MinutesPerWeek değerini alır.

**Returns:**
int - MinutesPerWeek değerinin.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


MoveCompletedEndsBack'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


MoveCompletedEndsForward'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


MoveRemainingStartsBack'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


MoveRemainingStartsForward'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


MultipleCriticalPaths'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Name değerini alır.

**Returns:**
java.lang.String - Name'in bir değeri.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


NewTaskStartDate değerini alır.

**Returns:**
int - NewTaskStartDate değerinin.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


NewTasksAreManual'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


NewTasksEffortDriven'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


NewTasksEstimated'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Bu proje dosyasına bağlanmış veya gömülmüş [OleObject](../../com.aspose.tasks/oleobject) sınıfının örneklerini içeren bir koleksiyon alır.

--------------------

Yalnızca mpp dosya formatı için kullanılabilir. Bu koleksiyon, 'Clear' işlemi dışında yalnızca okunabilir.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


OutlineCodeDefinitionCollection nesnesini alır. Bir proje ile ilişkili outline kod tanımlarının koleksiyonu.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Varsayılan [Timescale](../../com.aspose.tasks/timescale)(Gün) kullanılarak işlenecek proje için sayfa sayısını döndürür.

**Returns:**
int - Oluşturulacak sayfa sayısı.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Verilen [SaveOptions](../../com.aspose.tasks/saveoptions) kullanılarak işlenecek proje için sayfa sayısını döndürür.

--------------------

&gt; ```
&gt; Bu örnekte HtmlSaveOptions örneği ve oluşan HTML'deki sayfa sayısı konsola yazdırılır.
&gt; ``````

  [C#]
Project project = new Project(@\"test.mpp\");
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

