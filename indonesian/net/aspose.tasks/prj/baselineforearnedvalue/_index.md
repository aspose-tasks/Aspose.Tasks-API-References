---
title: "Prj.BaselineForEarnedValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Baseline spesifik yang digunakan untuk menghitung nilai Variance"
type: docs
weight: 80
url: /id/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

Baseline spesifik yang digunakan untuk menghitung nilai Variansi.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


