---
title: "Aspose::Tasks::Project sınıfı"
linktitle: "Project"
articleTitle: "Project"
second_title: "C++ için Aspose.Tasks"
description: "Bir projeyi temsil eder."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/project/
---

## Project class

Bir projeyi temsil eder.

Project, Aspose.Tasks kütüphanesindeki merkezi bir sınıftır.

Project'i, desteklenen proje yönetimi formatlarından birini (MPP, MPT, MPX, XML) okumak için kullanabilirsiniz.

Desteklenen formatlardan herhangi birinde mevcut bir belgeyi yüklemek için bir dosya adı veya akışı Project yapıcılarından birine aktarın. Boş bir proje oluşturmak için parametresiz yapıcıyı çağırın.

Projeyi, Aspose::Tasks::Saving::SaveFileFormat formatlarından herhangi birinde kaydetmek için Save yöntemi aşırı yüklemelerinden birini kullanın: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Sabit Düzen: PDF; Görseller: JPEG, PNG, BMP, TIFF, SVG; Metin: TXT; Diğerleri: HTML.

Project, Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps ve Aspose::Tasks::Project::ExtendedAttributes gibi proje genelindeki bilgileri depolar. Bu nesnelerin çoğu, Project sınıfının ilgili özellikleri aracılığıyla erişilebilir.

Project, diğer proje varlıklarını manipüle etmek için giriş noktaları içeren bir kök varlıktır, örneğin Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute ve Aspose::Tasks::Calendar.

