---
title: GanttBarShowFor
second_title: .NET API 참조용 Aspose.Tasks
description: Gantt 차트의 막대 스타일을 사용자 정의할 때 사용되는 작업 범주를 나타냅니다.
type: docs
weight: 2730
url: /ko/net/aspose.tasks.visualization/ganttbarshowfor/
---
## GanttBarShowFor enumeration

Gantt 차트의 막대 스타일을 사용자 정의할 때 사용되는 작업 범주를 나타냅니다.

```csharp
public enum GanttBarShowFor
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Normal | `0` | 일반 카테고리. |
| Milestone | `1` | 마일스톤 카테고리. |
| Summary | `2` | 요약 카테고리. |
| Critical | `3` | 중요 범주. |
| Noncritical | `4` | 중요하지 않은 범주. |
| Marked | `5` | 표시된 카테고리. |
| Finished | `6` | 완료된 카테고리. |
| InProgress | `7` | 진행 중인 범주. |
| NotFinished | `8` | 완료되지 않은 카테고리. |
| NotStarted | `9` | 시작되지 않은 범주. |
| StartedLate | `10` | 늦게 시작했습니다. |
| FinishedLate | `11` | 완료 늦은 카테고리. |
| StartedEarly | `12` | 초기 범주를 시작했습니다. |
| FinishedEarly | `13` | 초기 카테고리를 완료했습니다. |
| StartedOnTime | `14` | 시작 시간 범주. |
| FinishedOnTime | `15` | 완료 정시 범주. |
| Flag1 | `16` | 플래그1 범주. |
| Flag2 | `17` | 플래그2 범주. |
| Flag3 | `18` | 플래그3 범주. |
| Flag4 | `19` | 플래그4 범주. |
| Flag5 | `20` | 플래그5 범주. |
| Flag6 | `21` | 플래그6 카테고리. |
| Flag7 | `22` | 플래그7 범주. |
| Flag8 | `23` | 플래그8 카테고리. |
| Flag9 | `24` | 플래그9 카테고리. |
| Flag10 | `25` | 플래그10 범주. |
| RolledUp | `26` | 롤업 카테고리. |
| ProjectSummary | `27` | 프로젝트 요약 범주. |
| Split | `28` | 범주 분할. |
| ExternalTasks | `29` | 외부 작업 범주. |
| Flag11 | `30` | 플래그11 범주. |
| Flag12 | `31` | 플래그12 범주. |
| Flag13 | `32` | 플래그13 범주. |
| Flag14 | `33` | 플래그14 카테고리. |
| Flag15 | `34` | 플래그15 범주. |
| Flag16 | `35` | 플래그16 카테고리. |
| Flag17 | `36` | 플래그17 범주. |
| Flag18 | `37` | 플래그18 카테고리. |
| Flag19 | `38` | 플래그19 범주. |
| Flag20 | `39` | Flag20 범주. |
| GroupBySummary | `40` | 요약 범주별 그룹화. |
| Deliverable | `41` | 산출물 범주. |
| Dependency | `42` | 종속성 범주. |
| Active | `43` | 활성 카테고리. |
| ManuallyScheduled | `44` | 수동으로 예약된 범주. |
| Warning | `45` | 경고 범주. |
| PlaceholderStart | `46` | 자리 표시자(시작) 범주. |
| PlaceholderFinish | `47` | 자리 표시자(완료) 범주. |
| PlaceholderDuration | `48` | 자리 표시자(기간) 범주. |
| Placeholder | `49` | 자리 표시자 범주. |
| Late | `50` | 늦은 카테고리. |
| NotNormal | `64` | 정상이 아님 |
| NotMilestone | `65` | 마일스톤 범주가 아닙니다. |
| NotSummary | `66` | 요약 범주 아님. |
| NotCritical | `67` | 중요하지 않은 범주. |
| NotMarked | `69` | 표시되지 않음 = 69 category. |
| NotInProgress | `71` | 진행 중 아님 = 71 category. |
| NotStartedLate | `74` | 늦게 시작되지 않음 = 74 category. |
| NotFinishedLate | `75` | 완료되지 않음 늦은 카테고리. |
| NotStartedEarly | `76` | 시작되지 않음 조기 범주. |
| NotFinishedEarly | `77` | 미완성 초기 카테고리. |
| NotStartedOnTime | `78` | 시간 범주에서 시작되지 않음. |
| NotFinishedOnTime | `79` | 정시에 완료되지 않음 범주. |
| NotFlag1 | `80` | 플래그1 범주가 아닙니다. |
| NotFlag2 | `81` | Flag2 범주가 아닙니다. |
| NotFlag3 | `82` | Flag3 범주가 아닙니다. |
| NotFlag4 | `83` | 플래그4 범주 아님. |
| NotFlag5 | `84` | Flag5 범주가 아닙니다. |
| NotFlag6 | `85` | 플래그6 범주 아님. |
| NotFlag7 | `86` | 플래그7 범주 아님. |
| NotFlag8 | `87` | Flag8 범주가 아닙니다. |
| NotFlag9 | `88` | 플래그9 범주 아님. |
| NotFlag10 | `89` | Flag10 범주가 아닙니다. |
| NotRolledUp | `90` | 롤업되지 않은 범주. |
| NotProjectSummary | `91` | 프로젝트 요약 범주가 아닙니다. |
| NotSplit | `92` | 분할 범주가 아님. |
| NotExternalTasks | `93` | 외부 작업 범주가 아닙니다. |
| NotFlag11 | `94` | Flag11 범주가 아닙니다. |
| NotFlag12 | `95` | Flag12 범주가 아닙니다. |
| NotFlag13 | `96` | 플래그13 범주가 아닙니다. |
| NotFlag14 | `97` | 플래그14 범주가 아닙니다. |
| NotFlag15 | `98` | 플래그15 범주가 아닙니다. |
| NotFlag16 | `99` | Flag16 범주가 아닙니다. |
| NotFlag17 | `100` | Flag17 범주가 아닙니다. |
| NotFlag18 | `101` | Flag18 범주가 아닙니다. |
| NotFlag19 | `102` | Flag19 범주가 아닙니다. |
| NotFlag20 | `103` | Flag20 범주가 아닙니다. |
| NotGroupBySummary | `104` | 요약 범주로 그룹화하지 않음. |
| NotDeliverable | `105` | 배송 불가 범주. |
| NotDependency | `106` | 종속성 범주가 아닙니다. |
| NotActive | `107` | 활성 범주가 아닙니다. |
| NotManuallyScheduled | `108` | 수동으로 예약되지 않은 범주. |
| NotWarning | `109` | 경고 범주 아님. |
| NotPlaceholderStart | `110` | 자리 표시자(시작) 범주가 아닙니다. |
| NotPlaceholderFinish | `111` | 자리 표시자(완료) 범주가 아닙니다. |
| NotPlaceholderDuration | `112` | 자리 표시자(기간) 범주가 아닙니다. |
| NotPlaceholder | `113` | 자리 표시자 범주가 아닙니다. |
| NotLate | `114` | 늦지 않음 카테고리. |

### 비고

Gantt 차트의 '막대 스타일' 대화 상자, '표시 대상' 열을 참조하세요.

### 또한보십시오

* 네임스페이스 [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
