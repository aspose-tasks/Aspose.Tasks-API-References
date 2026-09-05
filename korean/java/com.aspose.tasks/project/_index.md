---
title: "프로젝트"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 나타냅니다."
type: docs
weight: 220
url: /ko/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

프로젝트를 나타냅니다.

--------------------

**Project**는 Aspose.Tasks 라이브러리의 핵심 클래스입니다.

지원되는 프로젝트 관리 형식 중 하나인 MPP, MPT, MPX, XML을 읽기 위해 **Project**를 사용할 수 있습니다.

지원되는 형식 중 하나로 기존 문서를 로드하려면 파일 이름이나 스트림을 **Project** 생성자 중 하나에 전달하십시오. 빈 프로젝트를 만들려면 매개변수가 없는 생성자를 호출하십시오.

프로젝트를 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 형식 중 하나로 저장하려면 Save 메서드 오버로드 중 하나를 사용하십시오: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; 이미지: JPEG, PNG, BMP, TIFF, SVG; 텍스트: TXT; 기타: HTML.

프로젝트를 인쇄하려면 [print()](../../com.aspose.tasks/project\#print--) 메서드 오버로드 중 하나를 사용하십시오.

**Project**는 `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), 및 `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-))와 같은 프로젝트 전체 정보를 저장합니다. 이러한 객체 대부분은 **Project** 클래스의 해당 속성을 통해 접근할 수 있습니다.

