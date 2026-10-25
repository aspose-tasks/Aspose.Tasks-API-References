---
title: "Aspose::Tasks::Project 클래스"
linktitle: "프로젝트"
articleTitle: "프로젝트"
second_title: "C++용 Aspose.Tasks"
description: "프로젝트를 나타냅니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/project/
---

## Project class

프로젝트를 나타냅니다.

Project는 Aspose.Tasks 라이브러리의 핵심 클래스입니다.

Project를 사용하여 지원되는 프로젝트 관리 형식 중 하나인 MPP, MPT, MPX, XML을 읽을 수 있습니다.

지원되는 형식 중 하나로 기존 문서를 로드하려면 파일 이름이나 스트림을 Project 생성자 중 하나에 전달하십시오. 빈 프로젝트를 만들려면 매개변수 없는 생성자를 호출하십시오.

Save 메서드 중 하나의 오버로드를 사용하여 프로젝트를 Aspose::Tasks::Saving::SaveFileFormat 형식 중 하나로 저장하십시오: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

Project는 Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps 및 Aspose::Tasks::Project::ExtendedAttributes와 같은 프로젝트 전체 정보를 저장합니다. 이러한 객체 대부분은 Project 클래스의 해당 속성을 통해 접근할 수 있습니다.

Project는 Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute 및 Aspose::Tasks::Calendar와 같은 다른 프로젝트 엔터티를 조작하기 위한 진입점을 포함하는 루트 엔터티입니다.

