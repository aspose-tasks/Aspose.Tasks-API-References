---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera 형식에서 로드된 프로젝트에 대한 간략한 정보를 나타냅니다."
type: docs
weight: 204
url: /ko/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Primavera 형식에서 로드된 프로젝트에 대한 간략한 정보를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | 프로젝트의 export flag를 가져옵니다. |
| [getName()](#getName--) | 프로젝트의 이름을 가져옵니다. |
| [getShortName()](#getShortName--) | 프로젝트의 짧은 이름(Project ID)을 가져옵니다. |
| [getUid()](#getUid--) | 프로젝트의 Uid를 가져옵니다. |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


프로젝트의 export flag를 가져옵니다. Primavera에서 프로젝트가 내보내기로 선택되면 해당 ExportFlag가 true가 됩니다. 명시적으로 내보내기로 선택되지 않은 일부 프로젝트도 내보낸 프로젝트와의 관계 때문에 XER 파일로 내보내질 수 있습니다.

**Returns:**
boolean - 프로젝트의 export flag.
### getName() {#getName--}
```
public final String getName()
```


프로젝트의 이름을 가져옵니다.

**Returns:**
java.lang.String - 프로젝트의 이름.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


프로젝트의 짧은 이름(Project ID)을 가져옵니다.

**Returns:**
java.lang.String - 프로젝트의 짧은 이름(Project ID).
### getUid() {#getUid--}
```
public final int getUid()
```


프로젝트의 Uid를 가져옵니다.

**Returns:**
int - 프로젝트의 Uid.