**Project**는 [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 및 [Calendar](../../com.aspose.tasks/calendar)와 같은 다른 프로젝트 엔터티를 조작하기 위한 진입점을 포함하는 루트 엔터티입니다.

**Project** 엔터티는 타입이 지정된 컬렉션을 통해 접근할 수 있습니다. 예를 들어 `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)) 등.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Project()](#Project--) | 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | 비밀번호로 보호된 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(String projectTemplate)](#Project-java.lang.String-) | 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | 스트림에서 지정된 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | 스트림에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | 템플릿(존재하는 MPP 또는 MPT 파일)에서 지정된 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | 데이터베이스에서 데이터를 읽기 위해, 해당 [DbSettings](../../com.aspose.tasks/dbsettings) 클래스 인스턴스로 지정된 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | 템플릿(존재하는 mpp 또는 mpt 파일)에서 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | 스트림에서 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 이 컨테이너에서 속성이 매핑된 값을 반환합니다. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | 루트 작업을 포함한 모든 프로젝트 작업을 재귀적으로 열거합니다. |
| [getActualsInSync()](#getActualsInSync--) | ActualsInSync가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getAdminProject()](#getAdminProject--) | AdminProject가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | AreEditableActualCosts가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getAuthor()](#getAuthor--) | Author의 값을 가져옵니다. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | AutoAddNewResourcesAndTasks가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | 할당 작업 및 리소스 요율을 사용하여 할당 비용과 남은 비용을 자동으로 계산해야 하는지 여부를 가져옵니다. |
| [getAutolink()](#getAutolink--) | Autolink가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | BaselineForEarnedValue의 값을 가져옵니다. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | 기준선 저장 시간을 반환합니다. |
| [getBuiltInProps()](#getBuiltInProps--) | 프로젝트의 내장 속성 컬렉션을 가져옵니다. |
| [getCalculationMode()](#getCalculationMode--) | 프로젝트의 계산 모드를 가져옵니다. |
| [getCalendar()](#getCalendar--) | Calendar 값을 가져옵니다. |
| [getCalendars()](#getCalendars--) | [CalendarCollection](../../com.aspose.tasks/calendarcollection) 객체를 이 Project 인스턴스에서 가져옵니다. |
| [getCategory()](#getCategory--) | Category의 값을 가져옵니다. |
| [getComments()](#getComments--) | Comments의 값을 가져옵니다. |
| [getCompany()](#getCompany--) | Company의 값을 가져옵니다. |
| [getCreationDate()](#getCreationDate--) | CreationDate의 값을 가져옵니다. |
| [getCriticalPath()](#getCriticalPath--) | 이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | 총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 Critical로 간주합니다. |
| [getCurrencyCode()](#getCurrencyCode--) | CurrencyCode의 값을 가져옵니다. |
| [getCurrencyDigits()](#getCurrencyDigits--) | CurrencyDigits의 값을 가져옵니다. |
| [getCurrencySymbol()](#getCurrencySymbol--) | CurrencySymbol의 값을 가져옵니다. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | CurrencySymbolPosition의 값을 가져옵니다. |
| [getCurrentDate()](#getCurrentDate--) | CurrentDate의 값을 가져옵니다. |
| [getCustomDateFormat()](#getCustomDateFormat--) | CustomDateFormat의 값을 가져옵니다. |
| [getCustomProps()](#getCustomProps--) | 프로젝트의 사용자 정의 속성 컬렉션을 가져옵니다. |
| [getDateFormat()](#getDateFormat--) | DateFormat의 값을 가져옵니다. |
| [getDaysPerMonth()](#getDaysPerMonth--) | DaysPerMonth의 값을 가져옵니다. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | DefaultFinishTime의 값을 가져옵니다. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | DefaultFixedCostAccrual의 값을 가져옵니다. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | DefaultOvertimeRate의 값을 가져옵니다. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | DefaultStandardRate의 값을 가져옵니다. |
| [getDefaultStartTime()](#getDefaultStartTime--) | DefaultStartTime의 값을 가져옵니다. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | DefaultTaskEVMethod의 값을 가져옵니다. |
| [getDefaultTaskType()](#getDefaultTaskType--) | DefaultTaskType의 값을 가져옵니다. |
| [getDefaultView()](#getDefaultView--) | 프로젝트의 기본 보기를 가져옵니다. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 클래스의 인스턴스를 가져옵니다. 이 클래스는 프로젝트 기본 주 작업일 및 작업 시간을 나타내는 컬렉션을 나타냅니다. |
| [getDisplayOptions()](#getDisplayOptions--) | [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) 클래스의 인스턴스를 가져옵니다. |
| [getDuration(double val)](#getDuration-double-) | [Duration](../../com.aspose.tasks/duration) 객체를 가져옵니다. 지정된 단위 수와 프로젝트 설정 [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT)에서 정의된 기본 기간 형식을 사용합니다. |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | [Duration](../../com.aspose.tasks/duration) 객체를 가져옵니다. 지정된 수의 [TimeUnitType](../../com.aspose.tasks/timeunittype) 단위를 사용합니다. |
| [getDurationFormat()](#getDurationFormat--) | DurationFormat의 값을 가져옵니다. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | EarnedValueMethod의 값을 가져옵니다. |
| [getExtendedAttributes()](#getExtendedAttributes--) | ExtendedAttributeDefinitionCollection 객체를 가져옵니다. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | ExtendedCreationDate의 값을 가져옵니다. |
| [getFinishDate()](#getFinishDate--) | FinishDate의 값을 가져옵니다. |
| [getFiscalYearStart()](#getFiscalYearStart--) | FiscalYearStart가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getFyStartDate()](#getFyStartDate--) | FyStartDate의 값을 가져옵니다. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | 프로젝트의 글로벌화(언어별) 설정을 가져옵니다. |
| [getGuid()](#getGuid--) | Guid의 값을 가져옵니다. |
| [getHonorConstraints()](#getHonorConstraints--) | HonorConstraints가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getHyperlinkBase()](#getHyperlinkBase--) | HyperlinkBase의 값을 가져옵니다. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getKeywords()](#getKeywords--) | Keywords의 값을 가져옵니다. |
| [getLastAuthor()](#getLastAuthor--) | LastAuthor의 값을 가져옵니다. |
| [getLastPrinted()](#getLastPrinted--) | LastPrinted의 값을 가져옵니다. |
| [getLastSaved()](#getLastSaved--) | LastSaved의 값을 가져옵니다. |
| [getManager()](#getManager--) | Manager의 값을 가져옵니다. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | MicrosoftProjectServerURL이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getMinutesPerDay()](#getMinutesPerDay--) | MinutesPerDay의 값을 가져옵니다. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | MinutesPerWeek의 값을 가져옵니다. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | MoveCompletedEndsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | MoveCompletedEndsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | MoveRemainingStartsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | MoveRemainingStartsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | MultipleCriticalPaths가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getName()](#getName--) | Name의 값을 가져옵니다. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | NewTaskStartDate의 값을 가져옵니다. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | NewTasksAreManual이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | NewTasksEffortDriven가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | NewTasksEstimated가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getOleObjects()](#getOleObjects--) | 이 프로젝트 파일에 연결되거나 포함된 [OleObject](../../com.aspose/tasks/oleobject) 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다. |
| [getOutlineCodes()](#getOutlineCodes--) | OutlineCodeDefinitionCollection 객체를 가져옵니다. |
| [getPageCount()](#getPageCount--) | 기본 [Timescale](../../com.aspose.tasks/timescale)(Days)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | 주어진 [SaveOptions](../../com.aspose.tasks/saveoptions)를 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | 주어진 [Timescale](../../com.aspose.tasks/timescale) 및 [PresentationFormat](../../com.aspose.tasks/presentationformat)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | 주어진 [Timescale](../../com.aspose.tasks/timescale) 및 [PageSize](../../com.aspose.tasks/pagesize)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | 주어진 [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) 및 날짜 범위를 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | 기본 [Timescale](../../com.aspose.tasks/timescale)(Days) 및 주어진 [PresentationFormat](../../com.aspose.tasks/presentationformat)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | 주어진 [Timescale](../../com.aspose.tasks/timescale)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | 지정된 작업의 선행 작업인 작업 링크 컬렉션을 반환합니다. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Primavera 파일에서 읽은 프로젝트에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | ProjectExternallyEdited가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | 스트림에서 프로젝트 파일 정보를 가져옵니다. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | 파일에서 프로젝트 파일 정보를 읽습니다. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getResourceAssignments()](#getResourceAssignments--) | ResourceAssignmentCollection 객체를 가져옵니다. |
| [getResourceFilters()](#getResourceFilters--) | 리소스 기반 필터 정의를 모두 가져옵니다. |
| [getResourceGroups()](#getResourceGroups--) | 리소스 기반 그룹 정의를 모두 가져옵니다. |
| [getResources()](#getResources--) | ResourceCollection 객체를 가져옵니다. |
| [getRevision()](#getRevision--) | Revision 값을 가져옵니다. |
| [getRootTask()](#getRootTask--) | 작업 트리의 루트를 가져옵니다. |
| [getSaveVersion()](#getSaveVersion--) | SaveVersion 값을 가져옵니다. |
| [getScheduleFromStart()](#getScheduleFromStart--) | ScheduleFromStart가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | ShowProjectSummaryTask가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getSpreadActualCost()](#getSpreadActualCost--) | SpreadActualCost가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | SpreadPercentComplete가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getStartDate()](#getStartDate--) | StartDate 값을 가져옵니다. |
| [getStatusDate()](#getStatusDate--) | StatusDate 값을 가져옵니다. |
| [getSubject()](#getSubject--) | Subject 값을 가져옵니다. |
| [getTables()](#getTables--) | [Table](../../com.aspose.tasks/table) 객체 목록을 가져옵니다. |
| [getTaskFilters()](#getTaskFilters--) | 작업 기반 필터 정의를 모두 가져옵니다. |
| [getTaskGroups()](#getTaskGroups--) | 작업 기반 그룹 정의를 모두 가져옵니다. |
| [getTaskLinks()](#getTaskLinks--) | [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) 객체를 가져옵니다. |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getTemplate()](#getTemplate--) | Template의 값을 가져옵니다. |
| [getTimescaleFinish()](#getTimescaleFinish--) | TimescaleFinish의 값을 가져옵니다. |
| [getTimescaleStart()](#getTimescaleStart--) | TimescaleStart의 값을 가져옵니다. |
| [getTitle()](#getTitle--) | Title의 값을 가져옵니다. |
| [getUid()](#getUid--) | Uid의 값을 가져옵니다. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getVbaProject()](#getVbaProject--) | `VbaProject` 클래스의 인스턴스를 가져옵니다([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | [View](../../com.aspose.tasks/view) 객체 목록을 가져옵니다. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | 프로젝트에 대한 WBS 코드 정의를 가져옵니다. |
| [getWeekStartDay()](#getWeekStartDay--) | WeekStartDay의 값을 가져옵니다. |
| [getWork(double val)](#getWork-double-) | 지정된 `double` 값과 기본 작업 형식을 사용하여 [Duration](../../com.aspose.tasks/duration) 객체를 가져옵니다. |
| [getWorkFormat()](#getWorkFormat--) | WorkFormat의 값을 가져옵니다. |
| [print()](#print--) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 기본 프린터 설정으로 프로젝트를 기본 프린터에 인쇄합니다. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 기본 프린터 설정 및 사용자 지정 저장 옵션으로 프로젝트를 기본 프린터에 인쇄합니다. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정 및 사용자 지정 저장 옵션에 따라 프로젝트를 인쇄합니다. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정, 사용자 지정 저장 옵션 및 지정된 문서 이름에 따라 프로젝트를 인쇄합니다. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [print(String printerName)](#print-java.lang.String-) | 표준 (no User Interface) 인쇄 컨트롤러를 사용하여 기본 프린터 설정으로 지정된 프린터에 프로젝트를 인쇄합니다. |
| [recalculate()](#recalculate--) | 모든 프로젝트 작업 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다. |
| [recalculate(boolean validate)](#recalculate-boolean-) | 선택적 검증을 포함하여 모든 프로젝트 작업 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다. |
| [recalculateResourceFields()](#recalculateResourceFields--) | 리소스의 ID, 시작 및 완료를 다시 계산합니다. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | 리소스의 시작 및 완료를 다시 계산합니다. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | 프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다. |
| [renumberWBSCode()](#renumberWBSCode--) | 모든 작업의 WBS 코드를 다시 번호 매깁니다. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | 전달된 작업의 WBS 코드를 다시 번호 매깁니다. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | 지정된 날짜 이후에 시작하도록 완료되지 않은 프로젝트 작업을 재조정합니다. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | 지정된 날짜 이후에 시작하도록 지정된 작업 목록에 대한 미완료 작업을 다시 일정합니다. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | 지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 프로젝트 데이터를 스트림에 저장합니다. |
| [save(String filename)](#save-java.lang.String-) | 프로젝트 데이터를 mpp 형식의 파일에 저장합니다. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | 지정된 저장 옵션을 사용하여 문서를 파일에 저장합니다. |
| [save(String filename, int format)](#save-java.lang.String-int-) | 프로젝트 데이터를 파일에 저장합니다. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | 프로젝트를 템플릿으로 지정된 스트림에 저장합니다. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | 프로젝트를 템플릿으로 지정된 스트림에 저장합니다. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | 프로젝트를 템플릿으로 지정된 파일 경로에 저장합니다. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | 프로젝트를 템플릿으로 저장합니다. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | 프로젝트 개요 보고서를 스트림에 저장합니다. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | 지정된 유형의 프로젝트 보고서를 지정된 스트림에 저장합니다. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | 프로젝트 개요 보고서를 PDF 파일에 저장합니다. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | 지정된 유형의 프로젝트 보고서를 PDF 형식으로 지정된 파일 경로에 저장합니다. |
| [selectAllChildTasks()](#selectAllChildTasks--) | 루트 작업의 모든 하위 작업을 재귀적으로 수집합니다. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | ActualsInSync가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | AdminProject가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | AreEditableActualCosts가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Author 값을 설정합니다. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | AutoAddNewResourcesAndTasks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | 할당 작업 및 리소스 요금을 사용하여 할당 비용과 남은 비용을 자동으로 계산할지 여부를 설정합니다. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Autolink가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setBaseline(int baselineType)](#setBaseline-int-) | 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | 선택된 작업에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | BaselineForEarnedValue 값을 설정합니다. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | 기준선 저장 시간을 설정합니다. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | 프로젝트의 계산 모드를 설정합니다. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar의 값을 설정합니다. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Category의 값을 설정합니다. |
| [setComments(String value)](#setComments-java.lang.String-) | Comments의 값을 설정합니다. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Company의 값을 설정합니다. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | CreationDate의 값을 설정합니다. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | 총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 Critical로 간주합니다. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | CurrencyCode의 값을 설정합니다. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | CurrencyDigits의 값을 설정합니다. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | CurrencySymbol의 값을 설정합니다. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | CurrencySymbolPosition의 값을 설정합니다. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | CurrentDate의 값을 설정합니다. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | CustomDateFormat의 값을 설정합니다. |
| [setDateFormat(int value)](#setDateFormat-int-) | DateFormat의 값을 설정합니다. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | DaysPerMonth의 값을 설정합니다. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | DefaultFinishTime의 값을 설정합니다. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | DefaultFixedCostAccrual의 값을 설정합니다. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | DefaultOvertimeRate의 값을 설정합니다. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | DefaultStandardRate의 값을 설정합니다. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | DefaultStartTime의 값을 설정합니다. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | DefaultTaskEVMethod의 값을 설정합니다. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | DefaultTaskType의 값을 설정합니다. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | 프로젝트의 기본 보기를 설정합니다. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | DurationFormat의 값을 설정합니다. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | EarnedValueMethod의 값을 설정합니다. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | ExtendedCreationDate의 값을 설정합니다. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | FinishDate의 값을 설정합니다. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | FiscalYearStart가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | FyStartDate의 값을 설정합니다. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | 프로젝트의 글로벌화(언어별) 설정을 설정합니다. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Guid의 값을 설정합니다. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | HonorConstraints가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | HyperlinkBase의 값을 설정합니다. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Keywords의 값을 설정합니다. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | LastAuthor의 값을 설정합니다. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | LastPrinted의 값을 설정합니다. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | LastSaved의 값을 설정합니다. |
| [setManager(String value)](#setManager-java.lang.String-) | Manager의 값을 설정합니다. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | MicrosoftProjectServerURL이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | MinutesPerDay의 값을 설정합니다. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | MinutesPerWeek의 값을 설정합니다. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | MoveCompletedEndsBack이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | MoveCompletedEndsForward가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | MoveRemainingStartsBack이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | MoveRemainingStartsForward가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | MultipleCriticalPaths가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setName(String value)](#setName-java.lang.String-) | Name의 값을 설정합니다. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | NewTaskStartDate의 값을 설정합니다. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | NewTasksAreManual이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | NewTasksEffortDriven가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | NewTasksEstimated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | ProjectExternallyEdited가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setRevision(int value)](#setRevision-int-) | Revision 값을 설정합니다. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | SaveVersion 값을 설정합니다. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | ScheduleFromStart가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | ShowProjectSummaryTask가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | SpreadActualCost가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | SpreadPercentComplete가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | StartDate 값을 설정합니다. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | StatusDate 값을 설정합니다. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Subject 값을 설정합니다. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Template 값을 설정합니다. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | TimescaleFinish 값을 설정합니다. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | TimescaleStart 값을 설정합니다. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Title 값을 설정합니다. |
| [setUid(String value)](#setUid-java.lang.String-) | Uid의 값을 설정합니다. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | 프로젝트에 대한 WBS 코드 정의를 설정합니다. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | WeekStartDay 값을 설정합니다. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | WorkFormat 값을 설정합니다. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | 전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | 지정된 작업 목록에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |
### Project() {#Project--}
```
public Project()
```


새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


비밀번호로 보호된 템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 프로젝트를 생성할 템플릿 경로입니다. |
|  | protectionPassword | java.lang.String | 보호 암호. |

--------------------

현재는 MSP 2003 파일 형식에 대해서만 암호로 보호된 파일을 읽는 것이 지원됩니다. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 프로젝트를 생성할 템플릿 경로입니다. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


스트림에서 지정된 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 프로젝트 java.io.InputStream 클래스의 스트림 |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Primavera 형식 (XER 또는 XML) 읽기를 사용자 정의할 수 있는 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 클래스의 지정된 인스턴스. |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 프로젝트를 생성할 템플릿 경로입니다. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML 구문 분석 오류를 처리하기 위한 지정된 콜백 메서드. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


스트림에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 템플릿을 로드하기 위한 java.io.InputStream. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


템플릿(존재하는 MPP 또는 MPT 파일)에서 지정된 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 프로젝트를 생성할 템플릿 경로 |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | 지정된 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 클래스의 인스턴스. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


데이터베이스에서 데이터를 읽기 위해, 해당 [DbSettings](../../com.aspose.tasks/dbsettings) 클래스 인스턴스로 지정된 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | 지정된 [DbSettings](../../com.aspose.tasks/dbsettings) 클래스의 인스턴스. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 템플릿을 로드하기 위한 java.io.InputStream. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML 구문 분석 오류를 처리하기 위한 지정된 콜백 메서드. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


템플릿(존재하는 mpp 또는 mpt 파일)에서 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 템플릿을 로드하기 위한 java.io.InputStream. |
|  | protectionPassword | java.lang.String | 보호 암호. |

--------------------

현재는 MSP 2003 파일 형식에 대해서만 암호로 보호된 파일을 읽는 것이 지원됩니다. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


템플릿(존재하는 mpp 또는 mpt 파일)에서 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 프로젝트를 생성할 템플릿 경로 |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스의 인스턴스. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


스트림에서 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스 인스턴스를 사용하여 새로운 [Project](../../com.aspose.tasks/project) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 프로젝트 java.io.InputStream 클래스의 스트림 |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | 지정된 [LoadOptions](../../com.aspose.tasks/loadoptions) 클래스의 인스턴스 |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


이 컨테이너에서 속성이 매핑된 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키. 속성 키를 가져오기 위해서는 [Prj](../../com.aspose.tasks/prj)를 사용합니다. |

**Returns:**
T - 이 컨테이너에서 속성이 매핑되는 값입니다.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키. 속성 키를 가져오기 위해서는 [Prj](../../com.aspose.tasks/prj)를 사용합니다. |
| val | T | 값입니다. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | 데이터를 복사할 다른 프로젝트. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | 데이터를 복사할 다른 프로젝트. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | 복사 프로세스를 제어하기 위한 복사 옵션. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


루트 작업을 포함한 모든 프로젝트 작업을 재귀적으로 열거합니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - 모든 프로젝트 작업을 반복할 수 있는 IEnumerable.

--------------------

[selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) 메서드에 비해 작업을 반복하는 보다 가벼운 방법을 제공하며, 모든 작업에 대한 메모리를 할당하지 않습니다.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


ActualsInSync가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


AdminProject가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


AreEditableActualCosts가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Author의 값을 가져옵니다.

**Returns:**
java.lang.String - 작성자 값.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


AutoAddNewResourcesAndTasks가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


할당 작업 및 리소스 요율을 사용하여 할당 비용과 남은 비용을 자동으로 계산해야 하는지 여부를 가져옵니다.

**Returns:**
boolean - 할당 작업 및 리소스 요금을 사용하여 할당 비용과 남은 비용을 자동으로 계산할지 여부.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Autolink가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


BaselineForEarnedValue의 값을 가져옵니다.

**Returns:**
int - BaselineForEarnedValue 값.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


베이스라인 저장 시간을 반환합니다. 베이스라인이 저장되지 않은 경우 DateTime.MinValue (00:00:00.0000000 UTC, 0001년 1월 1일)를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| baselineNumber | int | 베이스라인 번호 [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - 베이스라인의 마지막 저장 날짜 및 시간.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


프로젝트의 내장 속성 컬렉션을 가져옵니다.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


프로젝트의 계산 모드를 가져옵니다. `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) 열거형의 값 중 하나일 수 있습니다.

