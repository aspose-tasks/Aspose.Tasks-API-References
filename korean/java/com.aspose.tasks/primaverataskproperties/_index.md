---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera 파일 XER 또는 P6XML에서 읽은 작업에 대한 Primavera 전용 속성을 나타냅니다."
type: docs
weight: 209
url: /ko/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Primavera 파일(XER 또는 P6XML)에서 읽은 작업에 대한 Primavera 전용 속성을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getActivityId()](#getActivityId--) | 활동 ID 필드를 가져옵니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. |
| [getActivityType()](#getActivityType--) | 'Activity Type' 필드의 값을 가져옵니다. |
| [getActualExpenseCost()](#getActualExpenseCost--) | 실제 비용의 값을 가져옵니다. |
| [getActualLaborCost()](#getActualLaborCost--) | 실제 인건비의 값을 가져옵니다. |
| [getActualLaborUnits()](#getActualLaborUnits--) | 실제 인력 단위의 값을 가져옵니다. |
| [getActualMaterialCost()](#getActualMaterialCost--) | 실제 자재 비용의 값을 가져옵니다. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | 실제 비인력 단위의 값을 가져옵니다. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | 실제 비인력 비용의 값을 가져옵니다. |
| [getActualTotalCost()](#getActualTotalCost--) | 실제 비용의 총 값을 가져옵니다. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | 예산(또는 계획)된 비용의 값을 가져옵니다. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | 예산(또는 계획)된 인건비의 값을 가져옵니다. |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | 예산(또는 계획)된 자재 비용의 값을 가져옵니다. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | 예산(또는 계획된) 비노동 비용의 값을 가져옵니다. |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | 예산(또는 계획된) 비용의 총 값을 가져옵니다. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | 기간 완료 퍼센트의 값을 가져옵니다. |
| [getDurationType()](#getDurationType--) | 활동의 'Duration Type' 필드 값을 가져옵니다. |
| [getPercentCompleteType()](#getPercentCompleteType--) | 활동의 '% Complete Type' 필드 값을 가져옵니다. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Physical Percent Complete의 값을 가져옵니다. |
| [getPlannedDuration()](#getPlannedDuration--) | 원래 또는 계획된 기간을 가져옵니다 -- 작업 계획 시작일부터 계획 완료일까지의 총 작업 시간입니다. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | 주 제약 조건의 날짜를 가져옵니다. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | 주 제약 조건의 유형을 가져옵니다. |
| [getRawActivityType()](#getRawActivityType--) | 활동의 'Activity Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | 활동의 '% Complete Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다. |
| [getRawDurationType()](#getRawDurationType--) | 활동의 'Duration Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다. |
| [getRawStatus()](#getRawStatus--) | 활동의 'Status' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | 남은 조기 종료 날짜를 가져옵니다 - 활동의 남은 작업이 완료될 예정인 날짜입니다. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | 남은 조기 시작 날짜를 가져옵니다 - 활동의 남은 작업이 시작될 예정인 날짜입니다. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | 남은 경비 비용의 값을 가져옵니다. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | 남은 노동 단위의 값을 가져옵니다. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | 남은 늦은 종료 날짜를 가져옵니다. |
| [getRemainingLateStart()](#getRemainingLateStart--) | 남은 늦은 시작 날짜를 가져옵니다. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | 남은 비노동 단위의 값을 가져옵니다. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | 보조 제약 조건의 날짜를 가져옵니다. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | 보조 제약 조건의 유형을 가져옵니다. |
| [getSequenceNumber()](#getSequenceNumber--) | WBS 항목(요약 작업)의 순번을 가져옵니다. |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | 단위 완료 퍼센트의 값을 가져옵니다. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


활동 ID 필드를 가져옵니다 - Primavera에서 사용되는 작업의 고유 식별자입니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
java.lang.String - 활동 ID 필드 - Primavera에서 사용되는 작업의 고유 식별자.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


'Activity Type' 필드의 값을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
int - 'Activity Type' 필드의 값.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


실제 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 실제 비용의 값.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


실제 인건비의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 실제 인건비의 값.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


실제 인력 단위의 값을 가져옵니다.

**Returns:**
double - 실제 인력 단위의 값.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


실제 자재 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 실제 자재 비용의 값.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


실제 비인력 단위의 값을 가져옵니다.

**Returns:**
double - 실제 비인력 단위의 값.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


실제 비인력 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 실제 비인력 비용의 값.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


실제 비용의 총 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 실제 비용의 총값.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


예산(또는 계획)된 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 예산(또는 계획된) 비용의 값.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


예산(또는 계획)된 인건비의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 예산(또는 계획된) 인건비의 값.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


예산(또는 계획)된 자재 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 예산(또는 계획된) 자재 비용의 값.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


예산(또는 계획된) 비노동 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 예산(또는 계획된) 비인력 비용의 값.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


예산(또는 계획된) 비용의 총 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 예산(또는 계획된) 비용의 총값.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


기간 완료 퍼센트의 값을 가져옵니다.

**Returns:**
double - 기간 완료 백분율의 값.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


활동의 'Duration Type' 필드 값을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
int - 활동의 'Duration Type' 필드 값.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


활동의 '% Complete Type' 필드 값을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
int - 활동의 '% Complete Type' 필드 값.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Physical Percent Complete의 값을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
double - 물리적 완료 백분율의 값.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


원래 또는 계획된 기간을 가져옵니다 -- 작업 계획 시작일부터 계획 완료일까지의 총 작업 시간입니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


주 제약 조건의 날짜를 가져옵니다.

**Returns:**
java.util.Date - 주요 제약 조건의 날짜.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


주 제약 조건의 유형을 가져옵니다.

**Returns:**
int - 주요 제약 조건의 유형.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


활동의 'Activity Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
java.lang.String - 활동의 'Activity Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일).
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


활동의 '% Complete Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
java.lang.String - 활동의 '% Complete Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일).
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


활동의 'Duration Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
java.lang.String - 활동의 'Duration Type' 필드에 대한 원시 텍스트 표현(소스 파일과 동일).
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


활동의 'Status' 필드에 대한 원시 텍스트 표현(소스 파일과 동일)을 가져옵니다.

--------------------

활동(요약이 아닌 작업)에만 적용됩니다.

**Returns:**
java.lang.String - 활동의 'Status' 필드에 대한 원시 텍스트 표현(소스 파일과 동일).
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


남은 조기 종료 날짜를 가져옵니다 - 활동의 남은 작업이 완료될 예정인 날짜입니다.

**Returns:**
java.util.Date - 남은 조기 종료 날짜 - 활동의 남은 작업이 완료될 예정인 날짜.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


남은 조기 시작 날짜를 가져옵니다 - 활동의 남은 작업이 시작될 예정인 날짜입니다.

**Returns:**
java.util.Date - 남은 초기 시작 날짜 - 활동에 대한 남은 작업이 시작될 예정인 날짜입니다.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


남은 경비 비용의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 남은 비용 비용의 값.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


남은 노동 단위의 값을 가져옵니다.

**Returns:**
double - 남은 노동 단위의 값.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


남은 늦은 종료 날짜를 가져옵니다.

**Returns:**
java.util.Date - 남은 늦은 종료 날짜.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


남은 늦은 시작 날짜를 가져옵니다.

**Returns:**
java.util.Date - 남은 늦은 시작 날짜.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


남은 비노동 단위의 값을 가져옵니다.

**Returns:**
double - 남은 비노동 단위의 값.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


보조 제약 조건의 날짜를 가져옵니다.

**Returns:**
java.util.Date - 보조 제약 조건의 날짜.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


보조 제약 조건의 유형을 가져옵니다.

**Returns:**
int - 보조 제약 조건의 유형.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


WBS 항목(요약 작업)의 순번을 가져옵니다. Primavera에서 요약 작업을 정렬하는 데 사용됩니다.

--------------------

WBS 항목(요약 작업)에 적용됩니다.

**Returns:**
int - WBS 항목(요약 작업)의 순번.
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


단위 완료 퍼센트의 값을 가져옵니다.

**Returns:**
double - 단위 완료 비율의 값.
