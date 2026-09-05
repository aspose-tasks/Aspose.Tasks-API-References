---
title: "प्रोजेक्ट"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक प्रोजेक्ट दर्शाता है।"
type: docs
weight: 220
url: /hi/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

एक प्रोजेक्ट दर्शाता है।

--------------------

यह **Project** Aspose.Tasks लाइब्रेरी में एक केंद्रीय क्लास है।

आप **Project** का उपयोग करके समर्थित प्रोजेक्ट प्रबंधन फ़ॉर्मेट्स में से एक पढ़ सकते हैं: MPP, MPT, MPX, XML.

समर्थित किसी भी फ़ॉर्मेट में मौजूदा दस्तावेज़ को लोड करने के लिए, फ़ाइल नाम या स्ट्रीम को **Project** के किसी एक कंस्ट्रक्टर में पास करें। खाली प्रोजेक्ट बनाने के लिए, पैरामीटर‑रहित कंस्ट्रक्टर को कॉल करें।

परियोजना को किसी भी [SaveFileFormat](../../com.aspose.tasks/savefileformat) फ़ॉर्मेट में सहेजने के लिए Save मेथड के ओवरलोड्स में से एक का उपयोग करें: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

परियोजना को प्रिंट करने के लिए, [print()](../../com.aspose.tasks/project\#print--) मेथड के ओवरलोड्स में से एक का उपयोग करें।

यह **Project** परियोजना‑व्यापी जानकारी संग्रहीत करता है जैसे `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), और `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). इनमें से अधिकांश ऑब्जेक्ट्स **Project** क्लास की संबंधित प्रॉपर्टीज़ के माध्यम से उपलब्ध हैं।

यह **Project** एक मूल इकाई है जो अन्य प्रोजेक्ट इकाइयों को संशोधित करने के लिए प्रवेश बिंदु रखती है, जैसे कि [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) और [Calendar](../../com.aspose.tasks/calendar).