**Returns:**
int - 프로젝트의 계산 모드.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar 값을 가져옵니다.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


[CalendarCollection](../../com.aspose.tasks/calendarcollection) 객체를 이 Project 인스턴스에서 가져옵니다.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Category의 값을 가져옵니다.

**Returns:**
java.lang.String - Category 값.
### getComments() {#getComments--}
```
public final String getComments()
```


Comments의 값을 가져옵니다.

**Returns:**
java.lang.String - Comments 값.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Company의 값을 가져옵니다.

**Returns:**
java.lang.String - Company 값.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


CreationDate의 값을 가져옵니다.

**Returns:**
java.util.Date - CreationDate 값.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

이는 O(n) 연산이며, 여기서 n은 프로젝트의 작업 수입니다.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 Critical로 간주합니다.

**Returns:**
int - 작업이 중요하다고 간주되는 총 여유 시간(일)의 최대값
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


CurrencyCode의 값을 가져옵니다.

**Returns:**
java.lang.String - CurrencyCode 값.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


CurrencyDigits의 값을 가져옵니다.

**Returns:**
int - CurrencyDigits 값.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


CurrencySymbol의 값을 가져옵니다.

**Returns:**
java.lang.String - CurrencySymbol 값.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


CurrencySymbolPosition의 값을 가져옵니다.

