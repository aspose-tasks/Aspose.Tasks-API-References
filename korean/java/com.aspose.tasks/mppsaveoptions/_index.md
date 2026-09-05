---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 데이터를 MPP로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 149
url: /ko/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

프로젝트 데이터를 MPP로 저장할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | 새 인스턴스를 초기화합니다 [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getClearVba()](#getClearVba--) | 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 가져옵니다. |
| [getProtectionPassword()](#getProtectionPassword--) | 결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 가져옵니다. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 가져옵니다. |
| [getWriteFilters()](#getWriteFilters--) | 프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 가져옵니다. |
| [getWriteGroups()](#getWriteGroups--) | 프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값을 가져옵니다. |
| [getWriteVba()](#getWriteVba--) | MPP 파일의 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 가져옵니다. |
| [getWriteViewData()](#getWriteViewData--) | 프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값을 가져옵니다. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 설정합니다. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | 결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 설정합니다. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 설정합니다. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | 프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 설정합니다. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | 프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값을 설정합니다. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | MPP 파일의 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 설정합니다. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | 프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값을 설정합니다. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


새 인스턴스를 초기화합니다 [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) 클래스.

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 가져옵니다. 현재 MS Project 2010 및 이후 형식에서 지원됩니다.

--------------------

null 값은 프로젝트 파일이 보호되지 않음을 나타냅니다.

**Returns:**
java.lang.String - 결과 MPP 파일을 보호하는 데 사용되는 비밀번호.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 가져옵니다.

--------------------

MS Project는 각 작업에 대해 빈 리소스 할당을 생성합니다. 저장 시 이를 제거하려면 이 플래그를 true로 설정하십시오.

**Returns:**
boolean - MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 가져옵니다.

--------------------

필터 데이터에는 Project.TaskFilters 및 Project.ResourceFilters 컬렉션이 포함됩니다.

--------------------

현재 MSP 2010 또는 이후 형식에서 지원됩니다.

**Returns:**
boolean - 프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값을 가져옵니다.

--------------------

그룹 데이터에는 Project.TaskGroups 및 Project.ResourceGroups 컬렉션이 포함됩니다.

**Returns:**
boolean - 프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 가져옵니다. 현재 VbaModule.SourceCode의 쓰기가 지원됩니다.

**Returns:**
boolean - MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값을 가져옵니다.

--------------------

뷰 데이터에는 Project.Views, Filters 및 Tables 컬렉션이 포함됩니다.

**Returns:**
boolean - 프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 설정합니다. 현재 MS Project 2010 및 이후 형식에서 지원됩니다.

--------------------

null 값은 프로젝트 파일이 보호되지 않음을 나타냅니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 결과 MPP 파일을 보호하는 데 사용되는 비밀번호. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 설정합니다.

--------------------

MS Project는 각 작업에 대해 빈 리소스 할당을 생성합니다. 저장 시 이를 제거하려면 이 플래그를 true로 설정하십시오.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 설정합니다.

--------------------

필터 데이터에는 Project.TaskFilters 및 Project.ResourceFilters 컬렉션이 포함됩니다.

--------------------

현재 MSP 2010 또는 이후 형식에서 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값을 설정합니다.

--------------------

그룹 데이터에는 Project.TaskGroups 및 Project.ResourceGroups 컬렉션이 포함됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트를 MPP 형식으로 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 설정합니다. 현재 VbaModule.SourceCode의 쓰기가 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값을 설정합니다.

--------------------

뷰 데이터에는 Project.Views, Filters 및 Tables 컬렉션이 포함됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트를 MPP 형식으로 저장할 때 뷰 데이터를 기록할지 여부를 나타내는 값. |

