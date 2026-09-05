---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "MS Project Server 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다."
type: docs
weight: 161
url: /ko/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

MS Project Server 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | 새 인스턴스를 초기화합니다 [MspDbSettings](../../com.aspose.tasks/mspdbsettings) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | 읽을 프로젝트의 GUID를 가져옵니다. |
| [getSchema()](#getSchema--) | MS Project Server의 스키마를 가져옵니다. |
| [setSchema(String value)](#setSchema-java.lang.String-) | MS Project Server의 스키마를 설정합니다. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


새 인스턴스를 초기화합니다 [MspDbSettings](../../com.aspose.tasks/mspdbsettings) 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| connectionString | java.lang.String | 지정된 연결 문자열입니다. |
| projectGuid | java.util.UUID | 읽을 프로젝트의 지정된 GUID입니다. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


읽을 프로젝트의 GUID를 가져옵니다.

**Returns:**
java.util.UUID - 읽을 프로젝트의 GUID입니다.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


MS Project Server의 스키마를 가져옵니다. 기본값은 "pub"입니다.

**Returns:**
java.lang.String - MS Project Server의 스키마입니다.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


MS Project Server의 스키마를 설정합니다. 기본값은 "pub"입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | MS Project Server의 스키마입니다. |

