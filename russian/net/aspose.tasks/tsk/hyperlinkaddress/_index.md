---
title: "Tsk.HyperlinkAddress"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Адрес гиперссылки, связанной с задачей"
type: docs
weight: 500
url: /ru/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

Адрес гиперссылки, связанной с задачей.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## Примечания

Полный адрес (Hyperlink Href в Microsoft Project) гиперссылки представляет собой конкатенацию HyperlinkAddress и HyperlinkSubAddress.

## Примеры

Показывает, как читать/записывать свойства Tsk.Hyperlink.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


