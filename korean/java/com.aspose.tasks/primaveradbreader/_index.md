---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "Primavera DB에서 프로젝트 정보를 읽는 리더를 나타냅니다."
type: docs
weight: 200
url: /ko/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Primavera DB에서 프로젝트 정보를 읽는 리더를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | 새로운 [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) 클래스의 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | 지정된 고유 식별자를 사용하여 프로젝트를 로드합니다. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


새로운 [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) 클래스의 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Primavera DB에 연결하는 방법을 지정하는 설정. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
