---
title: "열거형 ApplicationInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ApplicationInfo 열거형. 파일이 생성된 프로젝트 버전을 지정합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

파일이 생성된 프로젝트 버전을 지정합니다.

```csharp
public enum ApplicationInfo
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `0` | 정의할 수 없습니다. |
| MSP2000 | `1` | 파일이 Microsoft Project 2000/2002에서 생성되었습니다. |
| MSP2003 | `2` | 파일이 Microsoft Project 2003에서 생성되었습니다. |
| MSP2007 | `3` | 파일이 Microsoft Project 2007에서 생성되었습니다. |
| MSP2010 | `4` | 파일이 Microsoft Project 2010에서 생성되었습니다. |
| MSP2013 | `5` | 파일이 Microsoft Project 2013에서 생성되었습니다. |
| MSP2016 | `6` | 파일이 Microsoft Project 2016에서 생성되었습니다. |

## 예제

프로젝트 애플리케이션 정보를 확인하는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


