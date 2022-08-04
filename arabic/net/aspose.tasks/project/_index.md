---
title: Project
second_title: Aspose.Tasks لمرجع .NET API
description: يمثل مشروعًا .
type: docs
weight: 1180
url: /ar/net/aspose.tasks/project/
---
## Project class

يمثل مشروعًا .

```csharp
public class Project
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Project](project#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة . |
| [Project](project#constructor_1)(DbSettings) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة لقراءة البيانات من قاعدة البيانات التي تم تحديدها بواسطة مثيل[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) فئة . |
| [Project](project#constructor_2)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من تيار . |
| [Project](project#constructor_9)(StreamReader) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من مثيل StreamReader. |
| [Project](project#constructor_10)(string) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف mpp أو mpt موجود) . |
| [Project](project#constructor_3)(Stream, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من Stream مع المثيل المحدد لملف[`LoadOptions`](../loadoptions) فئة . |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف mpp أو mpt موجود) . |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من Stream مع المثيل المحدد لملف[`PrimaveraReadOptions`](../primaverareadoptions) فئة . |
| [Project](project#constructor_8)(Stream, string) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف mpp أو mpt موجود) . |
| [Project](project#constructor_11)(string, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف mpp أو mpt موجود) مع المثيل المحدد لملف[`LoadOptions`](../loadoptions) فئة . |
| [Project](project#constructor_12)(string, ParseErrorCallback) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف mpp أو mpt موجود) . |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب (ملف MPP أو MPT موجود) مع المثيل المحدد لملف[`PrimaveraReadOptions`](../primaverareadoptions) فئة . |
| [Project](project#constructor_16)(string, string) | يقوم بتهيئة مثيل جديد لملف[`Project`](../project) فئة من قالب محمي بكلمة مرور (ملف mpp أو mpt موجود) . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | الحصول على مجموعة الخصائص المضمنة في المشروع. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | الحصول على أو تعيين وضع الحساب لمشروع . يمكن أن تكون إحدى قيم[`CalculationMode`](./calculationmode) التعداد . |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | يحصل[`CalendarCollection`](../calendarcollection) كائن مثيل المشروع هذا. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | الحصول على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع.هذه عملية O (n) ، حيث n هو عدد المهام في المشروع. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | الحصول على مجموعة الخصائص المخصصة للمشروع. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | الحصول على العرض الافتراضي للمشروع أو تعيينه. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | يحصل على مثيل[`WeekDayCollection`](../weekdaycollection) فئة تمثل مجموعة من أيام العمل الأسبوعية وأوقات العمل الافتراضية للمشروع. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | يحصل على مثيل لملف[`ProjectDisplayOptions`](../projectdisplayoptions) فئة . |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | الحصول على كائن ExtendedAttributeDefinitionCollection. مجموعة تعريفات السمات الموسعة (الحقول المخصصة) المرتبطة بمشروع. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | يحصل على مجموعة تحتوي على مثيلات[`OleObject`](../oleobject) فئة مرتبطة أو مضمنة في ملف المشروع هذا.متاح لتنسيق ملف mpp فقط. هذه المجموعة للقراءة فقط باستثناء عملية "مسح". |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | الحصول على كائن OutlineCodeDefinitionCollection . مجموعة تعريفات كود المخطط التفصيلي المرتبطة بمشروع. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | يحصل على كائن ResourceAssignmentCollection . |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | يحصل على كافة تعريفات عامل التصفية المستندة إلى الموارد. ResourceFilters هي مجموعة من[`Filter`](../filter) الكائنات . |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | يحصل على كافة تعريفات المجموعة المستندة إلى الموارد. ResourceGroups هي مجموعة من[`Group`](../group) الكائنات . |
| [Resources](../../aspose.tasks/project/resources) { get; } | الحصول على كائن ResourceCollection . |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | الحصول على جذر شجرة المهام. |
| [Tables](../../aspose.tasks/project/tables) { get; } | يحصل على قائمة[`Table`](../table) الكائنات . |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | يحصل على كافة تعريفات عوامل التصفية المستندة إلى المهام. TaskFilters عبارة عن مجموعة من ملفات[`Filter`](../filter) الكائنات . |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | يحصل على كافة تعريفات المجموعة المستندة إلى المهام. TaskGroups هي مجموعة من[`Group`](../group) الكائنات . |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | يحصل[`TaskLinkCollection`](../tasklinkcollection) الكائن . |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | الحصول على مثيل لـ[`VbaProject`](./vbaproject) فئة . |
| [Views](../../aspose.tasks/project/views) { get; } | يحصل على قائمة[`View`](../view) الكائنات . |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | الحصول على تعريف رمز WBS للمشروع أو تعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | نسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | نسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | يعدّد بشكل متكرر جميع مهام المشروع بما في ذلك مهمة الجذر. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | إرجاع القيمة التي تم تعيين الخاصية لها في هذه الحاوية. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | إرجاع وقت توفير الأساس . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | يحصل[`Duration`](../duration) مع العدد المحدد من الوحدات وتنسيق المدة الافتراضي المحدد في إعدادات المشروع[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | يحصل[`Duration`](../duration) بالرقم المحدد من[`TimeUnitType`](../timeunittype) الوحدات . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | يحصل[`Duration`](../duration) كائن مع المحددTimeSpan القيمة والمحددة[`TimeUnitType`](../timeunittype) القيمة . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام الافتراضي[`Timescale`](../../aspose.tasks.visualization/timescale) (أيام) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام الافتراضي[`Timescale`](../../aspose.tasks.visualization/timescale) (أيام) ومعطاء[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../aspose.tasks.visualization/timescale) و[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../aspose.tasks.visualization/timescale) و[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../aspose.tasks.visualization/timescale) و[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) ونطاق التاريخ. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | إرجاع مجموعة من ارتباطات المهام التي سبقت المهمة المحددة. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | يحصل[`Duration`](../duration) كائن مع المحددDouble القيمة وتنسيق العمل الافتراضي. |
| [Print](../../aspose.tasks/project/print#print)() | يطبع المشروع على الطابعة الافتراضية بإعدادات الطابعة الافتراضية باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | طباعة المشروع وفقًا لإعدادات الطابعة المحددة باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | يطبع المشروع على الطابعة الافتراضية بإعدادات الطابعة الافتراضية وخيارات الحفظ المخصصة باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | طباعة المشروع على الطابعة المحددة بإعدادات الطابعة الافتراضية باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | طباعة المشروع وفقًا لإعدادات الطابعة المحددة وخيارات الحفظ المخصصة باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | طباعة المشروع وفقًا لإعدادات الطابعة المحددة باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | طباعة المشروع وفقًا لإعدادات الطابعة المحددة وخيارات الحفظ المخصصة واسم المستند المحدد باستخدام وحدة تحكم الطباعة القياسية (بدون واجهة مستخدم). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | إعادة جدولة جميع معرفات مهام المشروع ، ومستويات المخطط التفصيلي ، وتواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وحساب فترات الركود ، وحقول العمل والتكلفة. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | إعادة جدولة جميع معرفات مهام المشروع ، ومستويات المخطط التفصيلي ، وتواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وحساب فترات السماح وحقول العمل والتكلفة باستخدام التحقق الاختياري. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | يعيد حساب المعرف والبدء والانتهاء من الموارد. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | إعادة حساب بداية الموارد وإنهائها . |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | يزيل تعيينات الموارد غير الصالحة من قائمة تخصيصات موارد المشروع. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | إعادة ترقيم رمز WBS لجميع المهام. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | إعادة ترقيم رمز WBS للمهام التي تم تمريرها. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | إعادة جدولة عمل المشروع غير المكتمل للبدء بعد تاريخ محدد. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | إعادة جدولة العمل غير المكتمل لقائمة محددة من المهام للبدء بعد تاريخ محدد. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | يحفظ بيانات المشروع في ملف بتنسيق mpp . |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | يحفظ المشروع في دفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | يحفظ بيانات المشروع في التدفق . |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | يحفظ المشروع في دفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | يحفظ المستند بتنسيق ملف mpp باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | يحفظ بيانات المشروع في الملف. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | يحفظ المستند في ملف باستخدام خيارات الحفظ المحددة. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | يحفظ المشروع كقالب لتيار محدد. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | يحفظ المشروع كقالب في مسار الملف المحدد. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | يحفظ المشروع كقالب لتيار محدد. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | يحفظ المشروع كنموذج . |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | يحفظ تقرير النظرة العامة على المشروع في الدفق. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | يحفظ تقرير النظرة العامة على المشروع في ملف PDF . |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | يحفظ تقرير المشروع من النوع المحدد في الدفق المحدد. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | يحفظ تقرير المشروع من النوع المحدد بتنسيق PDF في مسار الملف المحدد. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | يقوم بتجميع كافة المهام الفرعية للمهمة الجذر بشكل متكرر. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | تعيين الخاصية المحددة إلى القيمة المحددة في هذه الحاوية. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | تعيين الخاصية المحددة إلى القيمة المحددة في هذه الحاوية. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | يحفظ حقول الأساس إلى خط الأساس المحدد للمشروع بأكمله. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | يحفظ الحقول الأساسية إلى خط الأساس المحدد للمهام المحددة. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | يحدد وقت التوفير الأساسي. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | يقوم بتحديث جميع الأعمال على أنها مكتملة خلال تاريخ محدد للمشروع بأكمله. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | يقوم بتحديث جميع الأعمال على أنها مكتملة خلال تاريخ محدد لقائمة المهام المحددة. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | يحصل على معلومات ملف المشروع من الدفق. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | اقرأ معلومات ملف المشروع من الملف . |

### ملاحظات

ال **مشروع** هي فئة مركزية في مكتبة Aspose.Tasks.

يمكن للمرء استخدامها **مشروع** لقراءة أحد تنسيقات إدارة المشروع المدعومة: MPP ، MPT ، MPX ، XML.

لتحميل مستند موجود بأي من التنسيقات المدعومة ، قم بتمرير اسم ملف أو دفق إلى أحد ملفات **مشروع** الصانعين. لإنشاء مشروع فارغ ، اتصل بالمُنشئ بدون معلمات.

استخدم أحد طرق الحفظ الزائد لحفظ المشروع في أي من ملفات[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) التنسيقات: Primavera: P6 XML ، PM XER ؛ Microsoft Excel: XLSX ، XML ؛ التخطيط الثابت: PDF ؛ الصور: JPEG ، PNG ، BMP ، TIFF ، SVG ؛ النص: TXT ؛ آخرون: HTML.

لطباعة المشروع ، استخدم أحد ملفات[`Print`](./print) طريقة الزائدة.

ال **مشروع** يخزن المعلومات على مستوى المشروع مثل[`Views`](./views) ، [`BuiltInProps`](./builtinprops) و[`CustomProps`](./customprops) ، و[`ExtendedAttributes`](./extendedattributes) . يمكن الوصول إلى معظم هذه الكائنات عبر الخصائص المقابلة لملف **مشروع** صف دراسي.

ال **مشروع** هو كيان جذري يحتوي على نقاط دخول للتعامل مع كيانات المشروع الأخرى ، مثل[`Task`](../task) و[`Resource`](../resource) و[`ResourceAssignment`](../resourceassignment) و[`ExtendedAttribute`](../extendedattribute) و[`Calendar`](../calendar).

ملف **مشروع** يمكن الوصول إلى الكيانات عبر المجموعات المكتوبة ، على سبيل المثال[`Children`](../task/children) و[`Resources`](./resources) و[`ResourceAssignments`](./resourceassignments) ، وما إلى ذلك

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks)
* المجسم [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
