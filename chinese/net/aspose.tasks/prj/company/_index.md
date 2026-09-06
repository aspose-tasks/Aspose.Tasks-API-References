---
title: "Prj.Company"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。创建项目的公司。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/prj/company/
---
## Prj.Company field

创建项目的公司。

```csharp
public static readonly Key<string, PrjKey> Company;
```

## 示例

展示如何读取/写入 Prj.Company 属性。

```csharp
var project = new Project();

project.Set(Prj.Company, "Aspose");

Console.WriteLine("Company: " + project.Get(Prj.Company));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