**Returns:**
int - CurrencySymbolPosition 값.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


CurrentDate의 값을 가져옵니다.

**Returns:**
java.util.Date - CurrentDate 값.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


CustomDateFormat의 값을 가져옵니다.

**Returns:**
java.lang.String - CustomDateFormat 값.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


프로젝트의 사용자 정의 속성 컬렉션을 가져옵니다.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


DateFormat의 값을 가져옵니다.

**Returns:**
int - DateFormat 값.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


DaysPerMonth의 값을 가져옵니다.

**Returns:**
int - DaysPerMonth 값.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


DefaultFinishTime의 값을 가져옵니다.

**Returns:**
java.util.Date - DefaultFinishTime 값.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


DefaultFixedCostAccrual의 값을 가져옵니다.

**Returns:**
int - DefaultFixedCostAccrual 값.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


DefaultOvertimeRate의 값을 가져옵니다.

**Returns:**
double - DefaultOvertimeRate 값.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


DefaultStandardRate의 값을 가져옵니다.

**Returns:**
double - DefaultStandardRate 값.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


DefaultStartTime의 값을 가져옵니다.

**Returns:**
java.util.Date - DefaultStartTime 값.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


DefaultTaskEVMethod의 값을 가져옵니다.

**Returns:**
int - DefaultTaskEVMethod 값.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


