---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 리소스가 루트 리소스인지 여부를 나타내는 플래그를 가져옵니다. 루트 리소스는 MS Projects 형식의 내부를 지원하도록 설계된 특수 리소스로, 사용자 코드에서 직접 사용하도록 의도되지 않았습니다."
type: docs
weight: 470
url: /ko/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

리소스가 루트 리소스인지 여부를 나타내는 플래그를 가져옵니다. 루트 리소스는 MS Project 형식의 내부를 지원하도록 설계된 특수 리소스로, 사용자 코드에서 직접 사용하도록 설계되지 않았습니다.

```csharp
public virtual bool IsRoot { get; }
```

## 예제

루트 리소스를 건너뛰기 위해 IsRoot 속성을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


