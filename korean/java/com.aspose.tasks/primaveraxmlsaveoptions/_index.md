---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 Primavera xml 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 212
url: /ko/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

프로젝트를 Primavera xml 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | 새 인스턴스를 초기화합니다. [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | 루트 작업을 저장할지 여부를 나타내는 값을 가져옵니다. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 가져옵니다. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | 루트 작업을 저장할지 여부를 나타내는 값을 설정합니다. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 설정합니다. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


새 인스턴스를 초기화합니다. [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) 클래스.

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


루트 작업을 저장할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 루트 작업을 저장할지 여부를 나타내는 값.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값을 가져옵니다.

Primavera 소프트웨어는 리소스를 요약(WBS) 작업에 할당하는 것을 지원하지 않습니다. 따라서 이러한 할당을 내보내면 Primavera 모델에 따라 잘못된 파일이 될 수 있습니다. true인 경우, 요약 작업에 대한 할당은 내보내기 중에 건너뛰어집니다. false(기본값)인 경우, 내보내기 중에 요약 작업에 할당이 발견되면 예외가 발생합니다.

**Returns:**
boolean - 리소스를 요약 작업에 할당하는 것을 내보내기 중에 건너뛸지 여부를 나타내는 값.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


루트 작업을 저장할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 루트 작업을 저장할지 여부를 나타내는 값. |

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

