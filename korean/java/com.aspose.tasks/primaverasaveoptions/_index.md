---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 208
url: /ko/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | 새 인스턴스를 초기화합니다 [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | 활동 ID를 재번호 매기기에 사용되는 증가값을 가져옵니다. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | 활동 ID를 재번호 매기기에 사용되는 접두사를 가져옵니다. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | 활동 ID를 재번호 매기기에 사용되는 접미사를 가져옵니다. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | 활동 ID를 재번호 매기기 필요 여부를 나타내는 값을 가져옵니다. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 가져옵니다. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | 활동 ID를 재번호 매기기에 사용되는 증가값을 설정합니다. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | 활동 ID를 재번호 매기기에 사용되는 접두사를 설정합니다. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | 활동 ID를 재번호 매기기에 사용되는 접미사를 설정합니다. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | 활동 ID를 재번호 매기기 필요 여부를 나타내는 값을 설정합니다. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 설정합니다. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


새 인스턴스를 초기화합니다 [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) 클래스.

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


활동 ID를 재번호 매기기에 사용되는 증가값을 가져옵니다.

**Returns:**
int - 활동 ID를 재번호 매기기에 사용되는 증가값.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


활동 ID를 재번호 매기기에 사용되는 접두사를 가져옵니다.

**Returns:**
java.lang.String - 활동 ID를 재번호 매기기에 사용되는 접두사.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


활동 ID를 재번호 매기기에 사용되는 접미사를 가져옵니다.

**Returns:**
int - 활동 ID를 재번호 매기기에 사용되는 접미사.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


활동 ID를 재번호 매기기 필요 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 활동 ID를 재번호 매기기 필요 여부를 나타내는 값.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 가져옵니다.

Primavera 소프트웨어는 리소스를 요약(WBS) 작업에 할당하는 것을 지원하지 않습니다. 따라서 이러한 할당을 내보내면 Primavera 모델에 따라 잘못된 파일이 될 수 있습니다. true인 경우, 요약 작업에 대한 할당은 내보내기 중에 건너뛰어집니다. false(기본값)인 경우, 내보내기 중에 요약 작업에 할당이 발견되면 예외가 발생합니다.

**Returns:**
boolean - 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


활동 ID를 재번호 매기기에 사용되는 증가값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 활동 ID를 재번호 매기기에 사용되는 증가값. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


활동 ID를 재번호 매기기에 사용되는 접두사를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 활동 ID를 재번호 매기기에 사용되는 접두사. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


활동 ID를 재번호 매기기에 사용되는 접미사를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 활동 ID를 재번호 매기기에 사용되는 접미사. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


활동 ID를 재번호 매기기 필요 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 활동 ID를 재번호 매기기 필요 여부를 나타내는 값. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 설정합니다.

Primavera 소프트웨어는 리소스를 요약(WBS) 작업에 할당하는 것을 지원하지 않습니다. 따라서 이러한 할당을 내보내면 Primavera 모델에 따라 잘못된 파일이 될 수 있습니다. true인 경우, 요약 작업에 대한 할당은 내보내기 중에 건너뛰어집니다. false(기본값)인 경우, 내보내기 중에 요약 작업에 할당이 발견되면 예외가 발생합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값. |

