---
title: "Tsk.HyperlinkAddress"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업과 연결된 하이퍼링크 주소"
type: docs
weight: 500
url: /ko/net/aspose.tasks/tsk/hyperlinkaddress/
---
## Tsk.HyperlinkAddress field

작업에 연결된 하이퍼링크의 주소입니다.

```csharp
public static readonly Key<string, TaskKey> HyperlinkAddress;
```

## 비고

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 문자열입니다.

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


