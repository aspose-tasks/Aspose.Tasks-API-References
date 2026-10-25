---
title: "클래스 Tsk"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Tsk 클래스. Task 객체의 속성을 나타냅니다."
type: docs
weight: 2620
url: /ko/net/aspose.tasks/tsk/
---
## Tsk class

[`Task`](../task/) 객체의 속성을 나타냅니다.

```csharp
public static class Tsk
```

## 필드

| 이름 | 설명 |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | 활동 ID 필드를 나타냅니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. (Primavera 프로젝트에만 적용됩니다.) |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | 리소스가 자신의 작업에서 이미 수행한 작업에 대해 발생한 비용과 작업과 연관된 기타 기록된 비용을 포함합니다. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | 작업에 대한 실제 작업 시간의 범위로, 예정된 기간과 현재 남은 작업량 또는 완료 비율을 기반으로 합니다. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | 작업이 완료된 날짜. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | 할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용이 발생합니다. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | 작업에 할당된 리소스가 이미 수행한 초과 근무량. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | 실제 초과 근무가 보호되는 기간. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | 작업이 실제로 시작된 날짜와 시간. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | 작업에 할당된 리소스가 이미 수행한 작업량. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | 실제 작업이 보호되는 기간. 읽기는 XML 형식만 지원됩니다. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | 작업에 이미 수행된 작업에 대해 발생한 비용으로, 프로젝트 상태 날짜 또는 오늘 날짜까지 적용됩니다. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | 작업의 완료 비율에 시간 단계별 기준 비용을 곱한 누적 값. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | 상태 날짜 또는 오늘 날짜까지의 누적 시간 단계별 기준 비용. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | 예산 비용 리소스에 대한 예산 비용. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | 예산 작업 및 물자 리소스에 대한 예산 작업입니다. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | 작업 캘린더. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | 전달의 종료 날짜. 읽기는 XML 형식만 지원됩니다. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | 전달의 시작 날짜. 읽기는 XML 형식만 지원됩니다. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | 작업에 연관된 전달이 있는지 또는 연관된 전달에 대한 종속성이 있는지를 결정합니다. 읽기는 XML 형식만 지원됩니다. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | 제약 유형과 연관된 특정 날짜. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | 작업 일정에 적용할 수 있는 제약 유형에 대한 선택지를 제공합니다. |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | 작업에 책임이 있는 개인의 이름. |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | 작업에 할당된 리소스가 수행한 작업에 대해 이미 발생한 비용과 남은 작업에 대해 계획된 비용을 합산한, 작업에 대한 총 예정 또는 예상 비용. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | 작업, 리소스 또는 할당에 대한 기준 비용과 총 비용 간의 차이. |
| static readonly [Created](../../aspose.tasks/tsk/created/) | 작업이 생성된 날짜. |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | 작업에 대한 기준 비용과 총 비용 간의 차이. 비용 차이 = 비용 - 기준 비용 |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | 작업이 완료될 예정인 목표 날짜. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | 작업을 요약 작업으로 표시할지 여부를 결정합니다. 읽기는 XML 형식만 지원됩니다. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | 작업을 타임라인 보기에서 표시할지 여부를 지정합니다. |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | 시작 날짜, 종료 날짜, 캘린더 및 기타 일정 요소를 기반으로 Microsoft Project에서 입력되거나 계산된 작업의 전체 활성 작업 시간 범위. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | 작업의 기간 텍스트를 반환합니다. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | 작업의 기준 기간과 총 기간(현재 추정치) 간의 차이. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | 선행 및 후속 작업의 조기 종료 날짜, 기타 제약 조건 및 레벨링 지연을 기반으로 작업이 완료될 수 있는 가장 이른 날짜. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | 선행 및 후속 작업의 조기 시작 날짜와 기타 제약 조건을 기반으로 작업이 시작될 수 있는 가장 이른 날짜. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | % 완료 또는 물리적 % 완료 필드를 사용하여 수행된 작업의 예산 비용(BCWP)을 계산할지 여부를 결정합니다. |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | 작업이 외부 작업인 경우 해당 작업의 외부 ID를 포함합니다. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | 외부 작업의 소스 위치 및 작업 식별자. |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | 작업이 외부인 경우 외부 작업의 고유 식별자를 포함합니다. |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | 작업의 예정 종료 날짜. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | 조기 종료와 후기 종료 날짜 사이의 기간. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | 작업의 종료 텍스트를 반환합니다. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | 작업 또는 할당의 기준 종료 날짜와 현재 종료 날짜 간의 차이를 나타내는 시간. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | 리소스가 아닌 작업 비용을 표시합니다. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | 고정 비용을 작업 비용에 청구하거나 발생시킬 시기와 방법에 대한 선택을 결정합니다. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | 후속 작업을 지연시키지 않고 작업을 지연시킬 수 있는 시간. |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | 작업에 대해 생성된 고유 식별 코드. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | 작업에 할당된 리소스가 정상 작업 용량 내에서 완료될 수 있는 것보다 더 많은 작업을 할당받았는지 여부를 나타냅니다. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | Microsoft Project에 표시될 때 작업의 간트 바가 숨겨져 있는지 여부를 결정합니다. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | 작업에 연결된 하이퍼링크의 제목 또는 설명 텍스트입니다. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | 작업에 연결된 하이퍼링크의 주소입니다. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | 작업과 연결된 하이퍼링크의 문서 내 특정 위치입니다. |
| static readonly [Id](../../aspose.tasks/tsk/id/) | 작업 목록 내에서 작업의 위치 식별자입니다. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | 작업 일정이 해당 작업에 할당된 리소스의 캘린더를 고려하는지 여부를 결정합니다. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | Microsoft Project에서 일정 충돌 경고 표시기를 숨길지 여부를 나타냅니다. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | 작업이 활성 상태인지 여부를 결정합니다. 비활성 작업은 더 이상 다른 작업이나 전체 프로젝트 일정에 영향을 주지 않습니다. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | 작업이 중요 경로에 있는지 여부를 결정합니다. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | 작업 일정이 노력 기반 일정인지 여부를 결정합니다. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | 작업이 추정된 것인지 여부를 결정합니다. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | 간트 차트 보기에서 요약 작업이 확장되어 있는지 여부를 결정합니다. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | 작업이 외부 작업인지 여부를 결정합니다. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | 작업이 수동으로 일정이 지정되었는지 여부를 결정합니다. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | 작업이 추가 작업이나 특정 식별을 위해 표시되었는지 여부를 보여줍니다. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | 작업이 마일스톤인지 여부를 결정합니다. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | 작업이 널 작업인지 여부를 결정합니다. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | 작업에 할당된 리소스 중 어느 하나라도 정상 작업 용량 내에서 수행할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | 현재 작업을 프로젝트의 나머지와 함께 Project Server에 게시해야 하는지 여부를 결정합니다. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | 작업이 반복 작업 시리즈의 일부인지 여부를 결정합니다. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | 작업을 재개할 수 있는지 여부를 결정합니다. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | 하위 작업 간트 바에 대한 정보가 요약 작업 바로 집계되는지 여부를 결정합니다. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | 작업이 삽입된 프로젝트인지 여부를 결정합니다. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | 하위 프로젝트가 읽기 전용인지 여부를 결정합니다. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | 작업이 요약 작업인지 여부를 결정합니다. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | 작업이 프로젝트 완료를 지연시키지 않고 마칠 수 있는 가장 최신 날짜. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | 작업이 프로젝트 완료를 지연시키지 않고 시작할 수 있는 가장 최신 날짜. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | 레벨링 기능이 과다 할당을 해결하기 위해 개별 할당을 지연시키고 분할할 수 있는지 여부를 결정합니다. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | 리소스 레벨링 기능이 이 작업의 남은 작업을 분할시킬 수 있는지 여부를 결정합니다. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | 리소스 레벨링으로 인해 작업이 초기 시작 날짜로부터 지연되는 시간. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | 작업의 수동으로 일정이 지정된 기간을 정의합니다. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | 작업의 수동으로 일정이 지정된 완료일을 정의합니다. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | 작업의 수동으로 일정이 지정된 시작일을 정의합니다. |
| static readonly [Name](../../aspose.tasks/tsk/name/) | 작업 이름. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | RTF 형식의 텍스트 메모입니다. MPP 형식에서만 지원됩니다. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | RTF 데이터에서 추출한 메모의 일반 텍스트입니다. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | 작업의 개요 수준. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | 계층적 개요 구조에서 작업의 위치를 나타내는 번호. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | 작업에 대한 총 초과 근무 비용, 모든 할당된 작업에 대한 리소스의 비용, 또는 리소스 할당에 대한 비용. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | 작업에 할당된 모든 리소스가 수행하도록 예정된 초과 근무량. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | 작업의 현재 상태로, 작업 기간 중 완료된 비율로 표시됩니다. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | 작업의 현재 상태를 완료된 작업 비율로 표시합니다. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | 예산 작업 수행 비용(BCWP)을 계산하기 위한 대안으로 사용할 수 있는 완료 퍼센트 값. |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | 리소스 레벨링이 수행되기 전 작업의 완료 날짜. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | 리소스 레벨링이 수행되기 전 작업의 시작 날짜. |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | 작업에 부여된 중요도 수준으로, 이는 리소스 레벨링 중 작업이나 할당이 얼마나 쉽게 지연되거나 분할될 수 있는지를 나타냅니다. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | 리소스가 수행하도록 예정된 비초과 근무 총량. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | 남은 예정 작업을 완료하는 데 발생할 남은 예정 비용. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | 작업의 미완성 부분을 완료하는 데 필요한 시간. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | 작업에 대한 남은 예정 초과 근무 비용. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | 남은 예정 초과 근무 시간량. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | 작업 또는 작업 집합을 완료하는 데 아직 필요한 시간. |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | 작업의 남은 부분이 진행을 시작한 후 재개될 예정인 날짜. |
| static readonly [Start](../../aspose.tasks/tsk/start/) | 작업의 예정 시작 날짜. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | 조기 시작과 늦은 시작 날짜 사이의 기간. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | 작업의 시작 텍스트를 반환합니다. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | 작업 또는 할당의 기준 시작 날짜와 현재 예정된 시작 날짜 사이의 차이를 나타내는 시간. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | 현재 작업에 대한 상태 업데이트를 리소스로부터 받을 기업 리소스의 이름. |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | 작업 실제 부분의 종료를 나타내는 날짜. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | 하위 프로젝트의 소스 위치. |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | 프로젝트 상태 날짜까지의 획득 가치 일정 편차. 일정 편차(SV)는 BCWP와 BCWS 사이의 차이입니다. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | 프로젝트 종료 날짜를 지연시키지 않고 작업 종료 날짜를 연기할 수 있는 시간. |
| static readonly [Type](../../aspose.tasks/tsk/type/) | 작업의 유형. |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | 작업의 고유 Id. |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | 작업에 일정 불일치가 있음을 나타내는 플래그를 나타냅니다. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | 작업 분류 구조(WBS) 코드. |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | 작업의 가장 오른쪽 WBS 레벨. |
| static readonly [Work](../../aspose.tasks/tsk/work/) | 할당된 모든 리소스에 대해 작업에 예정된 총 시간. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | 작업의 기준 작업과 현재 예정된 작업 사이의 차이. |

## 예제

작업 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업을 추가하고 작업 속성을 설정합니다
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