DefaultTaskType의 값을 가져옵니다.

**Returns:**
int - DefaultTaskType 값.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


프로젝트의 기본 보기를 가져옵니다.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 클래스의 인스턴스를 가져옵니다. 이 클래스는 프로젝트 기본 주 작업일 및 작업 시간을 나타내는 컬렉션을 나타냅니다.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

데이터는 mpp 파일에만 포함되어 있으며 (xml에는 포함되지 않음).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


[Duration](../../com.aspose.tasks/duration) 객체를 가져옵니다. 지정된 단위 수와 프로젝트 설정 [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT)에서 정의된 기본 기간 형식을 사용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | val | double | 지정된 단위 수. |

--------------------

이 메서드는 Project.DurationFormat 설정에 따라 다른 기간을 반환하므로 신중히 사용해야 합니다. 예를 들어, Project.DurationFormat이 TimeUnitType.Hour인 경우 GetWork(1.0)은 1시간을 반환하고, Project.DurationFormat이 TimeUnitType.Day인 경우 1일을 반환합니다. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


[Duration](../../com.aspose.tasks/duration) 객체를 가져옵니다. 지정된 수의 [TimeUnitType](../../com.aspose.tasks/timeunittype) 단위를 사용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| val | double | 지정된 단위 수. |
| 시간 단위 | 바이트 | 지정된 TimeUnitType 값. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