Project 엔터티는 타입이 지정된 컬렉션을 통해 접근할 수 있으며, 예를 들어 Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments 등이 있습니다.

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Project (13 overloads)](./project/) | Project 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | 루트 작업을 포함한 프로젝트의 모든 작업을 재귀적으로 열거합니다. |
| [Get](./get/) | 이 컨테이너에서 속성이 매핑되는 값을 반환합니다. |
| [get_ActualsInSync](./get_actualsinsync/) | ActualsInSync가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_AdminProject](./get_adminproject/) | AdminProject가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | AreEditableActualCosts가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_Author](./get_author/) | Author 값을 가져옵니다. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | 할당 작업 및 리소스 요금을 사용하여 할당 비용과 남은 비용을 자동으로 계산해야 하는지 여부를 가져옵니다. |
| [get_Autolink](./get_autolink/) | Autolink가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | BaselineForEarnedValue 값을 가져옵니다. |
| [get_BuiltInProps](./get_builtinprops/) | 프로젝트의 내장 속성 컬렉션을 가져옵니다. |
| [get_CalculationMode](./get_calculationmode/) | 프로젝트의 계산 모드를 가져옵니다. CalculationMode 열거형의 값 중 하나일 수 있습니다. |
| [get_Calendar](./get_calendar/) | Calendar의 값을 가져옵니다. |
| [get_Calendars](./get_calendars/) | 이 Project 인스턴스의 CalendarCollection 객체를 가져옵니다. |
| [get_Category](./get_category/) | Category 값을 가져옵니다. |
| [get_Comments](./get_comments/) | Comments 값을 가져옵니다. |
| [get_Company](./get_company/) | Company 값을 가져옵니다. |
| [get_CreationDate](./get_creationdate/) | CreationDate 값을 가져옵니다. |
| [get_CriticalPath](./get_criticalpath/) | 이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | CriticalSlackLimit의 값을 가져옵니다. |
| [get_CurrencyCode](./get_currencycode/) | CurrencyCode의 값을 가져옵니다. |
| [get_CurrencyDigits](./get_currencydigits/) | CurrencyDigits의 값을 가져옵니다. |
| [get_CurrencySymbol](./get_currencysymbol/) | CurrencySymbol의 값을 가져옵니다. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | CurrencySymbolPosition의 값을 가져옵니다. |
| [get_CurrentDate](./get_currentdate/) | CurrentDate의 값을 가져옵니다. |
| [get_CustomDateFormat](./get_customdateformat/) | CustomDateFormat의 값을 가져옵니다. |
| [get_CustomProps](./get_customprops/) | 프로젝트의 사용자 정의 속성 컬렉션을 가져옵니다. |
| [get_DateFormat](./get_dateformat/) | DateFormat의 값을 가져옵니다. |
| [get_DaysPerMonth](./get_dayspermonth/) | DaysPerMonth의 값을 가져옵니다. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | DefaultFinishTime의 값을 가져옵니다. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | DefaultFixedCostAccrual의 값을 가져옵니다. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | DefaultOvertimeRate의 값을 가져옵니다. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | DefaultStandardRate의 값을 가져옵니다. |
| [get_DefaultStartTime](./get_defaultstarttime/) | DefaultStartTime의 값을 가져옵니다. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | DefaultTaskEVMethod의 값을 가져옵니다. |
| [get_DefaultTaskType](./get_defaulttasktype/) | DefaultTaskType의 값을 가져옵니다. |
| [get_DefaultView](./get_defaultview/) | 프로젝트의 기본 보기를 가져옵니다. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | 프로젝트 기본 주 작업일 및 작업 시간을 나타내는 컬렉션을 나타내는 WeekDayCollection 클래스의 인스턴스를 가져옵니다. |
| [get_DisplayOptions](./get_displayoptions/) | ProjectDisplayOptions 클래스의 인스턴스를 가져옵니다. |
| [get_DurationFormat](./get_durationformat/) | DurationFormat의 값을 가져옵니다. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod의 값을 가져옵니다. |
| [get_ExtendedAttributes](./get_extendedattributes/) | ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 이 객체는 프로젝트와 연결된 확장 속성(사용자 정의 필드) 정의의 컬렉션입니다. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | ExtendedCreationDate의 값을 가져옵니다. |
| [get_FinishDate](./get_finishdate/) | FinishDate의 값을 가져옵니다. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | FiscalYearStart가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_FyStartDate](./get_fystartdate/) | FyStartDate 값을 가져옵니다. |
| [get_Guid](./get_guid/) | Guid의 값을 가져옵니다. |
| [get_HonorConstraints](./get_honorconstraints/) | HonorConstraints가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | HyperlinkBase 값을 가져옵니다. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | InsertedProjectsLikeSummary가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_Keywords](./get_keywords/) | Keywords 값을 가져옵니다. |
| [get_LastAuthor](./get_lastauthor/) | LastAuthor 값을 가져옵니다. |
| [get_LastPrinted](./get_lastprinted/) | LastPrinted 값을 가져옵니다. |
| [get_LastSaved](./get_lastsaved/) | LastSaved 값을 가져옵니다. |
| [get_Manager](./get_manager/) | Manager 값을 가져옵니다. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | MicrosoftProjectServerURL이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_MinutesPerDay](./get_minutesperday/) | MinutesPerDay 값을 가져옵니다. |
| [get_MinutesPerWeek](./get_minutesperweek/) | MinutesPerWeek 값을 가져옵니다. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | MoveCompletedEndsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | MoveCompletedEndsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | MoveRemainingStartsBack이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | MoveRemainingStartsForward가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | MultipleCriticalPaths가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_Name](./get_name/) | Name의 값을 가져옵니다. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | NewTasksAreManual이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | NewTasksEffortDriven가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | NewTasksEstimated가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | NewTaskStartDate 값을 가져옵니다. |
| [get_OleObjects](./get_oleobjects/) | 이 프로젝트 파일에 연결되거나 포함된 OleObject 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다. |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연관된 개요 코드 정의 컬렉션입니다. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera 파일에서 읽은 프로젝트에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | ProjectExternallyEdited가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_RemoveFileProperties](./get_removefileproperties/) | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_ResourceAssignments](./get_resourceassignments/) | ResourceAssignmentCollection 객체를 가져옵니다. |
| [get_ResourceFilters](./get_resourcefilters/) | 리소스 기반 필터 정의를 모두 가져옵니다. ResourceFilters는 Filter 객체의 컬렉션입니다. |
| [get_ResourceGroups](./get_resourcegroups/) | 리소스 기반 그룹 정의를 모두 가져옵니다. ResourceGroups는 Group 객체의 컬렉션입니다. |
| [get_Resources](./get_resources/) | ResourceCollection 객체를 가져옵니다. |
| [get_Revision](./get_revision/) | Revision 값을 가져옵니다. |
| [get_RootTask](./get_roottask/) | 작업 트리의 루트를 가져옵니다. |
| [get_SaveVersion](./get_saveversion/) | SaveVersion 값을 가져옵니다. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | ScheduleFromStart가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | ShowProjectSummaryTask가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_SpreadActualCost](./get_spreadactualcost/) | SpreadActualCost가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | SpreadPercentComplete가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_StartDate](./get_startdate/) | StartDate 값을 가져옵니다. |
| [get_StatusDate](./get_statusdate/) | StatusDate 값을 가져옵니다. |
| [get_Subject](./get_subject/) | Subject 값을 가져옵니다. |
| [get_Tables](./get_tables/) | Table 객체 목록을 가져옵니다. |
| [get_TaskFilters](./get_taskfilters/) | 작업 기반 필터 정의를 모두 가져옵니다. TaskFilters는 Filter 객체의 컬렉션입니다. |
| [get_TaskGroups](./get_taskgroups/) | 작업 기반 그룹 정의를 모두 가져옵니다. TaskGroups는 Group 객체의 컬렉션입니다. |
| [get_TaskLinks](./get_tasklinks/) | TaskLinkCollection 객체를 가져옵니다. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_Template](./get_template/) | Template 값을 가져옵니다. |
| [get_TimescaleFinish](./get_timescalefinish/) | TimescaleFinish 값을 가져옵니다. |
| [get_TimescaleStart](./get_timescalestart/) | TimescaleStart의 값을 가져옵니다. |
| [get_Title](./get_title/) | Title의 값을 가져옵니다. |
| [get_Uid](./get_uid/) | Uid 값을 가져옵니다. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_VbaProject](./get_vbaproject/) | VbaProject 클래스의 인스턴스를 가져옵니다. |
| [get_Views](./get_views/) | View 객체 목록을 가져옵니다. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | 프로젝트에 대한 WBS 코드 정의를 가져옵니다. |
| [get_WeekStartDay](./get_weekstartday/) | WeekStartDay의 값을 가져옵니다. |
| [get_WorkFormat](./get_workformat/) | WorkFormat의 값을 가져옵니다. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | 기준선 저장 시간을 반환합니다. |
| [GetDuration (3 overloads)](./getduration/) | 프로젝트 설정 Prj::DurationFormat에 정의된 기본 기간 형식과 지정된 단위 수를 가진 Duration 객체를 가져옵니다. |
| [GetPageCount (7 overloads)](./getpagecount/) | 기본 Timescale(일)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다. |
| [GetPredecessors](./getpredecessors/) | 지정된 작업의 선행 작업인 작업 링크 컬렉션을 반환합니다. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | 스트림에서 프로젝트 파일 정보를 가져옵니다. |
| [GetWork](./getwork/) | 지정된 double 값과 기본 작업 형식을 가진 Duration 객체를 가져옵니다. |
| [Recalculate (2 overloads)](./recalculate/) | 모든 프로젝트 작업의 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다. |
| [RecalculateResourceFields](./recalculateresourcefields/) | 리소스의 Id, 시작 및 완료를 다시 계산합니다. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | 리소스의 시작 및 완료를 다시 계산합니다. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | 프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | 모든 작업의 WBS 코드를 다시 번호 매깁니다. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | 완료되지 않은 프로젝트 작업을 지정된 날짜 이후에 시작하도록 재조정합니다. |
| [Save (5 overloads)](./save/) | 지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | 프로젝트를 템플릿으로 지정된 스트림에 저장합니다. |
| [SaveReport (4 overloads)](./savereport/) | 프로젝트 개요 보고서를 스트림에 저장합니다. |
| [SelectAllChildTasks](./selectallchildtasks/) | 루트 작업의 모든 하위 작업을 재귀적으로 수집합니다. |
| [Set (2 overloads)](./set/) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [set_ActualsInSync](./set_actualsinsync/) | ActualsInSync가 설정되어 있는지 여부를 나타내는 값을 설정합니다. |
| [set_AdminProject](./set_adminproject/) | AdminProject가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | AreEditableActualCosts가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Author](./set_author/) | Author의 값을 설정합니다. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | 할당 작업 및 리소스 요금을 사용하여 할당 비용과 남은 비용을 자동으로 계산할지 여부를 설정합니다. |
| [set_Autolink](./set_autolink/) | Autolink가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | BaselineForEarnedValue의 값을 설정합니다. |
| [set_CalculationMode](./set_calculationmode/) | 프로젝트의 계산 모드를 설정합니다. CalculationMode 열거형의 값 중 하나일 수 있습니다. |
| [set_Calendar](./set_calendar/) | Calendar의 값을 설정합니다. |
| [set_Category](./set_category/) | Category의 값을 설정합니다. |
| [set_Comments](./set_comments/) | Comments의 값을 설정합니다. |
| [set_Company](./set_company/) | Company의 값을 설정합니다. |
| [set_CreationDate](./set_creationdate/) | CreationDate의 값을 설정합니다. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | CriticalSlackLimit의 값을 설정합니다. |
| [set_CurrencyCode](./set_currencycode/) | CurrencyCode의 값을 설정합니다. |
| [set_CurrencyDigits](./set_currencydigits/) | CurrencyDigits의 값을 설정합니다. |
| [set_CurrencySymbol](./set_currencysymbol/) | CurrencySymbol의 값을 설정합니다. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | CurrencySymbolPosition의 값을 설정합니다. |
| [set_CurrentDate](./set_currentdate/) | CurrentDate의 값을 설정합니다. |
| [set_CustomDateFormat](./set_customdateformat/) | CustomDateFormat의 값을 설정합니다. |
| [set_DateFormat](./set_dateformat/) | DateFormat의 값을 설정합니다. |
| [set_DaysPerMonth](./set_dayspermonth/) | DaysPerMonth의 값을 설정합니다. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | DefaultFinishTime의 값을 설정합니다. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | DefaultFixedCostAccrual의 값을 설정합니다. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | DefaultOvertimeRate의 값을 설정합니다. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | DefaultStandardRate의 값을 설정합니다. |
| [set_DefaultStartTime](./set_defaultstarttime/) | DefaultStartTime의 값을 설정합니다. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | DefaultTaskEVMethod의 값을 설정합니다. |
| [set_DefaultTaskType](./set_defaulttasktype/) | DefaultTaskType의 값을 설정합니다. |
| [set_DefaultView](./set_defaultview/) | 프로젝트의 기본 보기를 설정합니다. |
| [set_DurationFormat](./set_durationformat/) | DurationFormat의 값을 설정합니다. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod의 값을 설정합니다. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | ExtendedCreationDate의 값을 설정합니다. |
| [set_FinishDate](./set_finishdate/) | FinishDate의 값을 설정합니다. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | FiscalYearStart가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_FyStartDate](./set_fystartdate/) | FyStartDate의 값을 설정합니다. |
| [set_Guid](./set_guid/) | Guid의 값을 설정합니다. |
| [set_HonorConstraints](./set_honorconstraints/) | HonorConstraints가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | HyperlinkBase의 값을 설정합니다. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | InsertedProjectsLikeSummary가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Keywords](./set_keywords/) | Keywords의 값을 설정합니다. |
| [set_LastAuthor](./set_lastauthor/) | LastAuthor의 값을 설정합니다. |
| [set_LastPrinted](./set_lastprinted/) | LastPrinted의 값을 설정합니다. |
| [set_LastSaved](./set_lastsaved/) | LastSaved의 값을 설정합니다. |
| [set_Manager](./set_manager/) | Manager의 값을 설정합니다. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | MicrosoftProjectServerURL이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_MinutesPerDay](./set_minutesperday/) | MinutesPerDay의 값을 설정합니다. |
| [set_MinutesPerWeek](./set_minutesperweek/) | MinutesPerWeek의 값을 설정합니다. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | MoveCompletedEndsBack이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | MoveCompletedEndsForward가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | MoveRemainingStartsBack이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | MoveRemainingStartsForward가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | MultipleCriticalPaths가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Name](./set_name/) | Name의 값을 설정합니다. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | NewTasksAreManual이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | NewTasksEffortDriven가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | NewTasksEstimated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | NewTaskStartDate 값을 설정합니다. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | ProjectExternallyEdited가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_RemoveFileProperties](./set_removefileproperties/) | RemoveFileProperties가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Revision](./set_revision/) | Revision 값을 설정합니다. |
| [set_SaveVersion](./set_saveversion/) | SaveVersion 값을 설정합니다. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | ScheduleFromStart가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | ShowProjectSummaryTask가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | SplitsInProgressTasks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_SpreadActualCost](./set_spreadactualcost/) | SpreadActualCost가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | SpreadPercentComplete가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_StartDate](./set_startdate/) | StartDate 값을 설정합니다. |
| [set_StatusDate](./set_statusdate/) | StatusDate 값을 설정합니다. |
| [set_Subject](./set_subject/) | Subject 값을 설정합니다. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | TaskUpdatesResource가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Template](./set_template/) | Template 값을 설정합니다. |
| [set_TimescaleFinish](./set_timescalefinish/) | TimescaleFinish 값을 설정합니다. |
| [set_TimescaleStart](./set_timescalestart/) | TimescaleStart 값을 설정합니다. |
| [set_Title](./set_title/) | Title 값을 설정합니다. |
| [set_Uid](./set_uid/) | Uid의 값을 설정합니다. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | 프로젝트에 대한 WBS 코드 정의를 설정합니다. |
| [set_WeekStartDay](./set_weekstartday/) | WeekStartDay의 값을 설정합니다. |
| [set_WorkFormat](./set_workformat/) | WorkFormat의 값을 설정합니다. |
| [SetBaseline (2 overloads)](./setbaseline/) | 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | 기준선 저장 시간을 설정합니다. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | 전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다. |

