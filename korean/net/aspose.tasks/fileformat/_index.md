---
title: "Enum FileFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.FileFormat 열거형. 프로젝트 파일 형식을 지정합니다"
type: docs
weight: 590
url: /ko/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

프로젝트 파일 형식을 지정합니다.

```csharp
public enum FileFormat
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `0` | 정의할 수 없습니다. |
| P6XML | `1` | Primavera P6 XML 형식을 나타냅니다. |
| XML | `2` | Microsoft Project XML 형식. |
| MPP8 | `3` | Microsoft Project 2000 형식. |
| MPP9 | `4` | Microsoft Project 2003 형식. |
| MPP12 | `5` | Microsoft Project 2007 형식. |
| MPP14 | `6` | Microsoft Project 2010 형식. |
| MPT9 | `7` | Microsoft Project 2003 템플릿 형식. |
| MPT12 | `8` | Microsoft Project 2007 템플릿 형식. |
| MPT14 | `9` | Microsoft Project 2010 (2013) 템플릿 형식. |
| MPX | `10` | Mpx 파일 형식 |
| XER | `11` | Primavera XER 형식을 나타냅니다 |
| HTML | `12` | HTML 형식을 나타냅니다 |
| ProjectServer | `13` | 프로젝트가 Project Server 또는 Project Online에서 읽혔습니다 |

## 예제

프로젝트 파일 형식을 읽는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


