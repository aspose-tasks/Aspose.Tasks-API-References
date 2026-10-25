---
title: "ProjectFileInfo.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectFileInfo 메서드. 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(ProjectFileInfo other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | ProjectFileInfo | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

지정된 ProjectFileInfo와 이 인스턴스가 동일한 파일 형식 및 애플리케이션 정보를 가지고 있으면 true를 반환합니다.

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

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

지정된 ProjectFileInfo와 이 인스턴스가 동일한 파일 형식 및 애플리케이션 정보를 가지고 있으면 true를 반환합니다.

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