DurationFormat의 값을 가져옵니다.

**Returns:**
byte - DurationFormat의 값.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


EarnedValueMethod의 값을 가져옵니다.

**Returns:**
int - EarnedValueMethod의 값.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 확장 속성(사용자 정의 필드) 정의 컬렉션입니다.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


ExtendedCreationDate의 값을 가져옵니다.

**Returns:**
java.util.Date - ExtendedCreationDate의 값.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


FinishDate의 값을 가져옵니다.

**Returns:**
java.util.Date - FinishDate의 값.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


FiscalYearStart가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


FyStartDate의 값을 가져옵니다.

**Returns:**
int - FyStartDate의 값.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


프로젝트의 글로벌화(언어별) 설정을 가져옵니다.

프로젝트 전체에서 문화에 구애받지 않는 리터럴이나 형식을 사용하는 것이 권장됩니다. 그러나 프로젝트가 문화별 리터럴을 사용하는 경우, 이 클래스를 사용하여 계산 엔진이 해당 리터럴을 구문 분석하도록 도울 수 있습니다.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Guid의 값을 가져옵니다.

**Returns:**
java.util.UUID - Guid의 값.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


HonorConstraints가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


HyperlinkBase의 값을 가져옵니다.

**Returns:**
java.lang.String - HyperlinkBase의 값.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Keywords의 값을 가져옵니다.

