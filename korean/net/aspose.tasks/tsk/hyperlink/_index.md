---
title: "Tsk.Hyperlink"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업과 연결된 하이퍼링크의 제목 또는 설명 텍스트"
type: docs
weight: 490
url: /ko/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

작업에 연결된 하이퍼링크의 제목 또는 설명 텍스트입니다.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## 예제

Tsk.Hyperlink 속성을 읽고/쓰는 방법을 보여줍니다.

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

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


