---
title: Project
second_title: .NET API 참조용 Aspose.Tasks
description: 프로젝트를 나타냅니다.
type: docs
weight: 1190
url: /ko/net/aspose.tasks/project/
---
## Project class

프로젝트를 나타냅니다.

```csharp
public class Project
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Project](project/#constructor)() | 의 새 인스턴스를 초기화합니다.`Project` 클래스. |
| [Project](project/#constructor_1)(DbSettings) | 의 새 인스턴스를 초기화합니다.`Project` 인스턴스에 의해 지정된 데이터베이스에서 데이터를 읽는 클래스[`DbSettings`](../../aspose.tasks.connectivity/dbsettings/) 클래스. |
| [Project](project/#constructor_2)(Stream) | 의 새 인스턴스를 초기화합니다.`Project` stream. 의 클래스 |
| [Project](project/#constructor_7)(StreamReader) | 의 새 인스턴스를 초기화합니다.`Project` StreamReader instance. 의 클래스 |
| [Project](project/#constructor_8)(string) | 의 새 인스턴스를 초기화합니다.`Project` 템플릿의 클래스(기존 mpp 또는 mpt 파일). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | 의 새 인스턴스를 초기화합니다.`Project` 지정된 인스턴스가 있는 Stream 의 클래스[`LoadOptions`](../loadoptions/) 클래스. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | 의 새 인스턴스를 초기화합니다.`Project`템플릿의 클래스(기존 mpp 또는 mpt 파일). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | 의 새 인스턴스를 초기화합니다.`Project` 지정된 인스턴스가 있는 Stream 의 클래스[`PrimaveraReadOptions`](../primaverareadoptions/) 클래스. |
| [Project](project/#constructor_6)(Stream, string) | 의 새 인스턴스를 초기화합니다.`Project`템플릿의 클래스(기존 mpp 또는 mpt 파일). |
| [Project](project/#constructor_9)(string, LoadOptions) | 의 새 인스턴스를 초기화합니다.`Project` 지정된 인스턴스가 있는 템플릿의 클래스(기존 mpp 또는 mpt 파일) [`LoadOptions`](../loadoptions/) 클래스. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | 의 새 인스턴스를 초기화합니다.`Project` 템플릿의 클래스(기존 mpp 또는 mpt 파일). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | 의 새 인스턴스를 초기화합니다.`Project` 지정된 인스턴스가 있는 템플릿의 클래스(기존 MPP 또는 MPT 파일) [`PrimaveraReadOptions`](../primaverareadoptions/) 클래스. |
| [Project](project/#constructor_12)(string, string) | 의 새 인스턴스를 초기화합니다.`Project` 암호로 보호된 템플릿의 클래스(기존 mpp 또는 mpt 파일). |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | ActualsInSync 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | AdminProject 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | AreEditableActualCosts가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Author. 의 값을 가져오거나 설정합니다. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | AutoAddNewResourcesAndTasks 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | 자동 링크 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | BaselineForEarnedValue의 값을 가져오거나 설정합니다. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | 프로젝트의 기본 제공 속성 컬렉션을 가져옵니다. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | 프로젝트의 계산 모드를 가져오거나 설정합니다. 다음 값 중 하나일 수 있습니다.[`CalculationMode`](./calculationmode/) 열거형. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Calendar. 의 값을 가져오거나 설정합니다. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | 가져오기[`CalendarCollection`](../calendarcollection/) 이 프로젝트 instance. 의 객체 |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Category. 의 값을 가져오거나 설정합니다. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | 설명 값을 가져오거나 설정합니다. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Company. 값을 가져오거나 설정합니다. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | CreationDate 값을 가져오거나 설정합니다. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | 이 프로젝트의 중요 경로를 구성하는 중요 작업 목록이 포함된 컬렉션을 가져옵니다. 이것은 O(n) 작업이며 여기서 n은 프로젝트의 작업 수입니다. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | CriticalSlackLimit 값을 가져오거나 설정합니다. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | CurrencyCode. 의 값을 가져오거나 설정합니다. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | CurrencyDigits. 의 값을 가져오거나 설정합니다. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | CurrencySymbol. 의 값을 가져오거나 설정합니다. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | CurrencySymbolPosition. 의 값을 가져오거나 설정합니다. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | CurrentDate 값을 가져오거나 설정합니다. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | CustomDateFormat. 의 값을 가져오거나 설정합니다. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | 프로젝트의 사용자 지정 속성 컬렉션을 가져옵니다. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | DateFormat. 의 값을 가져오거나 설정합니다. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | DaysPerMonth. 값을 가져오거나 설정합니다. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | DefaultFinishTime. 값을 가져오거나 설정합니다. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | DefaultFixedCostAccrual. 값을 가져오거나 설정합니다. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | DefaultOvertimeRate 값을 가져오거나 설정합니다. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | DefaultStandardRate 값을 가져오거나 설정합니다. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | DefaultStartTime의 값을 가져오거나 설정합니다. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | DefaultTaskEVMethod. 의 값을 가져오거나 설정합니다. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | DefaultTaskType. 의 값을 가져오거나 설정합니다. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | 프로젝트의 기본 보기를 가져오거나 설정합니다. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | 인스턴스를 가져옵니다.[`WeekDayCollection`](../weekdaycollection/) 프로젝트 기본 주 작업일 및 작업 시간 모음을 나타내는 클래스입니다. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | 인스턴스를 가져옵니다.[`ProjectDisplayOptions`](../projectdisplayoptions/) 클래스. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | DurationFormat. 의 값을 가져오거나 설정합니다. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | EarnedValueMethod. 의 값을 가져오거나 설정합니다. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 확장 속성(사용자 정의 필드) 정의 모음입니다. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | ExtendedCreationDate 값을 가져오거나 설정합니다. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | FinishDate 값을 가져오거나 설정합니다. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | FiscalYearStart 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | FyStartDate 값을 가져오거나 설정합니다. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Guid 값을 가져오거나 설정합니다. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | HonorConstraints 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | HyperlinkBase. 의 값을 가져오거나 설정합니다. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | 키워드의 값을 가져오거나 설정합니다. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | LastAuthor. 의 값을 가져오거나 설정합니다. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | LastPrinted. 의 값을 가져오거나 설정합니다. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | LastSaved. 의 값을 가져오거나 설정합니다. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Manager. 의 값을 가져오거나 설정합니다. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | MicrosoftProjectServerURL이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | MinutesPerDay. 의 값을 가져오거나 설정합니다. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | MinutesPerWeek의 값을 가져오거나 설정합니다. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | MoveCompletedEndsBack이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | MoveCompletedEndsForward가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | MoveRemainingStartsBack 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | MoveRemainingStartsForward 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | MultipleCriticalPaths 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Name. 의 값을 가져오거나 설정합니다. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | NewTasksAreManual 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | NewTasksEffortDriven 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | NewTasksEstimated 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | NewTaskStartDate 값을 가져오거나 설정합니다. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | 인스턴스가 포함된 컬렉션을 가져옵니다.[`OleObject`](../oleobject/) 이 프로젝트 파일에 링크되거나 내장된 클래스. mpp 파일 형식에만 사용할 수 있습니다. 이 컬렉션은 '지우기' 작업을 제외하고는 읽기 전용입니다. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | OutlineCodeDefinitionCollection 개체를 가져옵니다. 프로젝트와 연결된 개요 코드 정의 컬렉션입니다. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | ProjectExternallyEdited 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | ResourceAssignmentCollection 개체를 가져옵니다. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | 모든 리소스 기반 필터 정의를 가져옵니다. ResourceFilters는[`Filter`](../filter/) 객체. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | 리소스 기반 그룹 정의를 모두 가져옵니다. ResourceGroups는[`Group`](../group/) 객체. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | ResourceCollection 개체를 가져옵니다. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Revision. 의 값을 가져오거나 설정합니다. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | 작업 트리의 루트를 가져옵니다. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | SaveVersion. 의 값을 가져오거나 설정합니다. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | ScheduleFromStart 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | ShowProjectSummaryTask 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | SpreadActualCost 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | SpreadPercentComplete 설정 여부를 나타내는 값을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | StartDate 값을 가져오거나 설정합니다. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | StatusDate 값을 가져오거나 설정합니다. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | 제목 값을 가져오거나 설정합니다. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | 목록을 가져옵니다.[`Table`](../table/) 객체. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | 모든 작업 기반 필터 정의를 가져옵니다. TaskFilters는[`Filter`](../filter/) 객체. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | 모든 작업 기반 그룹 정의를 가져옵니다. TaskGroups는[`Group`](../group/) 객체. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | 가져오기[`TaskLinkCollection`](../tasklinkcollection/) object. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Template. 의 값을 가져오거나 설정합니다. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | TimescaleFinish. 의 값을 가져오거나 설정합니다. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | TimescaleStart. 의 값을 가져오거나 설정합니다. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | 제목 값을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Uid 값을 가져오거나 설정합니다. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | 인스턴스를 가져옵니다.[`VbaProject`](./vbaproject/) 클래스. |
| [Views](../../aspose.tasks/project/views/) { get; } | 목록을 가져옵니다.[`View`](../view/) 객체. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | 프로젝트에 대한 WBS 코드 정의를 가져오거나 설정합니다. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | WeekStartDay의 값을 가져오거나 설정합니다. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | WorkFormat. 의 값을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | 루트 작업을 포함하여 프로젝트의 모든 작업을 재귀적으로 열거합니다. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | 이 컨테이너에서 속성이 매핑된 값을 반환합니다. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | 기본 저장 시간을 반환합니다. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | 가져오기[`Duration`](../duration/) 지정된 단위 수와 프로젝트 설정에 정의된 기본 기간 형식을 가진 객체[`DurationFormat`](../prj/durationformat/) . |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | 가져오기[`Duration`](../duration/) 지정된 수의 객체[`TimeUnitType`](../timeunittype/) 단위. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | 가져오기[`Duration`](../duration/) 지정된 객체TimeSpan 값 및 지정[`TimeUnitType`](../timeunittype/) 값. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | 기본값을 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) (일). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | 기본값을 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) (일) 및 주어진[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | 주어진 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`SaveOptions`](../../aspose.tasks.saving/saveoptions/) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | 주어진 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | 주어진 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) 그리고[`PageSize`](../../aspose.tasks.visualization/pagesize/) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | 주어진 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) 그리고[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | 주어진 사용하여 렌더링할 프로젝트의 페이지 수를 반환합니다.[`Timescale`](../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 및 날짜 범위. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | 지정된 작업의 선행 작업인 작업 링크 모음을 반환합니다. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | 가져오기[`Duration`](../duration/) 지정된 객체Double 값 및 기본 작업 형식. |
| [Print](../../aspose.tasks/project/print/#print)() | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터 설정으로 기본 프린터로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터 설정 및 사용자 지정 저장 옵션을 사용하여 기본 프린터로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터 설정으로 지정된 프린터로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정 및 사용자 지정 저장 옵션에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정, 사용자 지정 저장 옵션 및 지정된 문서 이름에 따라 프로젝트를 인쇄합니다. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | 모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜, 조기/지연 날짜 설정, 여유 시간, 작업 및 비용 필드를 계산합니다. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | 모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜, 조기/지연 날짜 설정, 선택적 유효성 검사를 통해 슬랙, 작업 및 비용 필드를 다시 예약합니다. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | 리소스의 Id, 시작 및 종료를 다시 계산합니다. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish/)() | 자원의 시작과 끝을 다시 계산합니다. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | 프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | 모든 작업의 WBS 코드를 다시 매깁니다. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | 전달된 작업의 WBS 코드 번호를 다시 매깁니다. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | 완료되지 않은 프로젝트 작업을 지정된 날짜 이후에 시작하도록 일정을 조정합니다. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | 지정된 날짜 이후에 시작하도록 지정된 작업 목록에 대해 완료되지 않은 작업 일정을 변경합니다. |
| [Save](../../aspose.tasks/project/save/#save_3)(string) | 프로젝트 데이터를 mpp 형식의 파일로 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, MPPSaveOptions) | 지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SaveFileFormat) | 스트림에 프로젝트 데이터를 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_2)(Stream, SaveOptions) | 지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, MPPSaveOptions) | 지정된 저장 옵션을 사용하여 문서를 mpp 파일 형식으로 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_5)(string, SaveFileFormat) | 프로젝트 데이터를 파일에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_6)(string, SaveOptions) | 지정된 저장 옵션을 사용하여 문서를 파일로 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | 프로젝트를 지정된 스트림에 템플릿으로 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | 지정된 파일 경로에 프로젝트를 템플릿으로 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | 프로젝트를 지정된 스트림에 템플릿으로 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | 프로젝트를 템플릿으로 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | 프로젝트 개요 보고서를 스트림에 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | 프로젝트 개요 보고서를 PDF 파일로 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | 지정된 유형의 프로젝트 보고서를 지정된 스트림에 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | 지정된 파일 경로에 지정된 유형의 프로젝트 보고서를 PDF 형식으로 저장합니다. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | 루트 작업의 모든 자식 작업을 재귀적으로 수집합니다. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | 선택한 작업에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | 기본 저장 시간을 설정합니다. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | 전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | 지정된 작업 목록에 대해 지정된 날짜까지 모든 작업이 완료된 것으로 업데이트합니다. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | 스트림에서 프로젝트 파일 정보를 가져옵니다. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | 파일에서 프로젝트 파일 정보를 읽습니다. |

### 비고

그만큼 **프로젝트** Aspose.Tasks 라이브러리의 중심 클래스입니다.

사용할 수 있음 **프로젝트**지원되는 프로젝트 관리 형식 중 하나 읽기: MPP, MPT, MPX, XML.

지원되는 형식으로 기존 문서를 로드하려면 파일 이름 또는 스트림을 **프로젝트** 생성자. 빈 프로젝트를 만들려면 매개 변수가 없는 생성자를 호출합니다.

Save 메서드 오버로드 중 하나를 사용하여 다음 중 하나에 프로젝트를 저장합니다.[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) 형식: Primavera: P6 XML, PM XER; 마이크로소프트 엑셀: XLSX, XML; 고정 레이아웃: PDF; 이미지: JPEG, PNG, BMP, TIFF, SVG; 텍스트: TXT; 기타: HTML.

프로젝트를 인쇄하려면 다음 중 하나를 사용하십시오.[`Print`](./print/) 메소드 오버로드.

그만큼 **프로젝트** 다음과 같은 프로젝트 전체 정보를 저장합니다.[`Views`](./views/) , [`BuiltInProps`](./builtinprops/) ,[`CustomProps`](./customprops/) , 그리고[`ExtendedAttributes`](./extendedattributes/) . 이러한 개체의 대부분은 해당 속성을 통해 액세스할 수 있습니다. **프로젝트** 수업.

그만큼 **프로젝트**다음과 같은 다른 프로젝트 엔터티를 조작하기 위한 진입점을 포함하는 루트 엔터티입니다.[`Task`](../task/) ,[`Resource`](../resource/) ,[`ResourceAssignment`](../resourceassignment/) ,[`ExtendedAttribute`](../extendedattribute/) 그리고[`Calendar`](../calendar/).

**프로젝트** 예를 들어 유형이 지정된 컬렉션을 통해 엔터티에 액세스할 수 있습니다.[`Children`](../task/children/) ,[`Resources`](./resources/) ,[`ResourceAssignments`](./resourceassignments/) 등

### 또한보십시오

* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
