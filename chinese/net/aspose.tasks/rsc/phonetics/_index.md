---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源名称的音标拼写。仅用于日语。"
type: docs
weight: 560
url: /zh/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

资源名称的音标拼写。仅用于日语。

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## 示例

展示如何读取/写入 Rsc.Phonetics 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


