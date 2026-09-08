---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 파일에서 프로젝트 파일 정보를 읽습니다"
type: docs
weight: 1280
url: /ko/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

파일에서 프로젝트 파일 정보를 읽습니다.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 파일명 | 문자열 | 프로젝트 파일 이름입니다. |

### 반환 값

프로젝트 파일 정보 [`ProjectFileInfo`](../../projectfileinfo/).

## 예제

XML 파일에서 읽은 프로젝트 파일 정보를 읽는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

스트림에서 프로젝트 파일 정보를 가져옵니다.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 데이터 스트림입니다. |

### 반환 값

프로젝트 파일 정보 [`ProjectFileInfo`](../../projectfileinfo/).

## 예제

스트림에서 읽은 XML 파일의 프로젝트 파일 정보를 읽는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### 또 보기

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


