---
title: "클래스 Project"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Project 클래스. 프로젝트를 나타냅니다."
type: docs
weight: 1440
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
| [Project](project/#constructor)() | `Project` 클래스의 새 인스턴스를 초기화합니다. |
| [Project](project/#constructor_1)(DbSettings) | `Project` 클래스의 새 인스턴스를 초기화하여 [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/) 클래스 인스턴스로 지정된 데이터베이스에서 데이터를 읽습니다. |
| [Project](project/#constructor_2)(Stream) | `Project` 클래스의 새 인스턴스를 스트림에서 초기화합니다. |
| [Project](project/#constructor_7)(StreamReader) | `Project` 클래스의 새 인스턴스를 StreamReader 인스턴스에서 초기화합니다. |
| [Project](project/#constructor_8)(string) | `Project` 클래스의 새 인스턴스를 템플릿(존재하는 mpp 또는 mpt 파일)에서 초기화합니다. |
| [Project](project/#constructor_3)(Stream, LoadOptions) | `Project` 클래스의 새 인스턴스를 지정된 [`LoadOptions`](../loadoptions/) 클래스 인스턴스로 스트림에서 초기화합니다. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | `Project` 클래스의 새 인스턴스를 템플릿(존재하는 mpp 또는 mpt 파일)에서 초기화합니다. |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | `Project` 클래스의 새 인스턴스를 지정된 [`PrimaveraReadOptions`](../primaverareadoptions/) 클래스 인스턴스로 스트림에서 초기화합니다. |
| [Project](project/#constructor_6)(Stream, string) | `Project` 클래스의 새 인스턴스를 템플릿(존재하는 mpp 또는 mpt 파일)에서 초기화합니다. |
| [Project](project/#constructor_9)(string, LoadOptions) | `Project` 클래스의 새 인스턴스를 지정된 [`LoadOptions`](../loadoptions/) 클래스 인스턴스로 템플릿(존재하는 mpp 또는 mpt 파일)에서 초기화합니다. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | `Project` 클래스의 새 인스턴스를 템플릿(존재하는 mpp 또는 mpt 파일)에서 초기화합니다. |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | `Project` 클래스의 새 인스턴스를 지정된 [`PrimaveraReadOptions`](../primaverareadoptions/) 클래스 인스턴스로 템플릿(존재하는 MPP 또는 MPT 파일)에서 초기화합니다. |
| [Project](project/#constructor_12)(string, string) | 비밀번호로 보호된 템플릿(존재하는 mpp 또는 mpt 파일)에서 `Project` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | ActualsInSync가 설정되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | AdminProject가 설정되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | AreEditableActualCosts가 설정되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Author 값을 가져오거나 설정합니다. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | AutoAddNewResourcesAndTasks가 설정되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | 할당 작업 및 리소스 요율을 사용하여 할당 비용과 남은 비용을 자동으로 계산할지 여부를 가져오거나 설정합니다. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Autolink가 설정되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | BaselineForEarnedValue 값을 가져오거나 설정합니다. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | 프로젝트의 내장 속성 컬렉션을 가져옵니다. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | 프로젝트의 계산 모드를 가져오거나 설정합니다. [`CalculationMode`](./calculationmode/) 열거형의 값 중 하나일 수 있습니다. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Calendar의 값을 가져오거나 설정합니다. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | 이 Project 인스턴스의 [`CalendarCollection`](../calendarcollection/) 객체를 가져옵니다. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Category 값을 가져오거나 설정합니다. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Comments 값을 가져오거나 설정합니다. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Company 값을 가져오거나 설정합니다. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | CreationDate 값을 가져오거나 설정합니다. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | 이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다. 이는 프로젝트의 작업 수 n에 따라 O(n) 연산입니다. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | 총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 Critical로 간주합니다. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | CurrencyCode 값을 가져오거나 설정합니다. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | CurrencyDigits 값을 가져오거나 설정합니다. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | CurrencySymbol 값을 가져오거나 설정합니다. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | CurrencySymbolPosition 값을 가져오거나 설정합니다. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | CurrentDate 값을 가져오거나 설정합니다. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | CustomDateFormat 값을 가져오거나 설정합니다. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | 프로젝트의 사용자 정의 속성 컬렉션을 가져옵니다. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | DateFormat의 값을 가져오거나 설정합니다. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | DaysPerMonth의 값을 가져오거나 설정합니다. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | DefaultFinishTime의 값을 가져오거나 설정합니다. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | DefaultFixedCostAccrual의 값을 가져오거나 설정합니다. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | DefaultOvertimeRate의 값을 가져오거나 설정합니다. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | DefaultStandardRate의 값을 가져오거나 설정합니다. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | DefaultStartTime의 값을 가져오거나 설정합니다. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | DefaultTaskEVMethod의 값을 가져오거나 설정합니다. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | DefaultTaskType의 값을 가져오거나 설정합니다. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | 프로젝트의 기본 보기를 가져오거나 설정합니다. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | 프로젝트 기본 주 작업일 및 작업 시간을 나타내는 컬렉션을 나타내는 [`WeekDayCollection`](../weekdaycollection/) 클래스의 인스턴스를 가져옵니다. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | `[`ProjectDisplayOptions`](../projectdisplayoptions/)` 클래스의 인스턴스를 가져옵니다. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | DurationFormat의 값을 가져오거나 설정합니다. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | EearnedValueMethod의 값을 가져오거나 설정합니다. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 확장 속성(사용자 정의 필드) 정의 컬렉션입니다. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | ExtendedCreationDate의 값을 가져오거나 설정합니다. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | FinishDate의 값을 가져오거나 설정합니다. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | FiscalYearStart가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | FyStartDate의 값을 가져오거나 설정합니다. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | 프로젝트의 글로벌화(언어별) 설정을 가져오거나 설정합니다. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Guid의 값을 가져오거나 설정합니다. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | HonorConstraints가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | HyperlinkBase의 값을 가져오거나 설정합니다. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Keywords의 값을 가져오거나 설정합니다. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | LastAuthor의 값을 가져오거나 설정합니다. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | LastPrinted의 값을 가져오거나 설정합니다. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | LastSaved의 값을 가져오거나 설정합니다. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Manager의 값을 가져오거나 설정합니다. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | MicrosoftProjectServerURL이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | MinutesPerDay의 값을 가져오거나 설정합니다. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | MinutesPerWeek의 값을 가져오거나 설정합니다. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | MoveCompletedEndsBack이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | MoveCompletedEndsForward가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | MoveRemainingStartsBack이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | MoveRemainingStartsForward가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | MultipleCriticalPaths가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Name 값을 가져오거나 설정합니다. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | NewTasksAreManual이 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | NewTasksEffortDriven가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | NewTasksEstimated가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | NewTaskStartDate의 값을 가져오거나 설정합니다. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | 이 프로젝트 파일에 연결되거나 포함된 [`OleObject`](../oleobject/) 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다. mpp 파일 형식에서만 사용할 수 있습니다. 이 컬렉션은 'Clear' 작업을 제외하고 읽기 전용입니다. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | OutlineCodeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 개요 코드 정의의 컬렉션입니다. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Primavera 파일에서 읽은 프로젝트에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | ProjectExternallyEdited가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | ResourceAssignmentCollection 객체를 가져옵니다. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | 리소스 기반 필터 정의를 모두 가져옵니다. ResourceFilters는 [`Filter`](../filter/) 객체의 컬렉션입니다. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | 리소스 기반 그룹 정의를 모두 가져옵니다. ResourceGroups는 [`Group`](../group/) 객체의 컬렉션입니다. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | ResourceCollection 객체를 가져옵니다. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Revision의 값을 가져오거나 설정합니다. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | 작업 트리의 루트를 가져옵니다. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | SaveVersion의 값을 가져오거나 설정합니다. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | ScheduleFromStart가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | ShowProjectSummaryTask가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | SpreadActualCost가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | SpreadPercentComplete가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | StartDate의 값을 가져오거나 설정합니다. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | StatusDate의 값을 가져오거나 설정합니다. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Subject의 값을 가져오거나 설정합니다. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | [`Table`](../table/) 객체 목록을 가져옵니다. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | 작업 기반 필터 정의를 모두 가져옵니다. TaskFilters는 [`Filter`](../filter/) 객체의 컬렉션입니다. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | 작업 기반 그룹 정의를 모두 가져옵니다. TaskGroups는 [`Group`](../group/) 객체의 컬렉션입니다. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | [`TaskLinkCollection`](../tasklinkcollection/) 객체를 가져옵니다. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Template의 값을 가져오거나 설정합니다. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | TimescaleFinish의 값을 가져오거나 설정합니다. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | TimescaleStart의 값을 가져오거나 설정합니다. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Title의 값을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Uid의 값을 가져오거나 설정합니다. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | [`VbaProject`](./vbaproject/) 클래스의 인스턴스를 가져옵니다. |
| [Views](../../aspose.tasks/project/views/) { get; } | [`View`](../view/) 객체 목록을 가져옵니다. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | 프로젝트에 대한 WBS 코드 정의를 가져오거나 설정합니다. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | WeekStartDay의 값을 가져오거나 설정합니다. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | WorkFormat의 값을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | 루트 작업을 포함하여 프로젝트의 모든 작업을 재귀적으로 열거합니다. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | 이 컨테이너에서 속성이 매핑된 값을 반환합니다. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | 기준선 저장 시간을 반환합니다. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | 프로젝트 설정 [`DurationFormat`](../prj/durationformat/)에 정의된 기본 기간 형식과 지정된 단위 수를 가진 [`Duration`](../duration/) 객체를 가져옵니다. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | 지정된 수의 [`TimeUnitType`](../timeunittype/) 단위를 가진 [`Duration`](../duration/) 객체를 가져옵니다. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | 지정된 TimeSpan 값과 지정된 [`TimeUnitType`](../timeunittype/) 값을 가진 [`Duration`](../duration/) 객체를 가져옵니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | 기본 [`Timescale`](../../aspose.tasks.visualization/timescale/)(일)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | 기본 [`Timescale`](../../aspose.tasks.visualization/timescale/)(일)과 지정된 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | 지정된 [`SaveOptions`](../../aspose.tasks.saving/saveoptions/)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | 지정된 [`Timescale`](../../aspose.tasks.visualization/timescale/)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | 지정된 [`Timescale`](../../aspose.tasks.visualization/timescale/)과 [`PageSize`](../../aspose.tasks.visualization/pagesize/)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | 지정된 [`Timescale`](../../aspose.tasks.visualization/timescale/)과 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)을 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | 지정된 [`Timescale`](../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 및 날짜 범위를 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | 지정된 작업의 선행 작업인 작업 링크 컬렉션을 반환합니다. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | 지정된 Double 값과 기본 작업 형식을 가진 [`Duration`](../duration/) 객체를 가져옵니다. |
| [Print](../../aspose.tasks/project/print/#print)() | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터와 기본 프린터 설정으로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터와 기본 프린터 설정 및 사용자 지정 저장 옵션으로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터와 기본 프린터 설정으로 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정 및 사용자 지정 저장 옵션에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | 표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정, 사용자 지정 저장 옵션 및 지정된 문서 이름에 따라 프로젝트를 인쇄합니다. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | 모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜를 재조정하고, 조기/후기 날짜를 설정하며, 여유 시간, 작업 및 비용 필드를 계산합니다. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | 옵션 검증을 포함하여 모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜를 재조정하고, 조기/후기 날짜를 설정하며, 여유 시간, 작업 및 비용 필드를 계산합니다. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | 리소스의 Id, 시작 및 종료를 다시 계산합니다. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | 프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | 모든 작업의 WBS 코드를 다시 번호 매깁니다. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | 통과된 작업의 WBS 코드를 다시 번호 매깁니다. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | 완료되지 않은 프로젝트 작업을 지정된 날짜 이후에 시작하도록 다시 일정 잡습니다. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | 지정된 작업 목록에 대한 완료되지 않은 작업을 지정된 날짜 이후에 시작하도록 다시 일정 잡습니다. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | 프로젝트 데이터를 mpp 형식 파일에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | 프로젝트 데이터를 스트림에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | 지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | 프로젝트 데이터를 파일에 저장합니다. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | 지정된 저장 옵션을 사용하여 문서를 파일에 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | 프로젝트를 템플릿으로 지정된 스트림에 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | 프로젝트를 템플릿으로 지정된 파일 경로에 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | 프로젝트를 템플릿으로 지정된 스트림에 저장합니다. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | 프로젝트를 템플릿으로 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | 프로젝트 개요 보고서를 스트림에 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | 프로젝트 개요 보고서를 PDF 파일에 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | 지정된 유형의 프로젝트 보고서를 지정된 스트림에 저장합니다. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | 지정된 유형의 프로젝트 보고서를 PDF 형식으로 지정된 파일 경로에 저장합니다. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | 루트 작업의 모든 하위 작업을 재귀적으로 수집합니다. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | 이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | 이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | 선택된 작업에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | 기준선 저장 시간을 설정합니다. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | 전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | 지정된 작업 목록에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | 스트림에서 프로젝트 파일 정보를 가져옵니다. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | 파일에서 프로젝트 파일 정보를 읽습니다. |

## 비고

**Project**는 Aspose.Tasks 라이브러리의 핵심 클래스입니다.

**Project**를 사용하여 지원되는 프로젝트 관리 형식 중 하나인 MPP, MPT, MPX, XML을 읽을 수 있습니다.

지원되는 형식 중 하나로 기존 문서를 로드하려면 파일 이름이나 스트림을 **Project** 생성자 중 하나에 전달하십시오. 빈 프로젝트를 만들려면 매개변수 없는 생성자를 호출하십시오.

Save 메서드 오버로드 중 하나를 사용하여 프로젝트를 [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) 형식 중 하나로 저장합니다: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

**Project**는 [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), [`ExtendedAttributes`](./extendedattributes/)와 같은 프로젝트 전체 정보를 저장합니다. 이러한 객체 대부분은 **Project** 클래스의 해당 속성을 통해 액세스할 수 있습니다.

**Project**는 [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/), [`Calendar`](../calendar/)와 같은 다른 프로젝트 엔터티를 조작하기 위한 진입점을 포함하는 루트 엔터티입니다.

**Project** 엔터티는 타입이 지정된 컬렉션을 통해 접근할 수 있으며, 예를 들어 [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/) 등이 있습니다.

## 예제

<see cref=\"Aspose.Tasks.Project\"/> 인스턴스를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// 새 작업을 추가하고 원하는 속성을 설정합니다.
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// 새 리소스를 추가합니다.
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// 새 리소스 할당을 추가합니다.
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// 프로젝트를 사용 가능한 형식 중 하나로 저장합니다.
// 여기서는 Microsoft Project XML 파일 형식으로 저장하고 있습니다.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


