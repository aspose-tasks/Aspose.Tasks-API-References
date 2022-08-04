---
title: Project
second_title: Aspose.Tasks for .NET API Referansı
description: Bir projeyi temsil eder.
type: docs
weight: 1180
url: /tr/net/aspose.tasks/project/
---
## Project class

Bir projeyi temsil eder.

```csharp
public class Project
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Project](project#constructor)() | Yeni bir örneğini başlatır[`Project`](../project) sınıf. |
| [Project](project#constructor_1)(DbSettings) | Yeni bir örneğini başlatır[`Project`](../project) örneği tarafından belirtilen bir veritabanından veri okumak için sınıf[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) sınıf. |
| [Project](project#constructor_2)(Stream) | Yeni bir örneğini başlatır[`Project`](../project) bir akıştan sınıf. |
| [Project](project#constructor_9)(StreamReader) | Yeni bir örneğini başlatır[`Project`](../project) bir StreamReader örneğinden sınıf. |
| [Project](project#constructor_10)(string) | Yeni bir örneğini başlatır[`Project`](../project) bir şablondan sınıf (mevcut mpp veya mpt dosyası). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Yeni bir örneğini başlatır[`Project`](../project) belirtilen örneği ile Stream sınıfından[`LoadOptions`](../loadoptions) sınıf. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Yeni bir örneğini başlatır[`Project`](../project) bir şablondan sınıf (mevcut mpp veya mpt dosyası). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Yeni bir örneğini başlatır[`Project`](../project) belirtilen örneği ile Stream sınıfından[`PrimaveraReadOptions`](../primaverareadoptions) sınıf. |
| [Project](project#constructor_8)(Stream, string) | Yeni bir örneğini başlatır[`Project`](../project) bir şablondan sınıf (mevcut mpp veya mpt dosyası). |
| [Project](project#constructor_11)(string, LoadOptions) | Yeni bir örneğini başlatır[`Project`](../project) belirtilen örnekle birlikte bir şablondan (mevcut mpp veya mpt dosyası) sınıfı[`LoadOptions`](../loadoptions) sınıf. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Yeni bir örneğini başlatır[`Project`](../project) bir şablondan sınıf (mevcut mpp veya mpt dosyası). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Yeni bir örneğini başlatır[`Project`](../project) belirtilen örnekle birlikte bir şablondan (mevcut MPP veya MPT dosyası) sınıfı[`PrimaveraReadOptions`](../primaverareadoptions) sınıf. |
| [Project](project#constructor_16)(string, string) | Yeni bir örneğini başlatır[`Project`](../project) parola korumalı bir şablondan sınıf (mevcut mpp veya mpt dosyası). |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Projenin yerleşik özellikler koleksiyonunu alır. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Bir projenin hesaplama modunu alır veya ayarlar. Değerlerinden biri olabilir[`CalculationMode`](./calculationmode) numaralandırma. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Alır[`CalendarCollection`](../calendarcollection) bu Proje örneğinin nesnesi. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Bu projenin Kritik Yolunu oluşturan Kritik görevlerin bir listesini içeren bir koleksiyon alır. Bu, n'nin projedeki görev sayısı olduğu bir O(n) işlemidir. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Projenin özel özellikler koleksiyonunu alır. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Projenin varsayılan görünümünü alır veya ayarlar. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Örneğini alır[`WeekDayCollection`](../weekdaycollection) proje varsayılan hafta çalışma günleri ve çalışma sürelerinin bir koleksiyonunu temsil eden sınıf. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Şunun bir örneğini alır:[`ProjectDisplayOptions`](../projectdisplayoptions) sınıf. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | ExtendedAttributeDefinitionCollection nesnesini alır. Bir projeyle ilişkili genişletilmiş öznitelik (özel alanlar) tanımları koleksiyonu. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Örneklerini içeren bir koleksiyon alır.[`OleObject`](../oleobject) bu proje dosyasına bağlı veya gömülü sınıf. Yalnızca mpp dosya biçimi için kullanılabilir. Bu koleksiyon, 'Clear' işlemi dışında salt okunurdur. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | OutlineCodeDefinitionCollection nesnesini alır. Bir projeyle ilişkili anahat kodu tanımları koleksiyonu. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | ResourceAssignmentCollection nesnesini alır. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Tüm kaynak tabanlı filtre tanımlarını alır. ResourceFilters bir koleksiyondur[`Filter`](../filter) nesneler. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Tüm kaynak tabanlı grup tanımlarını alır. ResourceGroups bir koleksiyondur[`Group`](../group) nesneler. |
| [Resources](../../aspose.tasks/project/resources) { get; } | ResourceCollection nesnesini alır. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Görev ağacının kökünü alır. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Şunların bir listesini alır:[`Table`](../table) nesneler. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Tüm görev tabanlı filtre tanımlarını alır. TaskFilters bir koleksiyondur[`Filter`](../filter) nesneler. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Tüm görev tabanlı grup tanımlarını alır. TaskGroups, aşağıdakilerin bir koleksiyonudur:[`Group`](../group) nesneler. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Alır[`TaskLinkCollection`](../tasklinkcollection) nesne. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Bir örneğini alır[`VbaProject`](./vbaproject) sınıf. |
| [Views](../../aspose.tasks/project/views) { get; } | Şunların bir listesini alır:[`View`](../view) nesneler. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Proje için ÇÇY Kodu Tanımını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Kök görev de dahil olmak üzere tüm projenin görevlerini yinelemeli olarak sıralar. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Özelliğin bu kapsayıcıda eşlendiği değeri döndürür. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Temel kaydetme süresini döndürür. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Alır[`Duration`](../duration) proje ayarlarında tanımlanan, belirtilen birim sayısı ve varsayılan süre biçimine sahip nesne[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Alır[`Duration`](../duration) belirtilen sayıda nesne[`TimeUnitType`](../timeunittype) birimler. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Alır[`Duration`](../duration) belirtilen nesneTimeSpan değer ve belirtilen[`TimeUnitType`](../timeunittype) değer. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Varsayılan kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) (Gün). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Varsayılan kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) (Günler) ve verilen[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) ve[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) ve[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) ve tarih aralığı. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Belirtilen görevin öncülleri olan bir görev bağlantıları koleksiyonu döndürür. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Alır[`Duration`](../duration) belirtilen nesneDouble değer ve varsayılan çalışma biçimi. |
| [Print](../../aspose.tasks/project/print#print)() | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak projeyi varsayılan yazıcı ayarlarıyla varsayılan yazıcıya yazdırır. |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak projeyi belirtilen yazıcı ayarlarına göre yazdırır. |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak varsayılan yazıcı ayarları ve özel kaydetme seçenekleriyle projeyi varsayılan yazıcıya yazdırır. |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak varsayılan yazıcı ayarlarıyla projeyi belirtilen yazıcıya yazdırır. |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak projeyi belirtilen yazıcı ayarlarına ve özel kaydetme seçeneklerine göre yazdırır. |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak projeyi belirtilen yazıcı ayarlarına göre yazdırır. |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Projeyi belirtilen yazıcı ayarlarına, özel kaydetme seçeneklerine ve standart (Kullanıcı Arayüzü yok) yazdırma denetleyicisini kullanarak belirtilen belge adına göre yazdırır. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Tüm proje görev kimliklerini, anahat düzeylerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihleri ayarlar, bollukları, çalışma ve maliyet alanlarını hesaplar. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Tüm proje görev kimliklerini, anahat düzeylerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihleri ayarlar, isteğe bağlı doğrulama ile bollukları, iş ve maliyet alanlarını hesaplar. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Kaynakların Kimliğini, Başlangıç ve Bitişini yeniden hesaplar. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Kaynakların Başlangıç ve Bitişini yeniden hesaplar. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Proje kaynak atamaları listesinden geçersiz kaynak atamalarını ortadan kaldırır. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Tüm görevlerin ÇÇY kodunu yeniden numaralandırın. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Geçilen görevlerin ÇÇY kodunu yeniden numaralandırın. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Tamamlanmamış proje çalışmasını belirli bir tarihten sonra başlayacak şekilde yeniden planlar. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Belirli bir görev listesi için tamamlanmamış işleri, belirli bir tarihten sonra başlayacak şekilde yeniden planlar. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Proje verilerini mpp formatında dosyaya kaydeder. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak projeyi bir akışa kaydeder. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Proje verilerini akışa kaydeder. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak projeyi bir akışa kaydeder. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak belgeyi mpp dosya biçiminde kaydeder. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Proje verilerini dosyaya kaydeder. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak belgeyi bir dosyaya kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Projeyi şablon olarak belirtilen bir akışa kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Projeyi şablon olarak belirtilen dosya yoluna kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Projeyi şablon olarak belirtilen bir akışa kaydeder. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Projeyi şablon olarak kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Projeye genel bakış raporunu akışa kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Projeye genel bakış raporunu PDF dosyasına kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Belirtilen türdeki proje raporunu belirtilen akışa kaydeder. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Belirtilen türdeki proje raporunu PDF biçiminde belirtilen dosya yoluna kaydeder. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Kök görevin tüm alt görevlerini yinelemeli olarak toplar. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Belirtilen özelliği, bu kapsayıcıda belirtilen değerle eşler. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Belirtilen özelliği, bu kapsayıcıda belirtilen değerle eşler. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Tüm proje için temel alanları belirtilen temele kaydeder. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Seçili görevler için temel alanları belirtilen taban çizgisine kaydeder. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Temel kaydetme süresini ayarlar. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Tüm çalışmaları, tüm proje için belirtilen bir tarihe kadar eksiksiz olarak günceller. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Belirtilen görev listesi için belirtilen bir tarihe kadar tüm çalışmaları eksiksiz olarak günceller. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Akıştan proje dosyası bilgilerini alır. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Dosyadan proje dosyası bilgilerini okuyun. |

### Notlar

bu **Proje** Aspose.Tasks kitaplığındaki merkezi bir sınıftır.

Kullanılabilir **Proje** desteklenen proje yönetimi biçimlerinden birini okumak için: MPP, MPT, MPX, XML.

Mevcut bir belgeyi desteklenen biçimlerden herhangi birinde yüklemek için, aşağıdakilerden birine bir dosya adı veya bir akış iletin. **Proje** yapıcılar. Boş bir proje oluşturmak için parametresiz kurucuyu çağırın.

Projeyi aşağıdakilerden herhangi birine kaydetmek için Save yöntemi aşırı yüklemelerinden birini kullanın.[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) biçimler: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Sabit Düzen: PDF; Görüntüler: JPEG, PNG, BMP, TIFF, SVG; Metin: TXT; Diğerleri: HTML.

Projeyi yazdırmak için aşağıdakilerden birini kullanın:[`Print`](./print) yöntem aşırı yüklemeleri.

bu **Proje** gibi proje çapındaki bilgileri depolar.[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , ve[`ExtendedAttributes`](./extendedattributes) . Bu nesnelerin çoğuna, ilgili nesnenin ilgili özellikleri aracılığıyla erişilebilir. **Proje** sınıf.

bu **Proje** gibi diğer proje varlıklarını işlemek için giriş noktaları içeren bir kök varlıktır.[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) ve[`Calendar`](../calendar).

**Proje** varlıklara, örneğin yazılan koleksiyonlar aracılığıyla erişilebilir[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , vb.

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
