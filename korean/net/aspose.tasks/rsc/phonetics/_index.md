---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스 이름의 음성 표기. 일본어 전용 사용"
type: docs
weight: 560
url: /ko/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

리소스 이름의 음성 철자. 일본어 전용 사용.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## 예제

Rsc.Phonetics 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