Project varlıklarına tiplenmiş koleksiyonlar aracılığıyla erişilebilir, örneğin Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments vb.

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Project (13 overloads)](./project/) | Project sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Kök görevi dahil olmak üzere projenin tüm görevlerini özyinelemeli olarak listeler. |
| [Get](./get/) | Bu konteynerde özelliğin eşlendiği değeri döndürür. |
| [get_ActualsInSync](./get_actualsinsync/) | ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_AdminProject](./get_adminproject/) | AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | AreEditableActualCosts'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_Author](./get_author/) | Author değerini alır. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Atama maliyetinin ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır. |
| [get_Autolink](./get_autolink/) | Autolink'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | BaselineForEarnedValue değerini alır. |
| [get_BuiltInProps](./get_builtinprops/) | Projenin yerleşik özellikler koleksiyonunu alır. |
| [get_CalculationMode](./get_calculationmode/) | Bir projenin hesaplama modunu alır. CalculationMode enum'ının değerlerinden biri olabilir. |
| [get_Calendar](./get_calendar/) | Calendar değerini alır. |
| [get_Calendars](./get_calendars/) | Bu Project örneğinin CalendarCollection nesnesini alır. |
| [get_Category](./get_category/) | Category değerini alır. |
| [get_Comments](./get_comments/) | Comments değerini alır. |
| [get_Company](./get_company/) | Company değerini alır. |
| [get_CreationDate](./get_creationdate/) | CreationDate değerini alır. |
| [get_CriticalPath](./get_criticalpath/) | Bu projenin Kritik Yolunu oluşturan Kritik görevlerin bir listesini içeren bir koleksiyon alır. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | CriticalSlackLimit değerini alır. |
| [get_CurrencyCode](./get_currencycode/) | CurrencyCode değerini alır. |
| [get_CurrencyDigits](./get_currencydigits/) | CurrencyDigits değerini alır. |
| [get_CurrencySymbol](./get_currencysymbol/) | CurrencySymbol değerini alır. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | CurrencySymbolPosition değerini alır. |
| [get_CurrentDate](./get_currentdate/) | CurrentDate değerini alır. |
| [get_CustomDateFormat](./get_customdateformat/) | CustomDateFormat değerini alır. |
| [get_CustomProps](./get_customprops/) | Projenin özel özellikler koleksiyonunu alır. |
| [get_DateFormat](./get_dateformat/) | DateFormat değerini alır. |
| [get_DaysPerMonth](./get_dayspermonth/) | DaysPerMonth değerini alır. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | DefaultFinishTime değerini alır. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | DefaultFixedCostAccrual değerini alır. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | DefaultOvertimeRate değerini alır. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | DefaultStandardRate değerini alır. |
| [get_DefaultStartTime](./get_defaultstarttime/) | DefaultStartTime değerini alır. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | DefaultTaskEVMethod değerini alır. |
| [get_DefaultTaskType](./get_defaulttasktype/) | DefaultTaskType değerini alır. |
| [get_DefaultView](./get_defaultview/) | Projenin varsayılan görünümünü alır. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Projenin varsayılan hafta çalışma günleri ve çalışma saatlerini temsil eden WeekDayCollection sınıfının örneğini alır. |
| [get_DisplayOptions](./get_displayoptions/) | ProjectDisplayOptions sınıfının bir örneğini alır. |
| [get_DurationFormat](./get_durationformat/) | DurationFormat değerini alır. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod değerini alır. |
| [get_ExtendedAttributes](./get_extendedattributes/) | ExtendedAttributeDefinitionCollection nesnesini alır. Proje ile ilişkili genişletilmiş öznitelik (özel alan) tanımlarının koleksiyonu. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | ExtendedCreationDate değerini alır. |
| [get_FinishDate](./get_finishdate/) | FinishDate değerini alır. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | FiscalYearStart ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [get_FyStartDate](./get_fystartdate/) | FyStartDate değerini alır. |
| [get_Guid](./get_guid/) | Guid değerini alır. |
| [get_HonorConstraints](./get_honorconstraints/) | HonorConstraints ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | HyperlinkBase değerini alır. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | InsertedProjectsLikeSummary ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_Keywords](./get_keywords/) | Keywords değerini alır. |
| [get_LastAuthor](./get_lastauthor/) | LastAuthor değerini alır. |
| [get_LastPrinted](./get_lastprinted/) | LastPrinted değerini alır. |
| [get_LastSaved](./get_lastsaved/) | LastSaved değerini alır. |
| [get_Manager](./get_manager/) | Manager değerini alır. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | MicrosoftProjectServerURL ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_MinutesPerDay](./get_minutesperday/) | MinutesPerDay değerini alır. |
| [get_MinutesPerWeek](./get_minutesperweek/) | MinutesPerWeek değerini alır. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | MoveCompletedEndsBack ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | MoveCompletedEndsForward ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | MoveRemainingStartsBack ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | MoveRemainingStartsForward ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | MultipleCriticalPaths ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_Name](./get_name/) | Name değerini alır. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | NewTasksAreManual ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | NewTasksEffortDriven ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | NewTasksEstimated ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | NewTaskStartDate değerini alır. |
| [get_OleObjects](./get_oleobjects/) | Bu proje dosyasına bağlı veya gömülü olan OleObject sınıfının örneklerini içeren bir koleksiyon alır. |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeDefinitionCollection nesnesini alır. Bir proje ile ilişkili outline kod tanımlarının koleksiyonu. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera dosyasından okunan bir proje için Primavera'ya özgü özellikleri içeren bir nesne alır. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | ProjectExternallyEdited ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_RemoveFileProperties](./get_removefileproperties/) | RemoveFileProperties ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [get_ResourceAssignments](./get_resourceassignments/) | ResourceAssignmentCollection nesnesini alır. |
| [get_ResourceFilters](./get_resourcefilters/) | Kaynak tabanlı tüm filtre tanımlarını alır. ResourceFilters, Filter nesnelerinden oluşan bir koleksiyondur. |
| [get_ResourceGroups](./get_resourcegroups/) | Kaynak tabanlı tüm grup tanımlarını alır. ResourceGroups, Group nesnelerinden oluşan bir koleksiyondur. |
| [get_Resources](./get_resources/) | ResourceCollection nesnesini alır. |
| [get_Revision](./get_revision/) | Revision değerini alır. |
| [get_RootTask](./get_roottask/) | Görev ağacının kökünü alır. |
| [get_SaveVersion](./get_saveversion/) | SaveVersion değerini alır. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | ScheduleFromStart ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | ShowProjectSummaryTask ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | SplitsInProgressTasks ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_SpreadActualCost](./get_spreadactualcost/) | SpreadActualCost ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | SpreadPercentComplete ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_StartDate](./get_startdate/) | StartDate değerini alır. |
| [get_StatusDate](./get_statusdate/) | StatusDate değerini alır. |
| [get_Subject](./get_subject/) | Subject değerini alır. |
| [get_Tables](./get_tables/) | Table nesnelerinin bir listesini alır. |
| [get_TaskFilters](./get_taskfilters/) | Görev tabanlı tüm filtre tanımlarını alır. TaskFilters, Filter nesnelerinden oluşan bir koleksiyondur. |
| [get_TaskGroups](./get_taskgroups/) | Görev tabanlı tüm grup tanımlarını alır. TaskGroups, Group nesnelerinden oluşan bir koleksiyondur. |
| [get_TaskLinks](./get_tasklinks/) | TaskLinkCollection nesnesini alır. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | TaskUpdatesResource ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_Template](./get_template/) | Template değerini alır. |
| [get_TimescaleFinish](./get_timescalefinish/) | TimescaleFinish değerini alır. |
| [get_TimescaleStart](./get_timescalestart/) | TimescaleStart değerini alır. |
| [get_Title](./get_title/) | Title değerini alır. |
| [get_Uid](./get_uid/) | Uid değerini alır. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [get_VbaProject](./get_vbaproject/) | VbaProject sınıfının bir örneğini alır. |
| [get_Views](./get_views/) | View nesnelerinin bir listesini alır. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Proje için WBS Kod Tanımını alır. |
| [get_WeekStartDay](./get_weekstartday/) | WeekStartDay değerini alır. |
| [get_WorkFormat](./get_workformat/) | WorkFormat değerini alır. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Temel kaydetme zamanını döndürür. |
| [GetDuration (3 overloads)](./getduration/) | Projenin ayarlarında Prj::DurationFormat ile tanımlanan varsayılan süre formatı ve belirtilen birim sayısı ile Duration nesnesini alır. |
| [GetPageCount (7 overloads)](./getpagecount/) | Varsayılan Timescale (Gün) kullanılarak render edilecek projenin sayfa sayısını döndürür. |
| [GetPredecessors](./getpredecessors/) | Belirtilen görevin öncülleri olan görev bağlantılarının bir koleksiyonunu döndürür. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Akıştan proje dosyası bilgilerini alır. |
| [GetWork](./getwork/) | Belirtilen çift değer ve varsayılan iş formatı ile Duration nesnesini alır. |
| [Recalculate (2 overloads)](./recalculate/) | Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden zamanlar, erken/geç tarihlerini ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Kaynakların Id, Başlangıç ve Bitiş değerlerini yeniden hesaplar. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Kaynakların Başlangıç ve Bitiş değerlerini yeniden hesaplar. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Proje kaynak atama listesinden geçersiz kaynak atamalarını ortadan kaldırır. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Tüm görevlerin WBS kodunu yeniden numaralar. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Tamamlanmamış proje çalışmasını belirtilen tarihten sonra başlayacak şekilde yeniden zamanlar. |
| [Save (5 overloads)](./save/) | Belirtilen kaydetme seçeneklerini kullanarak projeyi bir akışa kaydeder. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Projeyi bir şablon olarak belirtilen akışa kaydeder. |
| [SaveReport (4 overloads)](./savereport/) | Proje genel bakış raporunu akışa kaydeder. |
| [SelectAllChildTasks](./selectallchildtasks/) | Kök görevin tüm alt görevlerini yinelemeli olarak toplar. |
| [Set (2 overloads)](./set/) | Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler. |
| [set_ActualsInSync](./set_actualsinsync/) | ActualsInSync'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_AdminProject](./set_adminproject/) | AdminProject'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | AreEditableActualCosts'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_Author](./set_author/) | Author değerini ayarlar. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını ayarlar. |
| [set_Autolink](./set_autolink/) | Autolink'in ayarlanıp ayarlanmadığını gösteren bir değeri ayarlar. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | BaselineForEarnedValue değerini ayarlar. |
| [set_CalculationMode](./set_calculationmode/) | Bir projenin hesaplama modunu ayarlar. CalculationMode sayımının değerlerinden biri olabilir. |
| [set_Calendar](./set_calendar/) | Calendar değerini ayarlar . |
| [set_Category](./set_category/) | Category değerini ayarlar. |
| [set_Comments](./set_comments/) | Comments değerini ayarlar. |
| [set_Company](./set_company/) | Company değerini ayarlar. |
| [set_CreationDate](./set_creationdate/) | CreationDate değerini ayarlar. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | CriticalSlackLimit değerini ayarlar. |
| [set_CurrencyCode](./set_currencycode/) | CurrencyCode değerini ayarlar. |
| [set_CurrencyDigits](./set_currencydigits/) | CurrencyDigits değerini ayarlar. |
| [set_CurrencySymbol](./set_currencysymbol/) | CurrencySymbol değerini ayarlar. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | CurrencySymbolPosition değerini ayarlar. |
| [set_CurrentDate](./set_currentdate/) | CurrentDate değerini ayarlar. |
| [set_CustomDateFormat](./set_customdateformat/) | CustomDateFormat değerini ayarlar. |
| [set_DateFormat](./set_dateformat/) | DateFormat değerini ayarlar. |
| [set_DaysPerMonth](./set_dayspermonth/) | DaysPerMonth değerini ayarlar. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | DefaultFinishTime değerini ayarlar. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | DefaultFixedCostAccrual değerini ayarlar. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | DefaultOvertimeRate değerini ayarlar. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | DefaultStandardRate değerini ayarlar. |
| [set_DefaultStartTime](./set_defaultstarttime/) | DefaultStartTime değerini ayarlar. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | DefaultTaskEVMethod değerini ayarlar. |
| [set_DefaultTaskType](./set_defaulttasktype/) | DefaultTaskType değerini ayarlar. |
| [set_DefaultView](./set_defaultview/) | Projenin varsayılan görünümünü ayarlar. |
| [set_DurationFormat](./set_durationformat/) | DurationFormat değerini ayarlar. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod değerini ayarlar. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | ExtendedCreationDate değerini ayarlar. |
| [set_FinishDate](./set_finishdate/) | FinishDate değerini ayarlar. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | FiscalYearStart'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_FyStartDate](./set_fystartdate/) | FyStartDate değerini ayarlar. |
| [set_Guid](./set_guid/) | Guid değerini ayarlar. |
| [set_HonorConstraints](./set_honorconstraints/) | HonorConstraints'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | HyperlinkBase değerini ayarlar. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | InsertedProjectsLikeSummary'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_Keywords](./set_keywords/) | Keywords değerini ayarlar. |
| [set_LastAuthor](./set_lastauthor/) | LastAuthor değerini ayarlar. |
| [set_LastPrinted](./set_lastprinted/) | LastPrinted değerini ayarlar. |
| [set_LastSaved](./set_lastsaved/) | LastSaved değerini ayarlar. |
| [set_Manager](./set_manager/) | Manager değerini ayarlar. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | MicrosoftProjectServerURL'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_MinutesPerDay](./set_minutesperday/) | MinutesPerDay değerini ayarlar. |
| [set_MinutesPerWeek](./set_minutesperweek/) | MinutesPerWeek değerini ayarlar. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | MoveCompletedEndsBack'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | MoveCompletedEndsForward'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | MoveRemainingStartsBack'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | MoveRemainingStartsForward'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | MultipleCriticalPaths'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_Name](./set_name/) | Name değerini ayarlar. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | NewTasksAreManual'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | NewTasksEffortDriven'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | NewTasksEstimated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | NewTaskStartDate değerini ayarlar. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | ProjectExternallyEdited'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_RemoveFileProperties](./set_removefileproperties/) | RemoveFileProperties'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_Revision](./set_revision/) | Revision değerini ayarlar. |
| [set_SaveVersion](./set_saveversion/) | SaveVersion değerini ayarlar. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | ScheduleFromStart'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | ShowProjectSummaryTask'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | SplitsInProgressTasks'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_SpreadActualCost](./set_spreadactualcost/) | SpreadActualCost'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | SpreadPercentComplete'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_StartDate](./set_startdate/) | StartDate değerini ayarlar. |
| [set_StatusDate](./set_statusdate/) | StatusDate değerini ayarlar. |
| [set_Subject](./set_subject/) | Subject değerini ayarlar. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | TaskUpdatesResource'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_Template](./set_template/) | Template değerini ayarlar. |
| [set_TimescaleFinish](./set_timescalefinish/) | TimescaleFinish değerini ayarlar. |
| [set_TimescaleStart](./set_timescalestart/) | TimescaleStart değerini ayarlar. |
| [set_Title](./set_title/) | Title değerini ayarlar. |
| [set_Uid](./set_uid/) | Uid değerini ayarlar. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Proje için WBS Kod Tanımını ayarlar. |
| [set_WeekStartDay](./set_weekstartday/) | WeekStartDay değerini ayarlar. |
| [set_WorkFormat](./set_workformat/) | WorkFormat değerini ayarlar. |
| [SetBaseline (2 overloads)](./setbaseline/) | Tüm proje için belirtilen temel çizgiye temel alan alanları kaydeder. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Temel çizgi kaydetme zamanını ayarlar. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Belirtilen tarih itibarıyla tüm işi tamamlanmış olarak günceller ve tüm proje için. |