**Returns:**
java.lang.String - Keywords의 값.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


LastAuthor의 값을 가져옵니다.

**Returns:**
java.lang.String - LastAuthor의 값.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


LastPrinted의 값을 가져옵니다.

**Returns:**
java.util.Date - LastPrinted의 값.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


LastSaved의 값을 가져옵니다.

**Returns:**
java.util.Date - LastSaved의 값.
### getManager() {#getManager--}
```
public final String getManager()
```


Manager의 값을 가져옵니다.

**Returns:**
java.lang.String - Manager의 값.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


MicrosoftProjectServerURL이 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


MinutesPerDay의 값을 가져옵니다.

**Returns:**
int - MinutesPerDay의 값.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


MinutesPerWeek의 값을 가져옵니다.

**Returns:**
int - MinutesPerWeek의 값.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


MoveCompletedEndsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


MoveCompletedEndsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


MoveRemainingStartsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


MoveRemainingStartsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


MultipleCriticalPaths가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Name의 값을 가져옵니다.

**Returns:**
java.lang.String - Name의 값.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


NewTaskStartDate의 값을 가져옵니다.

**Returns:**
int - NewTaskStartDate의 값.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


NewTasksAreManual이 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


NewTasksEffortDriven가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


NewTasksEstimated가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


이 프로젝트 파일에 연결되거나 포함된 [OleObject](../../com.aspose/tasks/oleobject) 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다.

--------------------

mpp 파일 형식에서만 사용할 수 있습니다. 이 컬렉션은 'Clear' 작업을 제외하고는 읽기 전용입니다.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


OutlineCodeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 개요 코드 정의 컬렉션입니다.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


기본 [Timescale](../../com.aspose.tasks/timescale)(Days)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

**Returns:**
int - 렌더링할 페이지 수.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


주어진 [SaveOptions](../../com.aspose.tasks/saveoptions)를 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

--------------------

&gt; ```
&gt; 이 예제에서는 HtmlSaveOptions 인스턴스와 결과 HTML의 페이지 수가 콘솔에 출력됩니다.
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

