---
title: "Rsc"
second_title: "Aspose.Tasks for Java API Reference"
description: "Resource 객체의 지원되는 속성을 나타냅니다."
type: docs
weight: 271
url: /ko/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

`Resource` 객체의 지원되는 속성을 나타냅니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | 리소스 표준 비용 및 초과 근무 비용이 작업 비용에 청구되거나 발생되는 시기와 방법을 결정합니다. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | 리소스에 대한 Active Directory Guid. |
| [ACTUAL_COST](#ACTUAL-COST) | 리소스가 작업에서 이미 수행한 작업에 대한 비용과 작업과 관련된 기타 기록된 비용을 포함합니다. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 작업에 할당된 리소스가 이미 수행한 실제 초과 근무량. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 실제 초과 근무가 보호되는 작업량. |
| [ACTUAL_WORK](#ACTUAL-WORK) | 작업에 할당된 리소스가 이미 수행한 작업량. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 실제 작업이 보호되는 작업량. |
| [ACWP](#ACWP) | 프로젝트에 대해 리소스가 수행한 작업의 현재까지 실제 비용. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | 할당 소유자의 이름. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | 할당 소유자의 GUID. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | 리소스가 현재 기간에 지정된 단위로 작업 가능해지는 시작 날짜. |
| [AVAILABLE_TO](#AVAILABLE-TO) | 리소스가 현재 기간에 지정된 단위에서 작업할 수 있는 종료 날짜. |
| [BCWP](#BCWP) | 리소스가 프로젝트를 위해 수행한 작업의 현재까지 예산 비용. |
| [BCWS](#BCWS) | 리소스에 예정된 작업의 예산 비용. |
| [BOOKING_TYPE](#BOOKING-TYPE) | 리소스의 예약 유형. |
| [BUDGET_COST](#BUDGET-COST) | 예산 비용 리소스에 대한 예산 비용. |
| [BUDGET_WORK](#BUDGET-WORK) | 예산 작업 및 자재 리소스에 대한 예산 작업. |
| [CALENDAR](#CALENDAR) | 리소스의 캘린더. |
| [CAN_LEVEL](#CAN-LEVEL) | 리소스에 대해 리소스 레벨링을 수행할 수 있는지 여부를 결정합니다. |
| [CODE](#CODE) | 리소스에 대한 코드 또는 기타 정보. |
| [COST](#COST) | 작업에 할당된 리소스가 수행한 작업에 이미 발생한 비용과 남은 작업에 대한 계획 비용을 합산하여 리소스에 대한 총 예정 비용 또는 예상 비용. |
| [COST_CENTER](#COST-CENTER) | 리소스가 발생시킨 비용이 청구될 비용 센터를 나타냅니다. |
| [COST_PER_USE](#COST-PER-USE) | 리소스가 사용될 때마다 발생하는 비용. |
| [COST_VARIANCE](#COST-VARIANCE) | 리소스의 기준 비용과 총 비용 간의 차이. |
| [CREATED](#CREATED) | 리소스가 프로젝트에 추가된 날짜와 시간. |
| [CV](#CV) | 프로젝트 상태 날짜까지의 획득 가치 비용 편차. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | 리소스의 이메일 주소. |
| [FINISH](#FINISH) | 리소스가 할당된 모든 작업을 완료하도록 예정된 날짜. |
| [GROUP](#GROUP) | 리소스가 속한 그룹. |
| [GUID](#GUID) | 리소스에 대해 생성된 고유 식별 코드를 포함합니다. |
| [HYPERLINK](#HYPERLINK) | 리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 리소스와 연결된 하이퍼링크의 주소. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 작업과 연결된 하이퍼링크 내 문서의 특정 위치. |
| [ID](#ID) | 리소스 목록 내에서 리소스의 위치 식별자. |
| [INACTIVE](#INACTIVE) | 관리자 권한을 가진 사용자가 리소스를 비활성화했는지 여부를 결정합니다. |
| [INITIALS](#INITIALS) | 리소스의 이니셜. |
| [IS_BUDGET](#IS-BUDGET) | 작업, 자재 또는 비용 리소스가 예산 리소스인지 여부를 결정합니다. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | 리소스가 비용 리소스인지 여부를 결정합니다. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | 리소스가 엔터프라이즈 리소스 풀에 속하는지(true) 또는 로컬 리소스 풀에 속하는지(false)를 표시합니다. |
| [IS_GENERIC](#IS-GENERIC) | 리소스가 일반 리소스인지 여부를 결정합니다. |
| [IS_NULL](#IS-NULL) | 리소스가 null인지 여부를 결정합니다. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | 현재 리소스가 팀 리소스인지 여부를 표시합니다. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | 자재 리소스의 측정 단위입니다. |
| [MAX_UNITS](#MAX-UNITS) | 리소스가 현재 기간 동안 모든 작업을 수행할 수 있는 최대 용량을 나타내는 최대 단위 수입니다. |
| [NAME](#NAME) | 리소스의 이름입니다. |
| [NOTES_RTF](#NOTES-RTF) | RTF 형식의 텍스트 메모입니다. |
| [NOTES_TEXT](#NOTES-TEXT) | RTF 데이터에서 추출한 메모의 일반 텍스트입니다. |
| [OVERALLOCATED](#OVERALLOCATED) | 리소스가 특정 작업 또는 모든 작업에 대해 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다. |
| [OVERTIME_COST](#OVERTIME-COST) | 리소스가 할당된 모든 작업에 대한 총 초과 근무 비용입니다. |
| [OVERTIME_RATE](#OVERTIME-RATE) | 리소스가 수행한 초과 근무에 대한 급여율입니다. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Microsoft Project에서 초과 근무율을 표시하는 데 사용되는 단위입니다. |
| [OVERTIME_WORK](#OVERTIME-WORK) | 리소스가 작업에서 수행하도록 예정된 초과 근무량이며, 관련 리소스의 초과 근무율로 청구됩니다. |
| [PEAK_UNITS](#PEAK-UNITS) | 리소스가 할당된 모든 작업에 대해 언제든지 적용되는 최대 할당 단위입니다. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 모든 작업에 대해 완료된 작업 비율입니다. |
| [PHONETICS](#PHONETICS) | 리소스 이름의 발음 표기입니다. |
| [REGULAR_WORK](#REGULAR-WORK) | 리소스가 수행하도록 예정된 비초과 근무의 총량입니다. |
| [REMAINING_COST](#REMAINING-COST) | 남은 예정 작업을 완료하는 데 발생할 남은 예정 비용입니다. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 리소스에 대한 남은 예정 초과 근무 비용입니다. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 남은 예정 초과 근무량입니다. |
| [REMAINING_WORK](#REMAINING-WORK) | 작업 또는 작업 집합을 완료하는 데 아직 필요한 시간입니다. |
| [STANDARD_RATE](#STANDARD-RATE) | 리소스가 수행한 정규 비초과 근무에 대한 급여율입니다. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위. |
| [START](#START) | 할당된 리소스가 작업을 시작하도록 일정이 잡힌 날짜. |
| [SV](#SV) | 프로젝트 상태 날짜까지의 획득 가치 일정 편차. |
| [TYPE](#TYPE) | 리소스 유형. |
| [UID](#UID) | 리소스의 고유 식별자. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | 리소스와 연결된 NT 계정. |
| [WORK](#WORK) | 작업에서 리소스에 일정이 잡힌 총 시간. |
| [WORKGROUP](#WORKGROUP) | 리소스가 속한 작업 그룹 유형. |
| [WORK_VARIANCE](#WORK-VARIANCE) | 리소스의 기준 작업과 현재 일정된 작업 사이의 차이. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


리소스 표준 비용 및 초과 근무 비용이 작업 비용에 청구되거나 발생되는 시기와 방법을 결정합니다.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


리소스에 대한 Active Directory Guid.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


리소스가 작업에서 이미 수행한 작업에 대한 비용과 작업과 관련된 기타 기록된 비용을 포함합니다.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


작업에 할당된 리소스가 이미 수행한 실제 초과 근무량.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


실제 초과 근무가 보호되는 작업량.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


작업에 할당된 리소스가 이미 수행한 작업량.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


실제 작업이 보호되는 작업량.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


프로젝트에 대해 리소스가 수행한 작업의 현재까지 실제 비용.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


할당 소유자의 이름.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


할당 소유자의 GUID.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


리소스가 현재 기간에 지정된 단위로 작업 가능해지는 시작 날짜.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


리소스가 현재 기간에 지정된 단위에서 작업할 수 있는 종료 날짜.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


리소스가 프로젝트를 위해 수행한 작업의 현재까지 예산 비용.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


리소스에 예정된 작업의 예산 비용.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


리소스의 예약 유형.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


예산 비용 리소스에 대한 예산 비용. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


예산 작업 및 자재 리소스에 대한 예산 작업. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


리소스의 캘린더.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


리소스에 대해 리소스 레벨링을 수행할 수 있는지 여부를 결정합니다.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


리소스에 대한 코드 또는 기타 정보.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


작업에 할당된 리소스가 수행한 작업에 이미 발생한 비용과 남은 작업에 대한 계획 비용을 합산하여 리소스에 대한 총 예정 비용 또는 예상 비용.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


리소스가 발생시킨 비용이 청구될 비용 센터를 나타냅니다.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


리소스가 사용될 때마다 발생하는 비용.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


리소스의 기준 비용과 총 비용 간의 차이.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


리소스가 프로젝트에 추가된 날짜와 시간.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


프로젝트 상태 날짜까지의 획득 가치 비용 편차. CV는 작업의 BCWP(수행된 작업의 예산 비용)와 ACWP(실제 수행된 작업의 비용) 사이의 차이입니다.

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


리소스의 이메일 주소.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


리소스가 할당된 모든 작업을 완료하도록 예정된 날짜.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


리소스가 속한 그룹.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


리소스에 대해 생성된 고유 식별 코드를 포함합니다.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


리소스와 연결된 하이퍼링크의 주소.

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


리소스 목록 내에서 리소스의 위치 식별자.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


관리자 권한을 가진 사용자가 리소스를 비활성화했는지 여부를 결정합니다.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


리소스의 이니셜.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


작업, 자재 또는 비용 리소스가 예산 리소스인지 여부를 결정합니다.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


리소스가 비용 리소스인지 여부를 결정합니다.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


리소스가 엔터프라이즈 리소스 풀에 속하는지(true) 또는 로컬 리소스 풀에 속하는지(false)를 표시합니다.

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


리소스가 일반 리소스인지 여부를 결정합니다.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


리소스가 null인지 여부를 결정합니다.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


현재 리소스가 팀 리소스인지 여부를 표시합니다.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


자재 리소스의 측정 단위입니다.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


리소스가 현재 기간 동안 모든 작업을 수행할 수 있는 최대 용량을 나타내는 최대 단위 수입니다.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


리소스의 이름입니다.

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

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


리소스가 특정 작업 또는 모든 작업에 대해 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


리소스가 할당된 모든 작업에 대한 총 초과 근무 비용입니다.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


리소스가 수행한 초과 근무에 대한 급여율입니다.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Microsoft Project에서 초과 근무율을 표시하는 데 사용되는 단위입니다.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


리소스가 작업에서 수행하도록 예정된 초과 근무량이며, 관련 리소스의 초과 근무율로 청구됩니다.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


리소스가 할당된 모든 작업에 대해 언제든지 적용되는 최대 할당 단위입니다.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


모든 작업에 대해 완료된 작업 비율입니다.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


리소스 이름의 발음 표기. 일본어 전용 사용.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


리소스가 수행하도록 예정된 비초과 근무의 총량입니다.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


남은 예정 작업을 완료하는 데 발생할 남은 예정 비용입니다.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


리소스에 대한 남은 예정 초과 근무 비용입니다.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


남은 예정 초과 근무량입니다.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


작업 또는 작업 집합을 완료하는 데 아직 필요한 시간입니다.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


리소스가 수행한 정규 비초과 근무에 대한 급여율입니다.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위.

### START {#START}
```
public static final Key<Date,Byte> START
```


할당된 리소스가 작업을 시작하도록 일정이 잡힌 날짜.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


프로젝트 상태 날짜까지의 획득 가치 일정 편차. SV는 수행된 작업의 예산 비용(BCWP)와 예정된 작업의 예산 비용(BCWS) 사이의 차이입니다.

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


리소스 유형.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


리소스의 고유 식별자.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


리소스와 연결된 NT 계정.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


작업에서 리소스에 일정이 잡힌 총 시간.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


리소스가 속한 작업 그룹 유형.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


리소스의 기준 작업과 현재 일정된 작업 사이의 차이.

