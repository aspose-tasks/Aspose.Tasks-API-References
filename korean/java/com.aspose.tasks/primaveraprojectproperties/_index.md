---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera 파일 XER 또는 P6XML에서 읽은 프로젝트에 대한 Primavera 전용 속성을 나타냅니다."
type: docs
weight: 205
url: /ko/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Primavera 파일(XER 또는 P6XML)에서 읽은 프로젝트에 대한 Primavera 전용 속성을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | 현재 프로젝트의 기준선 프로젝트 배열을 가져옵니다. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | 중요 활동을 정의하는 방법을 가져옵니다: 최장 경로 또는 총 여유 시간 방식. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | 총 여유 시간 방식을 사용할 경우 중요한 활동을 정의하는 데 사용되는 임계값을 가져옵니다. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | 현재 기준선 프로젝트의 Id를 가져옵니다. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | 프로젝트 간 활동 관계를 무시할지 여부를 정의하는 플래그를 가져옵니다. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | 프로젝트를 일정에 잡을 때 활동을 중요하게 표시할지 여부를 정의하는 플래그를 가져옵니다. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Primavera 프로젝트에서 관계 지연을 일정에 잡을 때 사용할 캘린더를 정의하는 옵션을 가져옵니다. |
| [getShortName()](#getShortName--) | 프로젝트의 짧은 이름(Project ID)을 가져옵니다. |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | 활동 종료 날짜를 예상 종료 날짜로 일정에 잡을지 여부를 정의하는 플래그를 가져옵니다. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


현재 프로젝트의 기준선 프로젝트 배열을 가져옵니다. 내보낸 기준선이 포함된 Primavera XML 파일에서 읽은 프로젝트에 적용됩니다.

**Returns:**
com.aspose.tasks.Project[] - 현재 프로젝트의 기준선 프로젝트 배열.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


중요 활동을 정의하는 방법을 가져옵니다: 최장 경로 또는 총 여유 시간 방식.

**Returns:**
int - 중요한 활동을 정의하는 방법: 최장 경로 또는 총 여유 시간 방식.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


총 여유 시간 방식을 사용할 경우 중요한 활동을 정의하는 데 사용되는 임계값을 가져옵니다.

**Returns:**
java.lang.Double - 총 여유 시간 방식을 사용할 경우 중요한 활동을 정의하는 데 사용되는 임계값.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


현재 기준선 프로젝트의 Id를 가져옵니다. 내보낸 기준선이 포함된 Primavera XML 파일에서 읽은 프로젝트에 적용됩니다.

**Returns:**
int - 현재 기준선 프로젝트의 Id.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


프로젝트 간 활동 관계를 무시할지 여부를 정의하는 플래그를 가져옵니다.

**Returns:**
boolean - 프로젝트 간 활동 관계를 무시할지 여부를 정의하는 플래그.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


프로젝트를 일정에 잡을 때 활동을 중요하게 표시할지 여부를 정의하는 플래그를 가져옵니다.

**Returns:**
boolean - 프로젝트를 일정에 잡을 때 활동을 중요하게 표시할지 여부를 정의하는 플래그.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Primavera 프로젝트에서 관계 지연을 일정에 잡을 때 사용할 캘린더를 정의하는 옵션을 가져옵니다.

**Returns:**
int - Primavera 프로젝트에서 관계 지연을 일정에 잡을 때 사용할 캘린더를 정의하는 옵션.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


프로젝트의 짧은 이름(Project ID)을 가져옵니다.

**Returns:**
java.lang.String - 프로젝트의 짧은 이름(Project ID).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


활동 종료 날짜를 예상 종료 날짜로 일정에 잡을지 여부를 정의하는 플래그를 가져옵니다.

**Returns:**
boolean - 활동 종료 날짜를 예상 종료 날짜로 일정에 잡을지 여부를 정의하는 플래그.
