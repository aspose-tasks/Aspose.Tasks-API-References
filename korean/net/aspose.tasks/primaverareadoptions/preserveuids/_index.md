---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraReadOptions 속성. 엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

엔터티의 원래 고유 식별자를 보존할지 여부를 지정하는 플래그를 가져오거나 설정합니다.

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


