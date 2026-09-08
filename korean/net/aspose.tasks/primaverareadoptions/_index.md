---
title: "클래스 PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.PrimaveraReadOptions 클래스. Primavera Xml 또는 Primavera Xer 파일을 읽을 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 1370
url: /ko/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Primavera Xml 또는 Primavera Xer 파일을 읽을 때 추가 옵션을 지정할 수 있게 합니다.

```csharp
public class PrimaveraReadOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | `PrimaveraReadOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 가져오거나 설정합니다. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 가져오거나 설정합니다. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | 베이스라인 프로젝트를 로드할지 여부를 지정하는 플래그를 가져오거나 설정합니다. 기본값은 true입니다. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | XER 형식에서 읽은 정의되지 않은 제약 조건을 가진 작업을 처리하는 동작을 지정합니다. |

## 예제

여러 프로젝트가 포함된 Primavera XML 또는 Primavera XER 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


