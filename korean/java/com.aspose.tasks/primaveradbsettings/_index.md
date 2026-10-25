---
title: "PrimaveraDbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다."
type: docs
weight: 201
url: /ko/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

Primavera 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getProjectId()](#getProjectId--) | 읽을 프로젝트의 ID를 가져옵니다. |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


[PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| connectionString | java.lang.String | 지정된 연결 문자열입니다. |
| projectId | int | 읽을 프로젝트의 지정된 ID. |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


읽을 프로젝트의 ID를 가져옵니다.

**Returns:**
int - 읽을 프로젝트의 ID.
