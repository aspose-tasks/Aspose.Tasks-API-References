---
title: "클래스 ProjectFileInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectFileInfo 클래스. 이 클래스 인스턴스는 프로젝트 파일 형식 및 파일이 생성된 Microsoft Project 버전에 대한 정보를 포함합니다."
type: docs
weight: 1460
url: /ko/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

클래스 인스턴스는 파일이 생성된 Microsoft Project의 프로젝트 파일 형식 및 버전에 대한 정보를 포함합니다.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Aspose.Tasks가 프로젝트 파일을 처리할 수 있는지 여부를 나타내는 값을 가져옵니다. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | 프로젝트가 비밀번호로 보호되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | 프로젝트 파일 애플리케이션 정보를 가져옵니다. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | 프로젝트 파일 형식을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | `ProjectFileInfo` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

## 비고

라이브러리가 프로젝트 파일을 처리할 수 있음을 정의하려면 CanRead 속성을 사용하십시오.

## 예제

프로젝트 파일 정보를 읽는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


