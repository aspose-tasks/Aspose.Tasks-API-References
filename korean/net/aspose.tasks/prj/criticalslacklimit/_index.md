---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 중요 작업으로 간주합니다"
type: docs
weight: 140
url: /ko/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

총 여유 시간이 이 일수 이하이면 MS Project에서 작업을 Critical로 간주합니다.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## 예제

Prj.CriticalSlackLimit 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


