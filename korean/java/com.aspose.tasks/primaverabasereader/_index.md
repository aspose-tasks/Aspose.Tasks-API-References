---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "다중 프로젝트 Primavera XER 또는 XML 파일에서 프로젝트 UID를 읽는 데 사용할 수 있는 기본 리더를 나타냅니다."
type: docs
weight: 196
url: /ko/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

다중 프로젝트 Primavera XER 또는 XML 파일에서 프로젝트 UID를 읽는 데 사용할 수 있는 기본 리더를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | 프로젝트의 짧은 정보 객체 목록을 반환합니다. |
| [getProjectUids()](#getProjectUids--) | 프로젝트들의 고유 식별자 목록을 반환합니다. |
| [loadProject(int projectUid)](#loadProject-int-) | 지정된 고유 식별자를 사용하여 프로젝트를 로드합니다. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


프로젝트의 짧은 정보 객체 목록을 반환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - 프로젝트의 짧은 정보 객체 목록
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


프로젝트들의 고유 식별자 목록을 반환합니다.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 프로젝트 고유 식별자 목록.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


지정된 고유 식별자를 사용하여 프로젝트를 로드합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectUid | int | 로드할 프로젝트의 고유 식별자입니다. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
