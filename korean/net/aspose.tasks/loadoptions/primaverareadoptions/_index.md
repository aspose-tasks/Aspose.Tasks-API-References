---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LoadOptions 속성. PrimaveraReadOptions 클래스의 지정된 인스턴스를 가져오거나 설정합니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

[`PrimaveraReadOptions`](../../primaverareadoptions/) 클래스의 지정된 인스턴스를 가져오거나 설정합니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다.

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


