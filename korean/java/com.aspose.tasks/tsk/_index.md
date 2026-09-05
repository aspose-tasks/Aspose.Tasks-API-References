---
title: "Tsk"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체의 속성을 나타냅니다."
type: docs
weight: 328
url: /ko/java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

[Task](../../com.aspose.tasks/task) 객체의 속성을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## 필드

| 필드 | 설명 |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | 활동 ID 필드를 나타냅니다 - Primavera에서 사용하는 작업의 고유 식별자입니다. |
| [ACTUAL_COST](#ACTUAL-COST) | 리소스가 작업에서 이미 수행한 작업에 대한 비용과 해당 작업과 연관된 기타 기록된 비용을 포함합니다. |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | 예정된 기간과 현재 남은 작업 또는 완료 비율을 기반으로 한 작업의 실제 작업 시간 범위입니다. |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | 작업이 완료된 날짜입니다. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 작업에 할당된 리소스가 이미 수행한 초과 근무량을 나타냅니다. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 실제 초과 근무가 보호되는 기간입니다. |
| [ACTUAL_START](#ACTUAL-START) | 작업이 실제로 시작된 날짜와 시간입니다. |
| [ACTUAL_WORK](#ACTUAL-WORK) | 작업에 할당된 리소스가 이미 수행한 작업량입니다. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 실제 작업이 보호되는 기간입니다. |
| [ACWP](#ACWP) | 작업에 이미 수행된 작업에 대한 비용으로, 프로젝트 상태 날짜 또는 오늘 날짜까지 적용됩니다. |
| [BCWP](#BCWP) | 작업의 완료 비율에 시간 단계 기준 비용을 곱한 누적 값입니다. |
| [BCWS](#BCWS) | 상태 날짜 또는 오늘 날짜까지의 누적 시간 단계 기준 비용입니다. |
| [BUDGET_COST](#BUDGET-COST) | 예산 비용 리소스에 대한 예산 비용. |
| [BUDGET_WORK](#BUDGET-WORK) | 예산 작업 및 물자 리소스에 대한 예산 작업입니다. |
| [CALENDAR](#CALENDAR) | 작업 캘린더입니다. |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | 배송의 완료 날짜입니다. |
| [COMMITMENT_START](#COMMITMENT-START) | 배송의 시작 날짜입니다. |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | 작업에 연관된 전달이 있는지 또는 연관된 전달에 대한 종속성이 있는지를 결정합니다. |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | 제약 유형과 연관된 특정 날짜입니다. |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | 작업 일정에 적용할 수 있는 제약 유형에 대한 선택지를 제공합니다. |
| [CONTACT](#CONTACT) | 작업을 담당하는 개인의 이름입니다. |
| [COST](#COST) | 작업에 할당된 리소스가 수행한 작업에 대해 이미 발생한 비용과 남은 작업에 대해 계획된 비용을 합산한 작업의 총 예정 또는 예상 비용입니다. |
| [COST_VARIANCE](#COST-VARIANCE) | 작업, 리소스 또는 할당에 대한 기준 비용과 총 비용의 차이입니다. |
| [CREATED](#CREATED) | 작업이 생성된 날짜입니다. |
| [CV](#CV) | 작업에 대한 기준 비용과 총 비용의 차이입니다. |
| [DEADLINE](#DEADLINE) | 작업이 완료되어야 하는 목표 날짜입니다. |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | 작업을 요약 작업으로 표시할지 여부를 결정합니다. |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | 작업을 타임라인 보기에서 표시할지 여부를 지정합니다. |
| [DURATION](#DURATION) | 시작 날짜, 종료 날짜, 캘린더 및 기타 일정 요소를 기반으로 Microsoft Project가 입력하거나 계산한 작업의 전체 활성 작업 시간 범위입니다. |
| [DURATION_TEXT](#DURATION-TEXT) | 작업의 기간 텍스트를 반환합니다. |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | 작업의 기준 기간과 총 기간(현재 추정치) 사이의 차이입니다. |
| [EARLY_FINISH](#EARLY-FINISH) | 선행 및 후속 작업의 조기 종료 날짜, 기타 제약 조건 및 레벨링 지연을 기반으로 작업이 가장 빨리 종료될 수 있는 날짜입니다. |
| [EARLY_START](#EARLY-START) | 선행 및 후속 작업의 조기 시작 날짜와 기타 제약 조건을 기반으로 작업이 가장 빨리 시작될 수 있는 날짜입니다. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | % 완료 또는 물리적 % 완료 필드를 사용하여 수행된 작업의 예산 비용(BCWP)을 계산할지 여부를 결정합니다. |
| [EXTERNAL_ID](#EXTERNAL-ID) | 작업이 외부 작업인 경우 해당 작업의 외부 ID를 포함합니다. |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | 외부 작업의 소스 위치와 작업 식별자입니다. |
| [EXTERNAL_UID](#EXTERNAL-UID) | 작업이 외부인 경우 외부 작업의 고유 식별자를 포함합니다. |
| [FINISH](#FINISH) | 작업의 예정 종료 날짜입니다. |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | 조기 종료와 최종 종료 날짜 사이의 지속 시간(초)입니다. |
| [FINISH_TEXT](#FINISH-TEXT) | 작업의 종료 텍스트를 반환합니다. |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | 작업 또는 할당의 기준 종료 날짜와 현재 종료 날짜 사이의 차이를 나타내는 시간입니다. |
| [FIXED_COST](#FIXED-COST) | 리소스가 아닌 작업 비용을 표시합니다. |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | 고정 비용을 작업 비용에 언제, 어떻게 청구하거나 발생시킬지를 결정합니다. |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | 후속 작업을 지연시키지 않고 작업을 지연시킬 수 있는 시간(초)입니다. |
| [GUID](#GUID) | 작업에 대해 생성된 고유 식별 코드입니다. |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | 작업에 할당된 리소스가 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업을 할당받았는지 여부를 나타냅니다. |
| [HIDE_BAR](#HIDE-BAR) | Microsoft Project에서 표시될 때 작업의 간트 막대가 숨겨지는지 여부를 결정합니다. |
| [HYPERLINK](#HYPERLINK) | 작업과 연결된 하이퍼링크의 제목 또는 설명 텍스트입니다. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 작업과 연결된 하이퍼링크의 주소입니다. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 작업과 연결된 하이퍼링크 내 문서의 특정 위치. |
| [ID](#ID) | 작업 목록 내에서 작업의 위치 식별자입니다. |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | 작업 일정이 해당 작업에 할당된 리소스의 캘린더를 고려하는지 여부를 결정합니다. |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | Microsoft Project에서 일정 충돌 경고 표시기를 숨길지 여부를 나타냅니다. |
| [IS_ACTIVE](#IS-ACTIVE) | 작업이 활성 상태인지 여부를 결정합니다. |
| [IS_CRITICAL](#IS-CRITICAL) | 작업이 중요 경로에 있는지 여부를 결정합니다. |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | 작업 일정이 노력 기반 일정인지 여부를 결정합니다. |
| [IS_ESTIMATED](#IS-ESTIMATED) | 작업이 추정된 것인지 여부를 결정합니다. |
| [IS_EXPANDED](#IS-EXPANDED) | GanttChart 보기에서 요약 작업이 확장되어 있는지 여부를 결정합니다. |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | 작업이 외부 작업인지 여부를 결정합니다. |
| [IS_MANUAL](#IS-MANUAL) | 작업이 수동으로 일정이 지정되었는지 여부를 결정합니다. |
| [IS_MARKED](#IS-MARKED) | 작업이 추가 작업이나 특정 식별을 위해 표시되었는지 여부를 보여줍니다. |
| [IS_MILESTONE](#IS-MILESTONE) | 작업이 마일스톤인지 여부를 결정합니다. |
| [IS_NULL](#IS-NULL) | 작업이 널 작업인지 여부를 결정합니다. |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | 작업에 할당된 리소스 중 어느 하나라도 정상 작업 용량 내에서 수행할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다. |
| [IS_PUBLISHED](#IS-PUBLISHED) | 현재 작업을 프로젝트의 나머지와 함께 Project Server에 게시해야 하는지 여부를 결정합니다. |
| [IS_RECURRING](#IS-RECURRING) | 작업이 반복 작업 시리즈의 일부인지 여부를 결정합니다. |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | 작업을 재개할 수 있는지 여부를 결정합니다. |
| [IS_ROLLUP](#IS-ROLLUP) | 하위 작업 간트 막대에 대한 정보가 요약 작업 막대로 집계되는지 여부를 결정합니다. |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | 작업이 삽입된 프로젝트인지 여부를 결정합니다. |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | 하위 프로젝트가 읽기 전용인지 여부를 결정합니다. |
| [IS_SUMMARY](#IS-SUMMARY) | 작업이 요약 작업인지 여부를 결정합니다. |
| [LATE_FINISH](#LATE-FINISH) | 프로젝트 완료를 지연시키지 않고 작업이 끝날 수 있는 가장 최신 날짜입니다. |
| [LATE_START](#LATE-START) | 프로젝트 완료를 지연시키지 않고 작업을 시작할 수 있는 가장 최신 날짜입니다. |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | 리소스 레벨링 기능이 이 작업의 남은 작업을 분할시킬 수 있는지 여부를 결정합니다. |
| [LEVELING_DELAY](#LEVELING-DELAY) | 리소스 레벨링으로 인해 작업이 초기 시작 날짜에서 지연되는 시간입니다. |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | 레벨링 기능이 과다 할당을 해결하기 위해 개별 할당을 지연시키고 분할할 수 있는지 여부를 결정합니다. |
| [MANUAL_DURATION](#MANUAL-DURATION) | 작업의 수동으로 예약된 기간을 정의합니다. |
| [MANUAL_FINISH](#MANUAL-FINISH) | 작업의 수동으로 예약된 완료일을 정의합니다. |
| [MANUAL_START](#MANUAL-START) | 작업의 수동으로 예약된 시작일을 정의합니다. |
| [NAME](#NAME) | 작업 이름입니다. |
| [NOTES_RTF](#NOTES-RTF) | RTF 형식의 텍스트 메모입니다. |
| [NOTES_TEXT](#NOTES-TEXT) | RTF 데이터에서 추출한 메모의 일반 텍스트입니다. |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | 작업의 개요 수준입니다. |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | 계층적 개요 구조에서 작업의 위치를 나타내는 번호입니다. |
| [OVERTIME_COST](#OVERTIME-COST) | 작업에 대한 총 초과 근무 비용, 모든 할당된 작업에 대한 리소스의 비용, 또는 리소스 할당에 대한 비용입니다. |
| [OVERTIME_WORK](#OVERTIME-WORK) | 작업에 할당된 모든 리소스가 수행하도록 예약된 초과 근무량입니다. |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | 작업의 현재 상태로, 작업 기간 중 완료된 비율로 표시됩니다. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 작업의 현재 상태로, 완료된 작업 비율로 표시됩니다. |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | 예산 작업 수행 비용(BCWP)을 계산하기 위한 대안으로 사용할 수 있는 완료 비율 값입니다. |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | 리소스 레벨링이 수행되기 전 작업의 완료 날짜입니다. |
| [PRELEVELED_START](#PRELEVELED-START) | 리소스 레벨링이 수행되기 전 작업의 시작 날짜입니다. |
| [PRIORITY](#PRIORITY) | 작업에 부여된 중요도 수준으로, 이는 리소스 레벨링 중 작업이나 할당이 얼마나 쉽게 지연되거나 분할될 수 있는지를 나타냅니다. |
| [REGULAR_WORK](#REGULAR-WORK) | 리소스가 수행하도록 예약된 비초과 근무 작업의 총량입니다. |
| [REMAINING_COST](#REMAINING-COST) | 남은 예정 작업을 완료하는 데 발생할 남은 예정 비용입니다. |
| [REMAINING_DURATION](#REMAINING-DURATION) | 작업의 미완료 부분을 완료하는 데 필요한 시간입니다. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 작업에 대한 남은 예약 초과 근무 비용입니다. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 남은 예정 초과 근무 시간의 양. |
| [REMAINING_WORK](#REMAINING-WORK) | 작업 또는 작업 집합을 완료하는 데 아직 필요한 시간입니다. |
| [RESUME](#RESUME) | 작업의 남은 부분이 진행을 시작한 후 재개될 예정인 날짜. |
| [START](#START) | 작업의 예정 시작 날짜. |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | 조기 시작 날짜와 늦은 시작 날짜 사이의 지속 시간(초). |
| [START_TEXT](#START-TEXT) | 작업의 시작 텍스트를 반환합니다. |
| [START_VARIANCE](#START-VARIANCE) | 작업 또는 할당의 기준 시작 날짜와 현재 예정 시작 날짜 사이의 차이를 나타내는 시간. |
| [STATUS_MANAGER](#STATUS-MANAGER) | 현재 작업에 대한 상태 업데이트를 리소스로부터 받을 기업 리소스의 이름. |
| [STOP](#STOP) | 작업의 실제 부분이 끝나는 날짜를 나타냅니다. |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | 하위 프로젝트의 원본 위치. |
| [SV](#SV) | 프로젝트 상태 날짜까지의 획득 가치 일정 편차. |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | 프로젝트 종료 날짜를 지연시키지 않고 작업 종료 날짜를 연기할 수 있는 시간. |
| [TYPE](#TYPE) | 작업 유형. |
| [UID](#UID) | 작업의 고유 ID. |
| [WARNING](#WARNING) | 작업에 일정 차이가 있음을 나타내는 플래그를 나타냅니다. |
| [WBS](#WBS) | 작업 분류 구조(WBS) 코드. |
| [WBS_LEVEL](#WBS-LEVEL) | 작업의 가장 오른쪽 WBS 레벨. |
| [WORK](#WORK) | 할당된 모든 리소스에 대해 작업에 예정된 총 시간. |
| [WORK_VARIANCE](#WORK-VARIANCE) | 작업의 기준 작업량과 현재 예정 작업량 사이의 차이. |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Byte> ACTIVITY_ID
```


활동 ID 필드를 나타냅니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. (Primavera 프로젝트에만 적용됩니다).

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


리소스가 작업에서 이미 수행한 작업에 대한 비용과 해당 작업과 연관된 기타 기록된 비용을 포함합니다.

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Byte> ACTUAL_DURATION
```


예정된 기간과 현재 남은 작업 또는 완료 비율을 기반으로 한 작업의 실제 작업 시간 범위입니다.

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


작업이 완료된 날짜입니다.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


작업에 할당된 리소스가 이미 수행한 초과 근무량을 나타냅니다.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


실제 초과 근무가 보호되는 기간입니다.

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


작업이 실제로 시작된 날짜와 시간입니다.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


작업에 할당된 리소스가 이미 수행한 작업량입니다.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


실제 작업이 보호되는 기간입니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


작업에 이미 수행된 작업에 대한 비용으로, 프로젝트 상태 날짜 또는 오늘 날짜까지 적용됩니다.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


작업의 완료 비율에 시간 단계 기준 비용을 곱한 누적 값입니다.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


상태 날짜 또는 오늘 날짜까지의 누적 시간 단계 기준 비용입니다.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


예산 비용 리소스에 대한 예산 비용. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


예산 작업 및 자재 리소스에 대한 예산 작업입니다. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


작업 캘린더입니다.

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Byte> COMMITMENT_FINISH
```


배송의 완료 날짜입니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Byte> COMMITMENT_START
```


배송의 시작 날짜입니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Byte> COMMITMENT_TYPE
```


작업에 연관된 전달이 있는지 또는 연관된 전달에 대한 종속성이 있는지를 결정합니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Byte> CONSTRAINT_DATE
```


제약 유형과 연관된 특정 날짜입니다.

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Byte> CONSTRAINT_TYPE
```


작업 일정에 적용할 수 있는 제약 유형에 대한 선택지를 제공합니다.

### CONTACT {#CONTACT}
```
public static final Key<String,Byte> CONTACT
```


작업을 담당하는 개인의 이름입니다.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


작업에 할당된 리소스가 수행한 작업에 대해 이미 발생한 비용과 남은 작업에 대해 계획된 비용을 합산한 작업의 총 예정 또는 예상 비용입니다.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


작업, 리소스 또는 할당에 대한 기준 비용과 총 비용의 차이입니다.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


작업이 생성된 날짜입니다.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


작업의 기준 비용과 총 비용 사이의 차이. 비용 차이 = 비용 - 기준 비용

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Byte> DEADLINE
```


작업이 완료되어야 하는 목표 날짜입니다.

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Byte> DISPLAY_AS_SUMMARY
```


작업을 요약 작업으로 표시할지 여부를 결정합니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Byte> DISPLAY_ON_TIMELINE
```


작업을 타임라인 보기에서 표시할지 여부를 지정합니다.

### DURATION {#DURATION}
```
public static final Key<Duration,Byte> DURATION
```


시작 날짜, 종료 날짜, 캘린더 및 기타 일정 요소를 기반으로 Microsoft Project가 입력하거나 계산한 작업의 전체 활성 작업 시간 범위입니다.

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Byte> DURATION_TEXT
```


작업의 기간 텍스트를 반환합니다.

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Byte> DURATION_VARIANCE
```


작업의 기준 기간과 총 기간(현재 추정치) 사이의 차이입니다.

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Byte> EARLY_FINISH
```


선행 및 후속 작업의 조기 종료 날짜, 기타 제약 조건 및 레벨링 지연을 기반으로 작업이 가장 빨리 종료될 수 있는 날짜입니다.

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Byte> EARLY_START
```


선행 및 후속 작업의 조기 시작 날짜와 기타 제약 조건을 기반으로 작업이 가장 빨리 시작될 수 있는 날짜입니다.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


% 완료 또는 물리적 % 완료 필드를 사용하여 수행된 작업의 예산 비용(BCWP)을 계산할지 여부를 결정합니다.

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Byte> EXTERNAL_ID
```


작업이 외부 작업인 경우 해당 작업의 외부 ID를 포함합니다.

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Byte> EXTERNAL_TASK_PROJECT
```


외부 작업의 소스 위치와 작업 식별자입니다.

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Byte> EXTERNAL_UID
```


작업이 외부인 경우 외부 작업의 고유 식별자를 포함합니다.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


작업의 예정 종료 날짜입니다.

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FINISH_SLACK_TIME_SPAN
```


조기 종료와 최종 종료 날짜 사이의 지속 시간(초)입니다.

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Byte> FINISH_TEXT
```


작업의 종료 텍스트를 반환합니다.

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


작업 또는 할당의 기준 종료 날짜와 현재 종료 날짜 사이의 차이를 나타내는 시간입니다.

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Byte> FIXED_COST
```


리소스가 아닌 작업 비용을 표시합니다.

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> FIXED_COST_ACCRUAL
```


고정 비용을 작업 비용에 언제, 어떻게 청구하거나 발생시킬지를 결정합니다.

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FREE_SLACK_TIME_SPAN
```


후속 작업을 지연시키지 않고 작업을 지연시킬 수 있는 시간(초)입니다.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


작업에 대해 생성된 고유 식별 코드입니다.

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Byte> HAS_OVERALLOCATED_RESOURCE
```


작업에 할당된 리소스가 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업을 할당받았는지 여부를 나타냅니다.

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Byte> HIDE_BAR
```


Microsoft Project에서 표시될 때 작업의 간트 막대가 숨겨지는지 여부를 결정합니다.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


작업과 연결된 하이퍼링크의 제목 또는 설명 텍스트입니다.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


작업과 연결된 하이퍼링크의 주소입니다.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


작업과 연결된 하이퍼링크 내 문서의 특정 위치.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


작업 목록 내에서 작업의 위치 식별자입니다.

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Byte> IGNORE_RESOURCE_CALENDAR
```


작업 일정이 해당 작업에 할당된 리소스의 캘린더를 고려하는지 여부를 결정합니다.

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Byte> IGNORE_WARNINGS
```


Microsoft Project에서 일정 충돌 경고 표시기를 숨길지 여부를 나타냅니다.

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Byte> IS_ACTIVE
```


작업이 활성 상태인지 여부를 결정합니다. 비활성 작업은 더 이상 다른 작업이나 전체 프로젝트 일정에 영향을 주지 않습니다.

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Byte> IS_CRITICAL
```


작업이 중요 경로에 있는지 여부를 결정합니다.

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> IS_EFFORT_DRIVEN
```


작업 일정이 노력 기반 일정인지 여부를 결정합니다.

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Byte> IS_ESTIMATED
```


작업이 추정된 것인지 여부를 결정합니다.

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Byte> IS_EXPANDED
```


GanttChart 보기에서 요약 작업이 확장되어 있는지 여부를 결정합니다.

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Byte> IS_EXTERNAL_TASK
```


작업이 외부 작업인지 여부를 결정합니다.

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Byte> IS_MANUAL
```


작업이 수동으로 일정이 지정되었는지 여부를 결정합니다.

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Byte> IS_MARKED
```


작업이 추가 작업이나 특정 식별을 위해 표시되었는지 여부를 보여줍니다.

--------------------

mpp 파일 형식에만 적용됩니다.

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Byte> IS_MILESTONE
```


작업이 마일스톤인지 여부를 결정합니다.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


작업이 널 작업인지 여부를 결정합니다.

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Byte> IS_OVERALLOCATED
```


작업에 할당된 리소스 중 어느 하나라도 정상 작업 용량 내에서 수행할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다.

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Byte> IS_PUBLISHED
```


현재 작업을 프로젝트의 나머지와 함께 Project Server에 게시해야 하는지 여부를 결정합니다.

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Byte> IS_RECURRING
```


작업이 반복 작업 시리즈의 일부인지 여부를 결정합니다.

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Byte> IS_RESUME_VALID
```


작업을 재개할 수 있는지 여부를 결정합니다.

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Byte> IS_ROLLUP
```


하위 작업 간트 막대에 대한 정보가 요약 작업 막대로 집계되는지 여부를 결정합니다.

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Byte> IS_SUBPROJECT
```


작업이 삽입된 프로젝트인지 여부를 결정합니다.

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Byte> IS_SUBPROJECT_READ_ONLY
```


하위 프로젝트가 읽기 전용인지 여부를 결정합니다.

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Byte> IS_SUMMARY
```


작업이 요약 작업인지 여부를 결정합니다.

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Byte> LATE_FINISH
```


프로젝트 완료를 지연시키지 않고 작업이 끝날 수 있는 가장 최신 날짜입니다.

### LATE_START {#LATE-START}
```
public static final Key<Date,Byte> LATE_START
```


프로젝트 완료를 지연시키지 않고 작업을 시작할 수 있는 가장 최신 날짜입니다.

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Byte> LEVELING_CAN_SPLIT
```


리소스 레벨링 기능이 이 작업의 남은 작업을 분할시킬 수 있는지 여부를 결정합니다.

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


리소스 레벨링으로 인해 작업이 초기 시작 날짜에서 지연되는 시간입니다.

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Byte> LEVEL_ASSIGNMENTS
```


레벨링 기능이 과다 할당을 해결하기 위해 개별 할당을 지연시키고 분할할 수 있는지 여부를 결정합니다.

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Byte> MANUAL_DURATION
```


작업의 수동으로 예약된 기간을 정의합니다.

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Byte> MANUAL_FINISH
```


작업의 수동으로 예약된 완료일을 정의합니다.

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Byte> MANUAL_START
```


작업의 수동으로 예약된 시작일을 정의합니다.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


작업 이름입니다.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


RTF 형식의 텍스트 메모입니다.

--------------------

MPP 형식에만 지원됩니다.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


RTF 데이터에서 추출한 메모의 일반 텍스트입니다.

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Byte> OUTLINE_LEVEL
```


작업의 개요 수준입니다.

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Byte> OUTLINE_NUMBER
```


계층적 개요 구조에서 작업의 위치를 나타내는 번호입니다.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


작업에 대한 총 초과 근무 비용, 모든 할당된 작업에 대한 리소스의 비용, 또는 리소스 할당에 대한 비용입니다.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


작업에 할당된 모든 리소스가 수행하도록 예약된 초과 근무량입니다.

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_COMPLETE
```


작업의 현재 상태로, 작업 기간 중 완료된 비율로 표시됩니다.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


작업의 현재 상태로, 완료된 작업 비율로 표시됩니다.

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PHYSICAL_PERCENT_COMPLETE
```


예산 작업 수행 비용(BCWP)을 계산하기 위한 대안으로 사용할 수 있는 완료 비율 값입니다.

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Byte> PRELEVELED_FINISH
```


리소스 레벨링이 수행되기 전 작업의 완료 날짜입니다.

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Byte> PRELEVELED_START
```


리소스 레벨링이 수행되기 전 작업의 시작 날짜입니다.

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Byte> PRIORITY
```


작업에 부여된 중요도 수준으로, 이는 리소스 레벨링 중 작업이나 할당이 얼마나 쉽게 지연되거나 분할될 수 있는지를 나타냅니다.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


리소스가 수행하도록 예약된 비초과 근무 작업의 총량입니다.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


남은 예정 작업을 완료하는 데 발생할 남은 예정 비용입니다.

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Byte> REMAINING_DURATION
```


작업의 미완료 부분을 완료하는 데 필요한 시간입니다.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


작업에 대한 남은 예약 초과 근무 비용입니다.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


남은 예정 초과 근무 시간의 양.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


작업 또는 작업 집합을 완료하는 데 아직 필요한 시간입니다.

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


작업의 남은 부분이 진행을 시작한 후 재개될 예정인 날짜.

### START {#START}
```
public static final Key<Date,Byte> START
```


작업의 예정 시작 날짜.

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> START_SLACK_TIME_SPAN
```


조기 시작 날짜와 늦은 시작 날짜 사이의 지속 시간(초).

### START_TEXT {#START-TEXT}
```
public static final Key<String,Byte> START_TEXT
```


작업의 시작 텍스트를 반환합니다.

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


작업 또는 할당의 기준 시작 날짜와 현재 예정 시작 날짜 사이의 차이를 나타내는 시간.

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Byte> STATUS_MANAGER
```


현재 작업에 대한 상태 업데이트를 리소스로부터 받을 기업 리소스의 이름.

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


작업의 실제 부분이 끝나는 날짜를 나타냅니다.

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Byte> SUBPROJECT_NAME
```


하위 프로젝트의 원본 위치.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


프로젝트 상태 날짜까지의 획득 가치 일정 차이. 일정 차이(SV)는 BCWP와 BCWS 사이의 차이입니다.

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> TOTAL_SLACK_TIME_SPAN
```


프로젝트 종료 날짜를 지연시키지 않고 작업 종료 날짜를 연기할 수 있는 시간.

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


작업 유형.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


작업의 고유 ID.

### WARNING {#WARNING}
```
public static final Key<Boolean,Byte> WARNING
```


작업에 일정 차이가 있음을 나타내는 플래그를 나타냅니다.

### WBS {#WBS}
```
public static final Key<String,Byte> WBS
```


작업 분류 구조(WBS) 코드.

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Byte> WBS_LEVEL
```


작업의 가장 오른쪽 WBS 레벨.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


할당된 모든 리소스에 대해 작업에 예정된 총 시간.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


작업의 기준 작업량과 현재 예정 작업량 사이의 차이.

