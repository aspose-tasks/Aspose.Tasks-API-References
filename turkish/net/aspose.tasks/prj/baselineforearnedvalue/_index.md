---
title: "Prj.BaselineForEarnedValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Varyans değerlerini hesaplamak için kullanılan belirli temel çizgi"
type: docs
weight: 80
url: /tr/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

Varyans değerlerini hesaplamak için kullanılan belirli temel çizgi.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Örnekler

Prj.BaselineForEarnedValue özelliğini nasıl okuma/yazma yapacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


