---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MpdSettings 생성자. MpdSettings 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

새 인스턴스를 초기화합니다. [`MpdSettings`](../) 클래스.

```csharp
public MpdSettings(string connectionString, int projectId)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| connectionString | 문자열 | 지정된 연결 문자열입니다. |
| projectId | Int32 | 읽을 프로젝트의 지정된 ID입니다. |

## 예제

MPD 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


