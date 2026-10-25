---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目创建的日期和时间"
type: docs
weight: 130
url: /zh/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

项目创建的日期和时间。

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## 备注

以 UTC 格式保存在 mpp 文件中。DateTime 类型。

## 示例

展示如何读取/写入 Prj.CreationDate 属性。

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


