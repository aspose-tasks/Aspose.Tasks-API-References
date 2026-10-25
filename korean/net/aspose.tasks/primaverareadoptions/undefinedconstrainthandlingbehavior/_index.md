---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraReadOptions 속성. XER 형식에서 읽은 정의되지 않은 제약 조건이 있는 작업을 처리하는 데 사용되는 동작을 지정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

XER 형식에서 읽은 정의되지 않은 제약 조건을 가진 작업을 처리하는 동작을 지정합니다.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
```

## 예제

지정된 Id를 사용하여 Primavera 프로젝트를 로드하는 방법을 &lt;see cref="LoadOptions" /&gt;를 사용하여 보여줍니다.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// Primavera 읽기 옵션 설정
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// 프로젝트와 작업...
```

### 또 보기

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


