---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera Xml 또는 Primavera Xer 파일을 읽을 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 206
url: /ko/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Primavera Xml 또는 Primavera Xer 파일을 읽을 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | 새 인스턴스를 초기화합니다 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 가져옵니다. |
| [getProjectUid()](#getProjectUid--) | 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 가져옵니다. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | 베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그를 가져옵니다. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작을 지정합니다. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 설정합니다. |
| [setProjectUid(int value)](#setProjectUid-int-) | 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 설정합니다. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | 베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그를 설정합니다. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작을 지정합니다. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


새 인스턴스를 초기화합니다 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 클래스.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 가져옵니다.

**Returns:**
boolean - 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 가져옵니다.

**Returns:**
int - 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그를 가져옵니다. 기본값은 true입니다.

--------------------

이 플래그는 베이스라인 프로젝트가 포함된 Primavera XML 파일에 적용됩니다 (베이스라인은 XER 형식에서 지원되지 않습니다). 베이스라인 데이터가 필요하지 않을 때 큰 프로젝트의 로딩 속도를 높이기 위해 옵션을 false로 설정할 수 있습니다.

**Returns:**
boolean - 베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작을 지정합니다.

**Returns:**
int - XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그를 설정합니다. 기본값은 true입니다.

--------------------

이 플래그는 베이스라인 프로젝트가 포함된 Primavera XML 파일에 적용됩니다 (베이스라인은 XER 형식에서 지원되지 않습니다). 베이스라인 데이터가 필요하지 않을 때 큰 프로젝트의 로딩 속도를 높이기 위해 옵션을 false로 설정할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작을 지정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작. |

