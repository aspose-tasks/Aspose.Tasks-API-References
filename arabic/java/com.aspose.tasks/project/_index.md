---
title: "المشروع"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مشروعًا."
type: docs
weight: 220
url: /ar/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

يمثل مشروعًا.

--------------------

الـ **Project** هي فئة مركزية في مكتبة Aspose.Tasks.

يمكن استخدام **Project** لقراءة أحد صيغ إدارة المشاريع المدعومة: MPP، MPT، MPX، XML.

لتحميل مستند موجود بأي من الصيغ المدعومة، مرّر اسم ملف أو تدفق إلى أحد مُنشئات **Project**. لإنشاء مشروع فارغ، استدعِ المُنشئ بدون معلمات.

استخدم أحد تحميلات طريقة Save لحفظ المشروع بأي من صيغ [SaveFileFormat](../../com.aspose.tasks/savefileformat): Primavera: P6 XML، PM XER؛ Microsoft Excel: XLSX، XML؛ Fixed Layout: PDF؛ Images: JPEG، PNG، BMP، TIFF، SVG؛ Text: TXT؛ Others: HTML.

لطباعة المشروع، استخدم أحد تحميلات طريقة [print()](../../com.aspose.tasks/project\#print--).

يخزن **Project** معلومات على مستوى المشروع مثل `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), و `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). معظم هذه الكائنات يمكن الوصول إليها عبر الخصائص المقابلة لفئة **Project**.

الـ **Project** هو كيان جذري يحتوي على نقاط دخول للتعامل مع كيانات المشروع الأخرى، مثل [Task](../../com.aspose.tasks/task)، [Resource](../../com.aspose.tasks/resource)، [ResourceAssignment](../../com.aspose.tasks/resourceassignment)، [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) و [Calendar](../../com.aspose.tasks/calendar).

