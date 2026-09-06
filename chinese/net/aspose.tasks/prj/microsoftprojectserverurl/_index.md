---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定项目是由 Project Server 用户创建还是 NT 用户创建"
type: docs
weight: 460
url: /zh/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

确定项目是由 Project Server 用户还是 NT 用户创建的。

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## 示例

展示如何读取/写入 Prj.MicrosoftProjectServerURL 属性。

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


