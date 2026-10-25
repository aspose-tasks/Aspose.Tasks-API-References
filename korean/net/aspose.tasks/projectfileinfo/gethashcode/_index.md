---
title: "ProjectFileInfo.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectFileInfo 메서드. ProjectFileInfo 클래스 인스턴스에 대한 해시 코드 값을 반환합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

[`ProjectFileInfo`](../) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

프로젝트 파일 정보를 읽는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


