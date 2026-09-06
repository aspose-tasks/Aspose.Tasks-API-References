---
title: "Tsk.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务关联的超链接中文档的具体位置"
type: docs
weight: 510
url: /zh/net/aspose.tasks/tsk/hyperlinksubaddress/
---
## Tsk.HyperlinkSubAddress field

与任务关联的超链接在文档中的具体位置。

```csharp
public static readonly Key<string, TaskKey> HyperlinkSubAddress;
```

## 备注

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 和 HyperlinkSubAddress 的拼接。

## 示例

展示如何读取/写入 Tsk.Hyperlink 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