يمكن الوصول إلى كيانات **Project** عبر مجموعات ذات نوع، على سبيل المثال `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), إلخ.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Project()](#Project--) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) class. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب محمي بكلمة مرور (ملف mpp أو mpt موجود). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من الدفق مع المثيل المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من تدفق. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف MPP أو MPT موجود) مع المثيل المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) لقراءة البيانات من قاعدة بيانات يتم تحديدها بواسطة مثيل فئة [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود) مع المثيل المحدد لفئة [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من الدفق مع المثيل المحدد لفئة [LoadOptions](../../com.aspose.tasks/loadoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | يُعدد بشكل متكرر جميع مهام المشروع بما في ذلك المهمة الجذرية. |
| [getActualsInSync()](#getActualsInSync--) | يحصل على قيمة تشير إلى ما إذا كان ActualsInSync مُحددًا أم لا. |
| [getAdminProject()](#getAdminProject--) | يحصل على قيمة تشير إلى ما إذا كان AdminProject مُحددًا أم لا. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | يحصل على قيمة تشير إلى ما إذا كان AreEditableActualCosts مُحددًا أم لا. |
| [getAuthor()](#getAuthor--) | يحصل على قيمة Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | يحصل على قيمة تشير إلى ما إذا كان AutoAddNewResourcesAndTasks مُحددًا أم لا. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | يحصل على ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد. |
| [getAutolink()](#getAutolink--) | يحصل على قيمة تشير إلى ما إذا كان Autolink مُحددًا أم لا. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | يحصل على قيمة BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | يعيد وقت حفظ الخط الأساسي. |
| [getBuiltInProps()](#getBuiltInProps--) | يحصل على مجموعة الخصائص المدمجة للمشروع. |
| [getCalculationMode()](#getCalculationMode--) | يحصل على وضع الحساب للمشروع. |
| [getCalendar()](#getCalendar--) | يحصل على قيمة Calendar. |
| [getCalendars()](#getCalendars--) | يحصل على كائن [CalendarCollection](../../com.aspose.tasks/calendarcollection) لهذا المثيل من Project. |
| [getCategory()](#getCategory--) | يحصل على قيمة Category. |
| [getComments()](#getComments--) | يحصل على قيمة Comments. |
| [getCompany()](#getCompany--) | يحصل على قيمة Company. |
| [getCreationDate()](#getCreationDate--) | يحصل على قيمة CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | يحصل على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | تُعتبر المهام حرجة في MS Project إذا كان الفائض الكلي أقل أو يساوي هذا العدد من الأيام. |
| [getCurrencyCode()](#getCurrencyCode--) | يحصل على قيمة CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | يحصل على قيمة CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | يحصل على قيمة CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | يحصل على قيمة CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | يحصل على قيمة CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | يحصل على قيمة CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | يحصل على مجموعة الخصائص المخصصة للمشروع. |
| [getDateFormat()](#getDateFormat--) | يحصل على قيمة DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | يحصل على قيمة DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | يحصل على قيمة DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | يحصل على قيمة DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | يحصل على قيمة DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | يحصل على قيمة DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | يحصل على قيمة DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | يحصل على قيمة DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | يحصل على قيمة DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | يحصل على العرض الافتراضي للمشروع. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | يحصل على نسخة من الفئة [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) التي تمثل مجموعة أيام الأسبوع وساعات العمل الافتراضية للمشروع. |
| [getDisplayOptions()](#getDisplayOptions--) | يحصل على نسخة من الفئة [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | يحصل على كائن [Duration](../../com.aspose.tasks/duration) بالعدد المحدد من الوحدات وتنسيق المدة الافتراضي الذي تم تعريفه في إعدادات المشروع [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | يحصل على كائن [Duration](../../com.aspose.tasks/duration) بالعدد المحدد من الوحدات [TimeUnitType](../../com.aspose.tasks/timeunittype). |
| [getDurationFormat()](#getDurationFormat--) | يحصل على قيمة DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | يحصل على قيمة EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | يحصل على كائن ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | يحصل على قيمة ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | يحصل على قيمة FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | يحصل على قيمة تشير إلى ما إذا كان FiscalYearStart مضبوطًا أم لا. |
| [getFyStartDate()](#getFyStartDate--) | يحصل على قيمة FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | يحصل على إعدادات العولمة (المحددة للغة) للمشروع. |
| [getGuid()](#getGuid--) | يحصل على قيمة Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | يحصل على قيمة تشير إلى ما إذا كان HonorConstraints مضبوطًا أم لا. |
| [getHyperlinkBase()](#getHyperlinkBase--) | يحصل على قيمة HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | يحصل على قيمة تشير إلى ما إذا كان InsertedProjectsLikeSummary مضبوطًا أم لا. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | يحصل على قيمة تشير إلى ما إذا كان KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled مضبوطًا أم لا. |
| [getKeywords()](#getKeywords--) | يحصل على قيمة Keywords. |
| [getLastAuthor()](#getLastAuthor--) | يحصل على قيمة LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | يحصل على قيمة LastPrinted. |
| [getLastSaved()](#getLastSaved--) | يحصل على قيمة LastSaved. |
| [getManager()](#getManager--) | يحصل على قيمة Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | يحصل على قيمة تشير إلى ما إذا كان MicrosoftProjectServerURL مضبوطًا أم لا. |
| [getMinutesPerDay()](#getMinutesPerDay--) | يحصل على قيمة MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | يحصل على قيمة MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsBack مضبوطًا أم لا. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsForward مضبوطًا أم لا. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsBack مضبوطًا أم لا. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsForward مضبوطًا أم لا. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | يحصل على قيمة تشير إلى ما إذا كان MultipleCriticalPaths مضبوطًا أم لا. |
| [getName()](#getName--) | يحصل على قيمة Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | يحصل على قيمة NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | يحصل على قيمة تشير إلى ما إذا كان NewTasksAreManual مضبوطًا أم لا. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | يحصل على قيمة تشير إلى ما إذا كان NewTasksEffortDriven مضبوطًا أم لا. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | يحصل على قيمة تشير إلى ما إذا كان NewTasksEstimated مضبوطًا أم لا. |
| [getOleObjects()](#getOleObjects--) | يحصل على مجموعة تحتوي على مثيلات فئة [OleObject](../../com.aspose.tasks/oleobject) التي تم ربطها أو تضمينها في ملف المشروع هذا. |
| [getOutlineCodes()](#getOutlineCodes--) | يحصل على كائن OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) الافتراضي (أيام). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [SaveOptions](../../com.aspose.tasks/saveoptions) المحدد. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) و[PresentationFormat](../../com.aspose.tasks/presentationformat) المحددين. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) و[PageSize](../../com.aspose.tasks/pagesize) المحددين. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) و[PresentationFormat](../../com.aspose.tasks/presentationformat) ونطاق التاريخ المحدد. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) الافتراضي (أيام) و[PresentationFormat](../../com.aspose.tasks/presentationformat) المحدد. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) المحدد. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | يعيد مجموعة من روابط المهام التي هي سابقة للمهمة المحددة. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لمشروع تم قراءته من ملف Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين ProjectExternallyEdited أم لا. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | يحصل على معلومات ملف المشروع من الدفق. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | قراءة معلومات ملف المشروع من الملف. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين RemoveFileProperties أم لا. |
| [getResourceAssignments()](#getResourceAssignments--) | يحصل على كائن ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | يحصل على جميع تعريفات الفلاتر القائمة على الموارد. |
| [getResourceGroups()](#getResourceGroups--) | يحصل على جميع تعريفات المجموعات القائمة على الموارد. |
| [getResources()](#getResources--) | يحصل على كائن ResourceCollection. |
| [getRevision()](#getRevision--) | يحصل على قيمة Revision. |
| [getRootTask()](#getRootTask--) | يحصل على جذر شجرة المهام. |
| [getSaveVersion()](#getSaveVersion--) | يحصل على قيمة SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين ScheduleFromStart أم لا. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين ShowProjectSummaryTask أم لا. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين SplitsInProgressTasks أم لا. |
| [getSpreadActualCost()](#getSpreadActualCost--) | يحصل على قيمة تشير إلى ما إذا كان تم تعيين SpreadActualCost أم لا. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | يحصل على قيمة تشير إلى ما إذا كان SpreadPercentComplete معينًا أم لا. |
| [getStartDate()](#getStartDate--) | يحصل على قيمة لـ StartDate. |
| [getStatusDate()](#getStatusDate--) | يحصل على قيمة لـ StatusDate. |
| [getSubject()](#getSubject--) | يحصل على قيمة لـ Subject. |
| [getTables()](#getTables--) | يحصل على قائمة من كائنات [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | يحصل على جميع تعريفات الفلاتر المستندة إلى المهمة. |
| [getTaskGroups()](#getTaskGroups--) | يحصل على جميع تعريفات المجموعات المستندة إلى المهمة. |
| [getTaskLinks()](#getTaskLinks--) | يحصل على كائن [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | يحصل على قيمة تشير إلى ما إذا كان TaskUpdatesResource معينًا أم لا. |
| [getTemplate()](#getTemplate--) | يحصل على قيمة لـ Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | يحصل على قيمة لـ TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | يحصل على قيمة لـ TimescaleStart. |
| [getTitle()](#getTitle--) | يحصل على قيمة لـ Title. |
| [getUid()](#getUid--) | يحصل على قيمة Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | يحصل على قيمة تشير إلى ما إذا كان UpdateManuallyScheduledTasksWhenEditingLinks معينًا أم لا. |
| [getVbaProject()](#getVbaProject--) | يحصل على نسخة من الفئة `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | يحصل على قائمة من كائنات [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | يحصل على تعريف رمز WBS للمشروع. |
| [getWeekStartDay()](#getWeekStartDay--) | يحصل على قيمة لـ WeekStartDay. |
| [getWork(double val)](#getWork-double-) | يحصل على كائن [Duration](../../com.aspose.tasks/duration) بالقيمة `double` المحددة وتنسيق العمل الافتراضي. |
| [getWorkFormat()](#getWorkFormat--) | يحصل على قيمة لـ WorkFormat. |
| [print()](#print--) | يطبع المشروع إلى الطابعة الافتراضية باستخدام إعدادات الطابعة الافتراضية عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | يطبع المشروع إلى الطابعة الافتراضية باستخدام إعدادات الطابعة الافتراضية وخيارات حفظ مخصصة عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | يطبع المشروع وفقًا لإعدادات الطابعة المحددة عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | يطبع المشروع وفقًا لإعدادات الطابعة المحددة وخيارات حفظ مخصصة عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | يطبع المشروع وفقًا لإعدادات الطابعة المحددة، وخيارات حفظ مخصصة، واسم المستند المحدد عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | يطبع المشروع وفقًا لإعدادات الطابعة المحددة عبر وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم). |
| [print(String printerName)](#print-java.lang.String-) | يطبع المشروع إلى الطابعة المحددة باستخدام إعدادات الطابعة الافتراضية عبر وحدة التحكم القياسية للطباعة (بدون واجهة مستخدم). |
| [recalculate()](#recalculate--) | يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة. |
| [recalculate(boolean validate)](#recalculate-boolean-) | يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة مع التحقق الاختياري. |
| [recalculateResourceFields()](#recalculateResourceFields--) | يعيد حساب المعرف، وتاريخ البدء والانتهاء للموارد. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | يعيد حساب تاريخ البدء والانتهاء للموارد. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | يزيل تعيينات الموارد غير الصالحة من قائمة تعيينات موارد المشروع. |
| [renumberWBSCode()](#renumberWBSCode--) | يعيد ترقيم رمز WBS لجميع المهام. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | يعيد ترقيم رمز WBS للمهام التي تم تمريرها. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | يعيد جدولة العمل غير المكتمل في المشروع ليبدأ بعد تاريخ محدد. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | يعيد جدولة العمل غير المكتمل لقائمة محددة من المهام ليبدأ بعد تاريخ محدد. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | يحفظ المشروع إلى تدفق باستخدام خيارات الحفظ المحددة. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | يحفظ بيانات المشروع إلى التدفق. |
| [save(String filename)](#save-java.lang.String-) | يحفظ بيانات المشروع إلى الملف بصيغة mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | يحفظ المستند إلى ملف باستخدام خيارات الحفظ المحددة. |
| [save(String filename, int format)](#save-java.lang.String-int-) | يحفظ بيانات المشروع إلى الملف. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | يحفظ المشروع كقالب إلى تدفق محدد. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | يحفظ المشروع كقالب إلى تدفق محدد. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | يحفظ المشروع كقالب إلى مسار الملف المحدد. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | يحفظ المشروع كقالب. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | يحفظ تقرير نظرة عامة على المشروع إلى التدفق. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | يحفظ تقرير المشروع من النوع المحدد إلى التدفق المحدد. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | يحفظ تقرير نظرة عامة على المشروع إلى ملف PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | يحفظ تقرير المشروع من النوع المحدد بصيغة PDF إلى مسار الملف المحدد. |
| [selectAllChildTasks()](#selectAllChildTasks--) | يجمع بشكل متكرر جميع المهام الفرعية للمهمة الجذرية. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان ActualsInSync مضبوطًا أم لا. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان AdminProject مضبوطًا أم لا. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان AreEditableActualCosts مضبوطًا أم لا. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط قيمة للخاصية Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان AutoAddNewResourcesAndTasks مضبوطًا أم لا. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | يضبط ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان Autolink مضبوطًا أم لا. |
| [setBaseline(int baselineType)](#setBaseline-int-) | يحفظ حقول الخط الأساسي إلى الخط الأساسي المحدد لكامل المشروع. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | يحفظ حقول الخط الأساسي إلى الخط الأساسي المحدد للمهام المحددة. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | يضبط قيمة للخاصية BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | يضبط وقت حفظ الخط الأساسي. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | يضبط وضع الحساب للمشروع. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | يضبط قيمة للـ Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | يضبط قيمة للخاصية Category. |
| [setComments(String value)](#setComments-java.lang.String-) | يضبط قيمة للخاصية Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | يضبط قيمة للخاصية Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | يضبط قيمة للخاصية CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | تُعتبر المهام حرجة في MS Project إذا كان الفائض الكلي أقل أو يساوي هذا العدد من الأيام. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | يضبط قيمة للخاصية CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | يضبط قيمة للخاصية CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | يضبط قيمة للخاصية CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | يضبط قيمة للخاصية CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | يضبط قيمة للخاصية CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | يضبط قيمة للخاصية CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | يضبط قيمة للخاصية DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | يضبط قيمة للخاصية DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | يضبط قيمة للخاصية DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | يضبط قيمة للخاصية DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | يضبط قيمة للخاصية DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | يضبط قيمة DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | يضبط قيمة DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | يضبط قيمة DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | يضبط قيمة DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | يضبط العرض الافتراضي للمشروع. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | يضبط قيمة DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | يضبط قيمة EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | يضبط قيمة ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | يضبط قيمة FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان FiscalYearStart مُحددًا أم لا. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | يضبط قيمة FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | يضبط إعدادات العولمة (المحددة للغة) للمشروع. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | يضبط قيمة للـ Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان HonorConstraints مُحددًا أم لا. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | يضبط قيمة HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان InsertedProjectsLikeSummary مُحددًا أم لا. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled مُحددًا أم لا. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | يضبط قيمة Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | يضبط قيمة LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | يضبط قيمة LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | يضبط قيمة LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | يضبط قيمة Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MicrosoftProjectServerURL مُحددًا أم لا. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | يضبط قيمة MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | يضبط قيمة MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MoveCompletedEndsBack مُحددًا أم لا. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MoveCompletedEndsForward مُعينًا أم لا. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MoveRemainingStartsBack مُعينًا أم لا. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MoveRemainingStartsForward مُعينًا أم لا. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان MultipleCriticalPaths مُعينًا أم لا. |
| [setName(String value)](#setName-java.lang.String-) | يضبط قيمة Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | يضبط قيمة لـ NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان NewTasksAreManual مُعينًا أم لا. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان NewTasksEffortDriven مُعينًا أم لا. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان NewTasksEstimated مُعينًا أم لا. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان ProjectExternallyEdited مُعينًا أم لا. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان RemoveFileProperties مُعينًا أم لا. |
| [setRevision(int value)](#setRevision-int-) | يضبط قيمة لـ Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | يضبط قيمة لـ SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان ScheduleFromStart مُعينًا أم لا. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | يضبط قيمة تشير إلى ما إذا كان ShowProjectSummaryTask مُعينًا أم لا. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان SplitsInProgressTasks مُعينًا أم لا. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان SpreadActualCost مُعينًا أم لا. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان SpreadPercentComplete مُعينًا أم لا. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | يضبط قيمة لـ StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | يضبط قيمة لـ StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | يضبط قيمة لـ Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان TaskUpdatesResource مُعينًا أم لا. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | يضبط قيمة لـ Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | يضبط قيمة لـ TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | يضبط قيمة لـ TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يضبط قيمة لـ Title. |
| [setUid(String value)](#setUid-java.lang.String-) | يحدد قيمة للـ Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان UpdateManuallyScheduledTasksWhenEditingLinks مضبوطًا أم لا. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | يضبط تعريف رمز WBS للمشروع. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | يضبط قيمة WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | يضبط قيمة WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للمشروع بأكمله. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للقائمة المحددة من المهام. |
### Project() {#Project--}
```
public Project()
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) class.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب محمي بكلمة مرور (ملف mpp أو mpt موجود).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectTemplate | java.lang.String | المسار إلى القالب لإنشاء مشروع منه. |
|  | protectionPassword | java.lang.String | كلمة مرور الحماية. |

--------------------

قراءة الملفات المحمية بكلمة مرور مدعومة حاليًا لتنسيق ملف MSP 2003 فقط. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectTemplate | java.lang.String | المسار إلى القالب لإنشاء مشروع منه. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من الدفق مع المثيل المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق فئة java.io.InputStream الخاصة بالمشروع |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | الكائن المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) الذي يسمح بتخصيص قراءة صيغ Primavera (XER أو XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectTemplate | java.lang.String | المسار إلى القالب لإنشاء مشروع منه. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream لتحميل قالب منه. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


ينشئ مثيلاً جديداً من فئة [Project](../../com.aspose.tasks/project) من قالب (ملف MPP أو MPT موجود) مع المثيل المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectTemplate | java.lang.String | المسار إلى القالب لإنشاء مشروع منه |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | الكائن المحدد من فئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) لقراءة البيانات من قاعدة بيانات يتم تحديدها بواسطة مثيل فئة [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | الكائن المحدد من فئة [DbSettings](../../com.aspose.tasks/dbsettings). |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream لتحميل قالب منه. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream لتحميل قالب منه. |
|  | protectionPassword | java.lang.String | كلمة مرور الحماية. |

--------------------

قراءة الملفات المحمية بكلمة مرور مدعومة حاليًا لتنسيق ملف MSP 2003 فقط. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من قالب (ملف mpp أو mpt موجود) مع المثيل المحدد لفئة [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectTemplate | java.lang.String | المسار إلى القالب لإنشاء مشروع منه |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | الكائن المحدد من فئة [LoadOptions](../../com.aspose.tasks/loadoptions). |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


يُنشئ مثيلاً جديدًا لفئة [Project](../../com.aspose.tasks/project) من الدفق مع المثيل المحدد لفئة [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق فئة java.io.InputStream الخاصة بالمشروع |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | الكائن المحدد من فئة [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Prj](../../com.aspose.tasks/prj) للحصول على مفتاح الخاصية. |

**Returns:**
T - القيمة التي تُعيَّن لها الخاصية في هذه الحاوية.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Prj](../../com.aspose.tasks/prj) للحصول على مفتاح الخاصية. |
| القيمة | T | القيمة. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | مشروع آخر لنسخ البيانات إليه. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | مشروع آخر لنسخ البيانات إليه. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | خيارات النسخ للتحكم في عملية النسخ. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


يُعدد بشكل متكرر جميع مهام المشروع بما في ذلك المهمة الجذرية.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable التي يمكن استخدامها للتنقل عبر جميع مهام المشروع.

--------------------

يوفر طريقة أخف وزنًا للتنقل عبر المهام مقارنةً بطريقة [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) حيث لا تخصّص الذاكرة لجميع المهام.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


يحصل على قيمة تشير إلى ما إذا كان ActualsInSync مُحددًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


يحصل على قيمة تشير إلى ما إذا كان AdminProject مُحددًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


يحصل على قيمة تشير إلى ما إذا كان AreEditableActualCosts مُحددًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


يحصل على قيمة Author.

**Returns:**
java.lang.String - قيمة للمؤلف.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


يحصل على قيمة تشير إلى ما إذا كان AutoAddNewResourcesAndTasks مُحددًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


يحصل على ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد.

**Returns:**
boolean - ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


يحصل على قيمة تشير إلى ما إذا كان Autolink مُحددًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


يحصل على قيمة BaselineForEarnedValue.

**Returns:**
int - قيمة لـ BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


يعيد وقت حفظ الخط الأساسي. يعيد DateTime.MinValue (00:00:00.0000000 UTC، 1 يناير 0001) إذا لم يتم حفظ الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baselineNumber | int | رقم الخط الأساسي [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - تاريخ ووقت الحفظ الأخير للخط الأساسي.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


يحصل على مجموعة الخصائص المدمجة للمشروع.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


يحصل على وضع الحساب لمشروع. يمكن أن يكون أحد قيم تعداد `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - وضع الحساب لمشروع.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


يحصل على قيمة Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


يحصل على كائن [CalendarCollection](../../com.aspose.tasks/calendarcollection) لهذا المثيل من Project.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


يحصل على قيمة Category.

**Returns:**
java.lang.String - قيمة للفئة.
### getComments() {#getComments--}
```
public final String getComments()
```


يحصل على قيمة Comments.

**Returns:**
java.lang.String - قيمة للتعليقات.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


يحصل على قيمة Company.

**Returns:**
java.lang.String - قيمة للشركة.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


يحصل على قيمة CreationDate.

**Returns:**
java.util.Date - قيمة لتاريخ الإنشاء.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


يحصل على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

هذه عملية O(n)، حيث n هو عدد المهام في المشروع.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


تُعتبر المهام حرجة في MS Project إذا كان الفائض الكلي أقل أو يساوي هذا العدد من الأيام.

**Returns:**
int - القيمة القصوى لإجمالي وقت التراخي (بالأيام) التي يُعتبر فيها المهمة حرجة
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


يحصل على قيمة CurrencyCode.

**Returns:**
java.lang.String - قيمة لرمز العملة.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


يحصل على قيمة CurrencyDigits.

**Returns:**
int - قيمة لأرقام العملة.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


يحصل على قيمة CurrencySymbol.

**Returns:**
java.lang.String - قيمة لرمز العملة.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


يحصل على قيمة CurrencySymbolPosition.

**Returns:**
int - قيمة لموضع رمز العملة.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


يحصل على قيمة CurrentDate.

**Returns:**
java.util.Date - قيمة لتاريخ اليوم.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


يحصل على قيمة CustomDateFormat.

**Returns:**
java.lang.String - قيمة لتنسيق التاريخ المخصص.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


يحصل على مجموعة الخصائص المخصصة للمشروع.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


يحصل على قيمة DateFormat.

**Returns:**
int - قيمة لتنسيق التاريخ.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


يحصل على قيمة DaysPerMonth.

**Returns:**
int - قيمة لأيام في الشهر.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


يحصل على قيمة DefaultFinishTime.

**Returns:**
java.util.Date - قيمة لوقت الانتهاء الافتراضي.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


يحصل على قيمة DefaultFixedCostAccrual.

**Returns:**
int - قيمة لـ DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


يحصل على قيمة DefaultOvertimeRate.

**Returns:**
double - قيمة لـ DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


يحصل على قيمة DefaultStandardRate.

**Returns:**
double - قيمة لـ DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


يحصل على قيمة DefaultStartTime.

**Returns:**
java.util.Date - قيمة لـ DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


يحصل على قيمة DefaultTaskEVMethod.

**Returns:**
int - قيمة لـ DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


يحصل على قيمة DefaultTaskType.

**Returns:**
int - قيمة لـ DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


يحصل على العرض الافتراضي للمشروع.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


يحصل على نسخة من الفئة [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) التي تمثل مجموعة أيام الأسبوع وساعات العمل الافتراضية للمشروع.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

البيانات موجودة فقط في ملفات mpp (ليس في xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


يحصل على نسخة من الفئة [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


يحصل على كائن [Duration](../../com.aspose.tasks/duration) بالعدد المحدد من الوحدات وتنسيق المدة الافتراضي الذي تم تعريفه في إعدادات المشروع [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | double | عدد محدد من الوحدات. |

--------------------

يجب استخدام هذه الطريقة بحذر لأنها تُرجع فترات زمنية مختلفة اعتمادًا على إعداد Project.DurationFormat. على سبيل المثال، GetWork(1.0) سيعيد 1 ساعة عندما يكون Project.DurationFormat هو TimeUnitType.Hour أو 1 يوم إذا كان Project.DurationFormat هو TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


يحصل على كائن [Duration](../../com.aspose.tasks/duration) بالعدد المحدد من الوحدات [TimeUnitType](../../com.aspose.tasks/timeunittype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد محدد من الوحدات. |
| وحدة الوقت | byte | قيمة TimeUnitType محددة. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


يحصل على قيمة DurationFormat.

**Returns:**
byte - قيمة لـ DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


يحصل على قيمة EarnedValueMethod.

**Returns:**
int - قيمة لـ EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


يحصل على كائن ExtendedAttributeDefinitionCollection. مجموعة تعريفات السمة الموسعة (الحقول المخصصة) المرتبطة بمشروع.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


يحصل على قيمة ExtendedCreationDate.

**Returns:**
java.util.Date - قيمة لـ ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


يحصل على قيمة FinishDate.

**Returns:**
java.util.Date - قيمة لـ FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


يحصل على قيمة تشير إلى ما إذا كان FiscalYearStart مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


يحصل على قيمة FyStartDate.

**Returns:**
int - قيمة لـ FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


يحصل على إعدادات العولمة (المحددة للغة) للمشروع.

الطريقة الموصى بها هي استخدام القيم أو الصيغ غير المتأثرة بالثقافة عبر المشروع بأكمله. ومع ذلك، إذا كان المشروع يستخدم قيمًا خاصة بالثقافة، يمكن استخدام هذه class للمساعدة في تمكين محرك الحساب من تحليل تلك القيم.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


يحصل على قيمة Guid.

**Returns:**
java.util.UUID - قيمة لـ Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


يحصل على قيمة تشير إلى ما إذا كان HonorConstraints مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


يحصل على قيمة HyperlinkBase.

**Returns:**
java.lang.String - قيمة لـ HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


يحصل على قيمة تشير إلى ما إذا كان InsertedProjectsLikeSummary مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


يحصل على قيمة تشير إلى ما إذا كان KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


يحصل على قيمة Keywords.

**Returns:**
java.lang.String - قيمة لـ Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


يحصل على قيمة LastAuthor.

**Returns:**
java.lang.String - قيمة لـ LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


يحصل على قيمة LastPrinted.

**Returns:**
java.util.Date - قيمة لـ LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


يحصل على قيمة LastSaved.

**Returns:**
java.util.Date - قيمة لـ LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


يحصل على قيمة Manager.

**Returns:**
java.lang.String - قيمة لـ Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


يحصل على قيمة تشير إلى ما إذا كان MicrosoftProjectServerURL مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


يحصل على قيمة MinutesPerDay.

**Returns:**
int - قيمة MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


يحصل على قيمة MinutesPerWeek.

**Returns:**
int - قيمة MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsBack مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsForward مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsBack مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsForward مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


يحصل على قيمة تشير إلى ما إذا كان MultipleCriticalPaths مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


يحصل على قيمة Name.

**Returns:**
java.lang.String - قيمة لـ Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


يحصل على قيمة NewTaskStartDate.

**Returns:**
int - قيمة NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


يحصل على قيمة تشير إلى ما إذا كان NewTasksAreManual مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


يحصل على قيمة تشير إلى ما إذا كان NewTasksEffortDriven مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


يحصل على قيمة تشير إلى ما إذا كان NewTasksEstimated مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


يحصل على مجموعة تحتوي على مثيلات فئة [OleObject](../../com.aspose.tasks/oleobject) التي تم ربطها أو تضمينها في ملف المشروع هذا.

--------------------

متاح لتنسيق ملف mpp فقط. هذه المجموعة للقراءة فقط باستثناء عملية 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


يحصل على كائن OutlineCodeDefinitionCollection. مجموعة تعريفات رمز المخطط المرتبطة بمشروع.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [Timescale](../../com.aspose.tasks/timescale) الافتراضي (أيام).

**Returns:**
int - عدد الصفحات التي سيتم عرضها.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [SaveOptions](../../com.aspose.tasks/saveoptions) المحدد.

--------------------

&gt; ```
&gt; في هذا المثال يتم كتابة كائن HtmlSaveOptions وعدد الصفحات في HTML الناتج إلى وحدة التحكم.
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
عام نهائي فارغ rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
عام نهائي فارغ rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
عام نهائي فارغ حفظ(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
عام فارغ حفظ(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
عام نهائي فارغ حفظ(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
عام نهائي فارغ حفظ(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
عام نهائي فارغ حفظ(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
عام نهائي فارغ saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
عام نهائي فارغ saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
عام نهائي فارغ saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
عام فارغ saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
عام نهائي فارغ saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
عام فارغ saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
عام نهائي فارغ saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
عام نهائي فارغ saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
عام نهائي List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
عام نهائي فارغ تعيين(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
عام نهائي فارغ setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
عام نهائي فارغ setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
عام نهائي فارغ setBaseline(int baselineType)
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
عام نهائي فارغ setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
عام نهائي فارغ setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
عام نهائي فارغ setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
عام نهائي فارغ setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
عام نهائي فارغ setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
عام نهائي فارغ setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
عام نهائي فارغ setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
عام نهائي فارغ setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
عام نهائي فارغ setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
عام نهائي فارغ setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
عام نهائي فارغ setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
عام نهائي فارغ setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
عام نهائي فارغ setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
عام نهائي فارغ setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
عام نهائي فارغ setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
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