**Project** इकाइयों तक टाइप्ड कलेक्शन्स के माध्यम से पहुंचा जा सकता है, उदाहरण के लिए `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), आदि।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Project()](#Project--) | नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | पासवर्ड‑सुरक्षित टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(String projectTemplate)](#Project-java.lang.String-) | टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | स्ट्रीम से, निर्दिष्ट [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास के इंस्टेंस के साथ, नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | स्ट्रीम से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | टेम्पलेट (मौजूदा MPP या MPT फ़ाइल) से, निर्दिष्ट [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास के इंस्टेंस के साथ, नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | डेटाबेस से डेटा पढ़ने के लिए, जो [DbSettings](../../com.aspose.tasks/dbsettings) क्लास की इंस्टेंस द्वारा निर्दिष्ट है, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से, निर्दिष्ट [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की इंस्टेंस के साथ, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | स्ट्रीम से, निर्दिष्ट [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की इंस्टेंस के साथ, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है। |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है। |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है। |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है। |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | रूट टास्क सहित सभी परियोजना कार्यों को पुनरावर्ती रूप से सूचीबद्ध करता है। |
| [getActualsInSync()](#getActualsInSync--) | यह दर्शाने वाला मान प्राप्त करता है कि ActualsInSync सेट है या नहीं। |
| [getAdminProject()](#getAdminProject--) | यह दर्शाने वाला मान प्राप्त करता है कि AdminProject सेट है या नहीं। |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | यह दर्शाने वाला मान प्राप्त करता है कि AreEditableActualCosts सेट है या नहीं। |
| [getAuthor()](#getAuthor--) | Author का मान प्राप्त करता है। |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | यह दर्शाने वाला मान प्राप्त करता है कि AutoAddNewResourcesAndTasks सेट है या नहीं। |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | यह प्राप्त करता है कि असाइनमेंट की लागत और शेष लागत को असाइनमेंट के कार्य और संसाधन दरों का उपयोग करके स्वचालित रूप से गणना किया जाना चाहिए या नहीं। |
| [getAutolink()](#getAutolink--) | यह दर्शाने वाला मान प्राप्त करता है कि Autolink सेट है या नहीं। |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | BaselineForEarnedValue का मान प्राप्त करता है। |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | बेसलाइन सहेजने का समय लौटाता है। |
| [getBuiltInProps()](#getBuiltInProps--) | परियोजना की अंतर्निहित गुणों का संग्रह प्राप्त करता है। |
| [getCalculationMode()](#getCalculationMode--) | परियोजना की गणना मोड प्राप्त करता है। |
| [getCalendar()](#getCalendar--) | Calendar का मान प्राप्त करता है। |
| [getCalendars()](#getCalendars--) | इस Project इंस्टेंस का [CalendarCollection](../../com.aspose.tasks/calendarcollection) ऑब्जेक्ट प्राप्त करता है। |
| [getCategory()](#getCategory--) | Category का मान प्राप्त करता है। |
| [getComments()](#getComments--) | Comments का मान प्राप्त करता है। |
| [getCompany()](#getCompany--) | Company का मान प्राप्त करता है। |
| [getCreationDate()](#getCreationDate--) | CreationDate का मान प्राप्त करता है। |
| [getCriticalPath()](#getCriticalPath--) | एक संग्रह प्राप्त करता है जिसमें इस परियोजना के Critical Path को बनाते हुए Critical कार्यों की सूची शामिल है। |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | यदि कुल स्लैक इस संख्या के दिनों से कम या बराबर हो तो MS Project द्वारा कार्यों को महत्वपूर्ण माना जाता है। |
| [getCurrencyCode()](#getCurrencyCode--) | CurrencyCode का मान प्राप्त करता है। |
| [getCurrencyDigits()](#getCurrencyDigits--) | CurrencyDigits का मान प्राप्त करता है। |
| [getCurrencySymbol()](#getCurrencySymbol--) | CurrencySymbol का मान प्राप्त करता है। |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | CurrencySymbolPosition का मान प्राप्त करता है। |
| [getCurrentDate()](#getCurrentDate--) | CurrentDate का मान प्राप्त करता है। |
| [getCustomDateFormat()](#getCustomDateFormat--) | CustomDateFormat का मान प्राप्त करता है। |
| [getCustomProps()](#getCustomProps--) | प्रोजेक्ट की कस्टम प्रॉपर्टीज़ संग्रह प्राप्त करता है। |
| [getDateFormat()](#getDateFormat--) | DateFormat का मान प्राप्त करता है। |
| [getDaysPerMonth()](#getDaysPerMonth--) | DaysPerMonth का मान प्राप्त करता है। |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | DefaultFinishTime का मान प्राप्त करता है। |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | DefaultFixedCostAccrual का मान प्राप्त करता है। |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | DefaultOvertimeRate का मान प्राप्त करता है। |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | DefaultStandardRate का मान प्राप्त करता है। |
| [getDefaultStartTime()](#getDefaultStartTime--) | DefaultStartTime का मान प्राप्त करता है। |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | DefaultTaskEVMethod का मान प्राप्त करता है। |
| [getDefaultTaskType()](#getDefaultTaskType--) | DefaultTaskType का मान प्राप्त करता है। |
| [getDefaultView()](#getDefaultView--) | प्रोजेक्ट का डिफ़ॉल्ट व्यू प्राप्त करता है। |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | प्रोजेक्ट के डिफ़ॉल्ट सप्ताह के कार्य दिवसों और कार्य समयों का संग्रह दर्शाने वाली [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) क्लास का इंस्टेंस प्राप्त करता है। |
| [getDisplayOptions()](#getDisplayOptions--) | प्राप्त करता है [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) क्लास का इंस्टेंस। |
| [getDuration(double val)](#getDuration-double-) | निर्दिष्ट इकाइयों की संख्या और डिफ़ॉल्ट अवधि फ़ॉर्मेट के साथ [Duration](../../com.aspose.tasks/duration) ऑब्जेक्ट प्राप्त करता है, जो प्रोजेक्ट की सेटिंग्स में परिभाषित है [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT)। |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | निर्दिष्ट संख्या में [TimeUnitType](../../com.aspose.tasks/timeunittype) इकाइयों के साथ [Duration](../../com.aspose.tasks/duration) ऑब्जेक्ट प्राप्त करता है। |
| [getDurationFormat()](#getDurationFormat--) | DurationFormat का मान प्राप्त करता है। |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | EarnedValueMethod का मान प्राप्त करता है। |
| [getExtendedAttributes()](#getExtendedAttributes--) | ExtendedAttributeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | ExtendedCreationDate का मान प्राप्त करता है। |
| [getFinishDate()](#getFinishDate--) | FinishDate का मान प्राप्त करता है। |
| [getFiscalYearStart()](#getFiscalYearStart--) | FiscalYearStart सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getFyStartDate()](#getFyStartDate--) | FyStartDate का मान प्राप्त करता है। |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | प्रोजेक्ट की ग्लोबलाइज़ेशन (भाषा-विशिष्ट) सेटिंग्स प्राप्त करता है। |
| [getGuid()](#getGuid--) | GUID का मान प्राप्त करता है। |
| [getHonorConstraints()](#getHonorConstraints--) | HonorConstraints सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getHyperlinkBase()](#getHyperlinkBase--) | HyperlinkBase का मान प्राप्त करता है। |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | InsertedProjectsLikeSummary सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getKeywords()](#getKeywords--) | Keywords का मान प्राप्त करता है। |
| [getLastAuthor()](#getLastAuthor--) | LastAuthor का मान प्राप्त करता है। |
| [getLastPrinted()](#getLastPrinted--) | LastPrinted का मान प्राप्त करता है। |
| [getLastSaved()](#getLastSaved--) | LastSaved का मान प्राप्त करता है। |
| [getManager()](#getManager--) | Manager का मान प्राप्त करता है। |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | MicrosoftProjectServerURL सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMinutesPerDay()](#getMinutesPerDay--) | MinutesPerDay का मान प्राप्त करता है। |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | MinutesPerWeek का मान प्राप्त करता है। |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | MoveCompletedEndsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | MoveCompletedEndsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | MoveRemainingStartsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | MoveRemainingStartsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | MultipleCriticalPaths सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getName()](#getName--) | नाम का मान प्राप्त करता है। |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | NewTaskStartDate का मान प्राप्त करता है। |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | NewTasksAreManual सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | NewTasksEffortDriven सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | NewTasksEstimated सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getOleObjects()](#getOleObjects--) | इस प्रोजेक्ट फ़ाइल से जुड़े या एम्बेड किए गए [OleObject](../../com.aspose/tasks/oleobject) क्लास के इंस्टेंस को शामिल करने वाला संग्रह प्राप्त करता है। |
| [getOutlineCodes()](#getOutlineCodes--) | OutlineCodeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। |
| [getPageCount()](#getPageCount--) | डिफ़ॉल्ट [Timescale](../../com.aspose.tasks/timescale)(Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | दिए गए [SaveOptions](../../com.aspose.tasks/saveoptions) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | दिए गए [Timescale](../../com.aspose.tasks/timescale) और [PresentationFormat](../../com.aspose.tasks/presentationformat) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | दिए गए [Timescale](../../com.aspose.tasks/timescale) और [PageSize](../../com.aspose.tasks/pagesize) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | दिए गए [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) और तिथि सीमा का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | डिफ़ॉल्ट [Timescale](../../com.aspose.tasks/timescale)(Days) और दिए गए [PresentationFormat](../../com.aspose.tasks/presentationformat) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | दिए गए [Timescale](../../com.aspose.tasks/timescale) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है। |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | निर्दिष्ट टास्क के पूर्ववर्ती होने वाले टास्क लिंक का संग्रह लौटाता है। |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Primavera फ़ाइल से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट गुणों वाला ऑब्जेक्ट प्राप्त करता है। |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | यह दर्शाने वाला मान प्राप्त करता है कि ProjectExternallyEdited सेट है या नहीं। |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | स्ट्रीम से प्रोजेक्ट फ़ाइल जानकारी प्राप्त करता है। |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | फ़ाइल से प्रोजेक्ट फ़ाइल जानकारी पढ़ता है। |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | यह दर्शाने वाला मान प्राप्त करता है कि RemoveFileProperties सेट है या नहीं। |
| [getResourceAssignments()](#getResourceAssignments--) | ResourceAssignmentCollection ऑब्जेक्ट प्राप्त करता है। |
| [getResourceFilters()](#getResourceFilters--) | सभी रिसोर्स-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। |
| [getResourceGroups()](#getResourceGroups--) | सभी रिसोर्स-आधारित समूह परिभाषाएँ प्राप्त करता है। |
| [getResources()](#getResources--) | ResourceCollection ऑब्जेक्ट प्राप्त करता है। |
| [getRevision()](#getRevision--) | Revision का मान प्राप्त करता है। |
| [getRootTask()](#getRootTask--) | टास्क ट्री की जड़ प्राप्त करता है। |
| [getSaveVersion()](#getSaveVersion--) | SaveVersion का मान प्राप्त करता है। |
| [getScheduleFromStart()](#getScheduleFromStart--) | यह दर्शाने वाला मान प्राप्त करता है कि ScheduleFromStart सेट है या नहीं। |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | यह दर्शाने वाला मान प्राप्त करता है कि ShowProjectSummaryTask सेट है या नहीं। |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | यह दर्शाने वाला मान प्राप्त करता है कि SplitsInProgressTasks सेट है या नहीं। |
| [getSpreadActualCost()](#getSpreadActualCost--) | यह दर्शाने वाला मान प्राप्त करता है कि SpreadActualCost सेट है या नहीं। |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | SpreadPercentComplete सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getStartDate()](#getStartDate--) | StartDate का मान प्राप्त करता है। |
| [getStatusDate()](#getStatusDate--) | StatusDate का मान प्राप्त करता है। |
| [getSubject()](#getSubject--) | Subject का मान प्राप्त करता है। |
| [getTables()](#getTables--) | [Table](../../com.aspose.tasks/table) वस्तुओं की सूची प्राप्त करता है। |
| [getTaskFilters()](#getTaskFilters--) | सभी टास्क-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। |
| [getTaskGroups()](#getTaskGroups--) | सभी टास्क-आधारित समूह परिभाषाएँ प्राप्त करता है। |
| [getTaskLinks()](#getTaskLinks--) | [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) ऑब्जेक्ट प्राप्त करता है। |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | TaskUpdatesResource सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getTemplate()](#getTemplate--) | Template का मान प्राप्त करता है। |
| [getTimescaleFinish()](#getTimescaleFinish--) | TimescaleFinish का मान प्राप्त करता है। |
| [getTimescaleStart()](#getTimescaleStart--) | TimescaleStart का मान प्राप्त करता है। |
| [getTitle()](#getTitle--) | Title का मान प्राप्त करता है। |
| [getUid()](#getUid--) | यूआईडी का मान प्राप्त करता है। |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | UpdateManuallyScheduledTasksWhenEditingLinks सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getVbaProject()](#getVbaProject--) | `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) क्लास का एक उदाहरण प्राप्त करता है। |
| [getViews()](#getViews--) | [View](../../com.aspose.tasks/view) वस्तुओं की सूची प्राप्त करता है। |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | परियोजना के लिए WBS कोड परिभाषा प्राप्त करता है। |
| [getWeekStartDay()](#getWeekStartDay--) | WeekStartDay का मान प्राप्त करता है। |
| [getWork(double val)](#getWork-double-) | निर्दिष्ट `double` मान और डिफ़ॉल्ट कार्य स्वरूप के साथ [Duration](../../com.aspose.tasks/duration) ऑब्जेक्ट प्राप्त करता है। |
| [getWorkFormat()](#getWorkFormat--) | WorkFormat का मान प्राप्त करता है। |
| [print()](#print--) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स के साथ प्रोजेक्ट को डिफ़ॉल्ट प्रिंटर पर प्रिंट करता है। |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स और कस्टम सहेजने विकल्पों के साथ प्रोजेक्ट को डिफ़ॉल्ट प्रिंटर पर प्रिंट करता है। |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स के अनुसार प्रोजेक्ट को प्रिंट करता है। |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स और कस्टम सहेजने विकल्पों के अनुसार प्रोजेक्ट को प्रिंट करता है। |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स, कस्टम सहेजने विकल्प और निर्दिष्ट दस्तावेज़ नाम के अनुसार प्रोजेक्ट को प्रिंट करता है। |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | मानक (बिना यूज़र इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स के अनुसार प्रोजेक्ट को प्रिंट करता है। |
| [print(String printerName)](#print-java.lang.String-) | निर्दिष्ट प्रिंटर पर डिफ़ॉल्ट प्रिंटर सेटिंग्स के साथ मानक (कोई उपयोगकर्ता इंटरफ़ेस नहीं) प्रिंट कंट्रोलर का उपयोग करके प्रोजेक्ट प्रिंट करता है। |
| [recalculate()](#recalculate--) | सभी प्रोजेक्ट कार्यों के आईडी, रूपरेखा स्तर, प्रारंभ/समाप्ति तिथियों को पुनः निर्धारित करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है। |
| [recalculate(boolean validate)](#recalculate-boolean-) | वैकल्पिक सत्यापन के साथ सभी प्रोजेक्ट कार्यों के आईडी, रूपरेखा स्तर, प्रारंभ/समाप्ति तिथियों को पुनः निर्धारित करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है। |
| [recalculateResourceFields()](#recalculateResourceFields--) | संसाधनों के आईडी, प्रारंभ और समाप्ति को पुनः गणना करता है। |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | संसाधनों के प्रारंभ और समाप्ति को पुनः गणना करता है। |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | प्रोजेक्ट संसाधन असाइनमेंट सूची से अमान्य संसाधन असाइनमेंट को हटाता है। |
| [renumberWBSCode()](#renumberWBSCode--) | सभी कार्यों के WBS कोड को पुनः क्रमांकित करता है। |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | प्रदान किए गए कार्यों के WBS कोड को पुनः क्रमांकित करता है। |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | अपूर्ण प्रोजेक्ट कार्य को निर्दिष्ट तिथि के बाद शुरू होने के लिए पुनः निर्धारित करता है। |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | निर्दिष्ट कार्यों की सूची के लिए अपूर्ण कार्य को निर्दिष्ट तिथि के बाद शुरू होने के लिए पुनः निर्धारित करता है। |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके प्रोजेक्ट को स्ट्रीम में सहेजता है। |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | प्रोजेक्ट डेटा को स्ट्रीम में सहेजता है। |
| [save(String filename)](#save-java.lang.String-) | प्रोजेक्ट डेटा को mpp फ़ॉर्मेट में फ़ाइल में सहेजता है। |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके दस्तावेज़ को फ़ाइल में सहेजता है। |
| [save(String filename, int format)](#save-java.lang.String-int-) | प्रोजेक्ट डेटा को फ़ाइल में सहेजता है। |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | प्रोजेक्ट को टेम्प्लेट के रूप में निर्दिष्ट स्ट्रीम में सहेजता है। |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | प्रोजेक्ट को टेम्प्लेट के रूप में निर्दिष्ट स्ट्रीम में सहेजता है। |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | प्रोजेक्ट को टेम्प्लेट के रूप में निर्दिष्ट फ़ाइल पथ पर सहेजता है। |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | प्रोजेक्ट को टेम्प्लेट के रूप में सहेजता है। |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | प्रोजेक्ट अवलोकन रिपोर्ट को स्ट्रीम में सहेजता है। |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | निर्दिष्ट प्रकार की प्रोजेक्ट रिपोर्ट को निर्दिष्ट स्ट्रीम में सहेजता है। |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | प्रोजेक्ट अवलोकन रिपोर्ट को PDF फ़ाइल में सहेजता है। |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | निर्दिष्ट प्रकार की प्रोजेक्ट रिपोर्ट को PDF फ़ॉर्मेट में निर्दिष्ट फ़ाइल पथ पर सहेजता है। |
| [selectAllChildTasks()](#selectAllChildTasks--) | रूट टास्क के सभी चाइल्ड टास्क को पुनरावर्ती रूप से एकत्र करता है। |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है। |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि ActualsInSync सेट है या नहीं। |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि AdminProject सेट है या नहीं। |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि AreEditableActualCosts सेट है या नहीं। |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Author का मान सेट करता है। |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि AutoAddNewResourcesAndTasks सेट है या नहीं। |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | निर्धारित करता है कि असाइनमेंट लागत और शेष लागत को असाइनमेंट के कार्य और संसाधन दरों का उपयोग करके स्वचालित रूप से गणना किया जाना चाहिए या नहीं। |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि Autolink सेट है या नहीं। |
| [setBaseline(int baselineType)](#setBaseline-int-) | पूरे प्रोजेक्ट के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड सहेजता है। |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | चयनित कार्यों के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड सहेजता है। |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | BaselineForEarnedValue का मान सेट करता है। |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | बेसलाइन सहेजने का समय सेट करता है। |
| [setCalculationMode(int value)](#setCalculationMode-int-) | प्रोजेक्ट की गणना मोड सेट करता है। |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar का मान सेट करता है। |
| [setCategory(String value)](#setCategory-java.lang.String-) | Category का मान सेट करता है। |
| [setComments(String value)](#setComments-java.lang.String-) | Comments का मान सेट करता है। |
| [setCompany(String value)](#setCompany-java.lang.String-) | Company का मान सेट करता है। |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | CreationDate का मान सेट करता है। |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | यदि कुल स्लैक इस संख्या के दिनों से कम या बराबर हो तो MS Project द्वारा कार्यों को महत्वपूर्ण माना जाता है। |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | CurrencyCode का मान सेट करता है। |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | CurrencyDigits का मान सेट करता है। |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | CurrencySymbol का मान सेट करता है। |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | CurrencySymbolPosition का मान सेट करता है। |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | CurrentDate का मान सेट करता है। |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | CustomDateFormat का मान सेट करता है। |
| [setDateFormat(int value)](#setDateFormat-int-) | DateFormat का मान सेट करता है। |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | DaysPerMonth का मान सेट करता है। |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | DefaultFinishTime का मान सेट करता है। |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | DefaultFixedCostAccrual का मान सेट करता है। |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | DefaultOvertimeRate का मान सेट करता है। |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | DefaultStandardRate का मान सेट करता है। |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | DefaultStartTime का मान सेट करता है। |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | DefaultTaskEVMethod का मान सेट करता है। |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | DefaultTaskType का मान सेट करता है। |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | परियोजना का डिफ़ॉल्ट दृश्य सेट करता है। |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | DurationFormat का मान सेट करता है। |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | EarnedValueMethod का मान सेट करता है। |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | ExtendedCreationDate का मान सेट करता है। |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | FinishDate का मान सेट करता है। |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | FiscalYearStart सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setFyStartDate(int value)](#setFyStartDate-int-) | FyStartDate का मान सेट करता है। |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | परियोजना की ग्लोबलाइज़ेशन (भाषा-विशिष्ट) सेटिंग्स सेट करता है। |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Guid का मान सेट करता है। |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | HonorConstraints सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | HyperlinkBase का मान सेट करता है। |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | InsertedProjectsLikeSummary सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Keywords का मान सेट करता है। |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | LastAuthor का मान सेट करता है। |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | LastPrinted का मान सेट करता है। |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | LastSaved का मान सेट करता है। |
| [setManager(String value)](#setManager-java.lang.String-) | Manager का मान सेट करता है। |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | MicrosoftProjectServerURL सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | MinutesPerDay का मान सेट करता है। |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | MinutesPerWeek का मान सेट करता है। |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | MoveCompletedEndsBack सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि MoveCompletedEndsForward सेट है या नहीं। |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि MoveRemainingStartsBack सेट है या नहीं। |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि MoveRemainingStartsForward सेट है या नहीं। |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि MultipleCriticalPaths सेट है या नहीं। |
| [setName(String value)](#setName-java.lang.String-) | Name का मान सेट करता है। |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | NewTaskStartDate का मान सेट करता है। |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि NewTasksAreManual सेट है या नहीं। |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि NewTasksEffortDriven सेट है या नहीं। |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि NewTasksEstimated सेट है या नहीं। |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि ProjectExternallyEdited सेट है या नहीं। |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि RemoveFileProperties सेट है या नहीं। |
| [setRevision(int value)](#setRevision-int-) | Revision का मान सेट करता है। |
| [setSaveVersion(int value)](#setSaveVersion-int-) | SaveVersion का मान सेट करता है। |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि ScheduleFromStart सेट है या नहीं। |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | एक मान सेट करता है जो दर्शाता है कि ShowProjectSummaryTask सेट है या नहीं। |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि SplitsInProgressTasks सेट है या नहीं। |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि SpreadActualCost सेट है या नहीं। |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि SpreadPercentComplete सेट है या नहीं। |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | StartDate का मान सेट करता है। |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | StatusDate का मान सेट करता है। |
| [setSubject(String value)](#setSubject-java.lang.String-) | Subject का मान सेट करता है। |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | एक मान सेट करता है जो दर्शाता है कि TaskUpdatesResource सेट है या नहीं। |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Template का मान सेट करता है। |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | TimescaleFinish का मान सेट करता है। |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | TimescaleStart का मान सेट करता है। |
| [setTitle(String value)](#setTitle-java.lang.String-) | Title का मान सेट करता है। |
| [setUid(String value)](#setUid-java.lang.String-) | Uid का मान सेट करता है। |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | UpdateManuallyScheduledTasksWhenEditingLinks सेट है या नहीं, यह दर्शाने के लिए एक मान सेट करता है। |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | प्रोजेक्ट के लिए WBS कोड परिभाषा सेट करता है। |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | WeekStartDay का मान सेट करता है। |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | WorkFormat का मान सेट करता है। |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | पूरे प्रोजेक्ट के लिए निर्दिष्ट तिथि तक सभी कार्यों को पूर्ण के रूप में अपडेट करता है। |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | निर्दिष्ट कार्यों की सूची के लिए निर्दिष्ट तिथि तक सभी कार्यों को पूर्ण के रूप में अपडेट करता है। |
### Project() {#Project--}
```
public Project()
```


नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


पासवर्ड‑सुरक्षित टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | java.lang.String | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पथ। |
|  | protectionPassword | java.lang.String | सुरक्षा पासवर्ड। |

--------------------

वर्तमान में केवल MSP 2003 फ़ाइल फ़ॉर्मेट के लिए पासवर्ड-संरक्षित फ़ाइलों को पढ़ना समर्थित है। |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | java.lang.String | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पथ। |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


स्ट्रीम से, निर्दिष्ट [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास के इंस्टेंस के साथ, नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | प्रोजेक्ट का स्ट्रीम java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास की निर्दिष्ट इंस्टेंस जो Primavera फ़ॉर्मेट (XER या XML) को पढ़ने को अनुकूलित करने की अनुमति देती है। |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | java.lang.String | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पथ। |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML पार्स त्रुटियों को संभालने के लिए निर्दिष्ट कॉलबैक मेथड। |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


स्ट्रीम से नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | टेम्प्लेट लोड करने के लिए java.io.InputStream। |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


टेम्पलेट (मौजूदा MPP या MPT फ़ाइल) से, निर्दिष्ट [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास के इंस्टेंस के साथ, नए [Project](../../com.aspose.tasks/project) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | java.lang.String | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पथ |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास की निर्दिष्ट इंस्टेंस। |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


डेटाबेस से डेटा पढ़ने के लिए, जो [DbSettings](../../com.aspose.tasks/dbsettings) क्लास की इंस्टेंस द्वारा निर्दिष्ट है, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | [DbSettings](../../com.aspose.tasks/dbsettings) क्लास की निर्दिष्ट इंस्टेंस। |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | टेम्प्लेट लोड करने के लिए java.io.InputStream। |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML पार्स त्रुटियों को संभालने के लिए निर्दिष्ट कॉलबैक मेथड। |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | टेम्प्लेट लोड करने के लिए java.io.InputStream। |
|  | protectionPassword | java.lang.String | सुरक्षा पासवर्ड। |

--------------------

वर्तमान में केवल MSP 2003 फ़ाइल फ़ॉर्मेट के लिए पासवर्ड-संरक्षित फ़ाइलों को पढ़ना समर्थित है। |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से, निर्दिष्ट [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की इंस्टेंस के साथ, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | java.lang.String | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पथ |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की निर्दिष्ट इंस्टेंस। |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


स्ट्रीम से, निर्दिष्ट [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की इंस्टेंस के साथ, नया [Project](../../com.aspose.tasks/project) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | प्रोजेक्ट का स्ट्रीम java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास की निर्दिष्ट इंस्टेंस |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Prj](../../com.aspose.tasks/prj)। |

**Returns:**
T - वह मान जिससे इस कंटेनर में प्रॉपर्टी मैप की गई है।
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Prj](../../com.aspose.tasks/prj)। |
| मान | T | मान। |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | डेटा कॉपी करने के लिए दूसरा प्रोजेक्ट। |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


परियोजना के मुख्य डेटा और गुणों को दूसरी परियोजना में कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | डेटा कॉपी करने के लिए दूसरा प्रोजेक्ट। |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | कॉपी प्रक्रिया को नियंत्रित करने के लिए कॉपी विकल्प। |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


रूट टास्क सहित सभी परियोजना कार्यों को पुनरावर्ती रूप से सूचीबद्ध करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - वह IEnumerable जो सभी प्रोजेक्ट के कार्यों पर इटररेट करने के लिए उपयोग किया जा सकता है।

--------------------

यह कार्यों पर इटररेट करने के लिए [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) मेथड की तुलना में अधिक हल्का तरीका प्रदान करता है क्योंकि यह सभी कार्यों के लिए मेमोरी आवंटित नहीं करता।
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


यह दर्शाने वाला मान प्राप्त करता है कि ActualsInSync सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


यह दर्शाने वाला मान प्राप्त करता है कि AdminProject सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


यह दर्शाने वाला मान प्राप्त करता है कि AreEditableActualCosts सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Author का मान प्राप्त करता है।

**Returns:**
java.lang.String - Author का मान।
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


यह दर्शाने वाला मान प्राप्त करता है कि AutoAddNewResourcesAndTasks सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


यह प्राप्त करता है कि असाइनमेंट की लागत और शेष लागत को असाइनमेंट के कार्य और संसाधन दरों का उपयोग करके स्वचालित रूप से गणना किया जाना चाहिए या नहीं।

**Returns:**
boolean - यह निर्धारित करता है कि असाइनमेंट लागत और शेष लागत को असाइनमेंट के कार्य और संसाधन दरों का उपयोग करके स्वचालित रूप से गणना किया जाना चाहिए या नहीं।
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


यह दर्शाने वाला मान प्राप्त करता है कि Autolink सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


BaselineForEarnedValue का मान प्राप्त करता है।

**Returns:**
int - BaselineForEarnedValue का मान।
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


बेसलाइन सहेजने का समय लौटाता है। यदि बेसलाइन सहेजा नहीं गया हो तो DateTime.MinValue (00:00:00.0000000 UTC, 1 जनवरी 0001) लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| baselineNumber | int | बेसलाइन का नंबर [BaselineType](../../com.aspose.tasks/baselinetype)। |

**Returns:**
java.util.Date - बेसलाइन की अंतिम सहेजने की तिथि और समय।
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


परियोजना की अंतर्निहित गुणों का संग्रह प्राप्त करता है।

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


एक प्रोजेक्ट का कैलकुलेशन मोड प्राप्त करता है। यह `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) एनेमरेशन के मानों में से एक हो सकता है।

**Returns:**
int - प्रोजेक्ट का कैलकुलेशन मोड।
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar का मान प्राप्त करता है।

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


इस Project इंस्टेंस का [CalendarCollection](../../com.aspose.tasks/calendarcollection) ऑब्जेक्ट प्राप्त करता है।

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Category का मान प्राप्त करता है।

**Returns:**
java.lang.String - Category का मान।
### getComments() {#getComments--}
```
public final String getComments()
```


Comments का मान प्राप्त करता है।

**Returns:**
java.lang.String - Comments का मान।
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Company का मान प्राप्त करता है।

**Returns:**
java.lang.String - Company का मान।
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


CreationDate का मान प्राप्त करता है।

**Returns:**
java.util.Date - CreationDate का मान।
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


एक संग्रह प्राप्त करता है जिसमें इस परियोजना के Critical Path को बनाते हुए Critical कार्यों की सूची शामिल है।

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

यह O(n) ऑपरेशन है, जहाँ n प्रोजेक्ट में कार्यों की संख्या है।
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


यदि कुल स्लैक इस संख्या के दिनों से कम या बराबर हो तो MS Project द्वारा कार्यों को महत्वपूर्ण माना जाता है।

**Returns:**
int - वह अधिकतम कुल स्लैक समय (दिनों में) जिसका कार्य महत्वपूर्ण माना जाता है।
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


CurrencyCode का मान प्राप्त करता है।

**Returns:**
java.lang.String - CurrencyCode का मान।
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


CurrencyDigits का मान प्राप्त करता है।

**Returns:**
int - CurrencyDigits का मान।
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


CurrencySymbol का मान प्राप्त करता है।

**Returns:**
java.lang.String - CurrencySymbol का मान।
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


CurrencySymbolPosition का मान प्राप्त करता है।

**Returns:**
int - CurrencySymbolPosition का मान।
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


CurrentDate का मान प्राप्त करता है।

**Returns:**
java.util.Date - CurrentDate का मान।
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


CustomDateFormat का मान प्राप्त करता है।

**Returns:**
java.lang.String - CustomDateFormat का मान।
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


प्रोजेक्ट की कस्टम प्रॉपर्टीज़ संग्रह प्राप्त करता है।

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


DateFormat का मान प्राप्त करता है।

**Returns:**
int - DateFormat का मान।
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


DaysPerMonth का मान प्राप्त करता है।

**Returns:**
int - DaysPerMonth का मान।
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


DefaultFinishTime का मान प्राप्त करता है।

**Returns:**
java.util.Date - DefaultFinishTime का मान।
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


DefaultFixedCostAccrual का मान प्राप्त करता है।

**Returns:**
int - DefaultFixedCostAccrual का मान।
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


DefaultOvertimeRate का मान प्राप्त करता है।

**Returns:**
double - DefaultOvertimeRate का मान।
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


DefaultStandardRate का मान प्राप्त करता है।

**Returns:**
double - DefaultStandardRate का मान।
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


DefaultStartTime का मान प्राप्त करता है।

**Returns:**
java.util.Date - DefaultStartTime का मान।
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


DefaultTaskEVMethod का मान प्राप्त करता है।

**Returns:**
int - DefaultTaskEVMethod का मान।
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


DefaultTaskType का मान प्राप्त करता है।

**Returns:**
int - DefaultTaskType का मान।
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


प्रोजेक्ट का डिफ़ॉल्ट व्यू प्राप्त करता है।

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


प्रोजेक्ट के डिफ़ॉल्ट सप्ताह के कार्य दिवसों और कार्य समयों का संग्रह दर्शाने वाली [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) क्लास का इंस्टेंस प्राप्त करता है।

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

डेटा केवल mpp फ़ाइलों में मौजूद है (xml में नहीं)।
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


प्राप्त करता है [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) क्लास का इंस्टेंस।

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


निर्दिष्ट इकाइयों की संख्या और डिफ़ॉल्ट अवधि फ़ॉर्मेट के साथ [Duration](../../com.aspose.tasks/duration) ऑब्जेक्ट प्राप्त करता है, जो प्रोजेक्ट की सेटिंग्स में परिभाषित है [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | double | निर्दिष्ट इकाइयों की संख्या। |

--------------------

इस विधि का उपयोग सावधानीपूर्वक किया जाना चाहिए क्योंकि यह Project.DurationFormat सेटिंग के आधार पर विभिन्न अवधि लौटाता है। उदाहरण के लिए, GetWork(1.0) 1 घंटे लौटाएगा जब Project.DurationFormat TimeUnitType.Hour है या 1 दिन जब Project.DurationFormat TimeUnitType.Day है। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


निर्दिष्ट संख्या में [TimeUnitType](../../com.aspose.tasks/timeunittype) इकाइयों के साथ [Duration](../../com.aspose.tasks/duration) ऑब्जेक्ट प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | निर्दिष्ट इकाइयों की संख्या। |
| समय इकाई | byte | निर्दिष्ट TimeUnitType मान। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


DurationFormat का मान प्राप्त करता है।

**Returns:**
byte - DurationFormat का मान।
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


EarnedValueMethod का मान प्राप्त करता है।

**Returns:**
int - EarnedValueMethod का मान।
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


ExtendedAttributeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़े विस्तारित विशेषता (कस्टम फ़ील्ड) परिभाषाओं का संग्रह।

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


ExtendedCreationDate का मान प्राप्त करता है।

**Returns:**
java.util.Date - ExtendedCreationDate का मान।
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


FinishDate का मान प्राप्त करता है।

**Returns:**
java.util.Date - FinishDate का मान।
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


FiscalYearStart सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


FyStartDate का मान प्राप्त करता है।

**Returns:**
int - FyStartDate का मान।
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


प्रोजेक्ट की ग्लोबलाइज़ेशन (भाषा-विशिष्ट) सेटिंग्स प्राप्त करता है।

परियोजना में संस्कृति-निर्भर नहीं ऐसे लिटरल या फ़ॉर्मेट का उपयोग करने की अनुशंसित विधि है। हालांकि, यदि कोई परियोजना संस्कृति-विशिष्ट लिटरल का उपयोग करती है, तो इस क्लास का उपयोग गणना इंजन को उन लिटरल को पार्स करने में मदद करने के लिए किया जा सकता है।

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


GUID का मान प्राप्त करता है।

**Returns:**
java.util.UUID - Guid का मान।
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


HonorConstraints सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


HyperlinkBase का मान प्राप्त करता है।

**Returns:**
java.lang.String - HyperlinkBase का मान।
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


InsertedProjectsLikeSummary सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Keywords का मान प्राप्त करता है।

**Returns:**
java.lang.String - Keywords का मान।
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


LastAuthor का मान प्राप्त करता है।

**Returns:**
java.lang.String - LastAuthor का मान।
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


LastPrinted का मान प्राप्त करता है।

**Returns:**
java.util.Date - LastPrinted का मान।
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


LastSaved का मान प्राप्त करता है।

**Returns:**
java.util.Date - LastSaved का मान।
### getManager() {#getManager--}
```
public final String getManager()
```


Manager का मान प्राप्त करता है।

**Returns:**
java.lang.String - Manager का मान।
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


MicrosoftProjectServerURL सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


MinutesPerDay का मान प्राप्त करता है।

**Returns:**
int - MinutesPerDay का मान।
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


MinutesPerWeek का मान प्राप्त करता है।

**Returns:**
int - MinutesPerWeek का मान।
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


MoveCompletedEndsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


MoveCompletedEndsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


MoveRemainingStartsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


MoveRemainingStartsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


MultipleCriticalPaths सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


नाम का मान प्राप्त करता है।

**Returns:**
java.lang.String - Name का मान।
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


NewTaskStartDate का मान प्राप्त करता है।

**Returns:**
int - NewTaskStartDate का मान।
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


NewTasksAreManual सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


NewTasksEffortDriven सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


NewTasksEstimated सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


इस प्रोजेक्ट फ़ाइल से जुड़े या एम्बेड किए गए [OleObject](../../com.aspose/tasks/oleobject) क्लास के इंस्टेंस को शामिल करने वाला संग्रह प्राप्त करता है।

--------------------

केवल mpp फ़ाइल फ़ॉर्मेट के लिए उपलब्ध। यह संग्रह 'Clear' ऑपरेशन को छोड़कर केवल‑पढ़ने‑योग्य है।

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


OutlineCodeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। वह संग्रह जिसमें प्रोजेक्ट से संबंधित आउटलाइन कोड परिभाषाएँ होती हैं।

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


डिफ़ॉल्ट [Timescale](../../com.aspose.tasks/timescale)(Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है।

**Returns:**
int - रेंडर किए जाने वाले पृष्ठों की संख्या।
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


दिए गए [SaveOptions](../../com.aspose.tasks/saveoptions) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पेज काउंट लौटाता है।

--------------------

&gt; ```
&gt; इस उदाहरण में HtmlSaveOptions का इंस्टेंस और परिणामस्वरूप HTML में पृष्ठों की संख्या कंसोल में लिखी जाती है।
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

