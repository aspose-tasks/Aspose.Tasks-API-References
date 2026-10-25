---
title: "Asn.Hyperlink"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당과 연결된 하이퍼링크의 제목 또는 설명 텍스트"
type: docs
weight: 280
url: /ko/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

과제와 연결된 하이퍼링크의 제목 또는 설명 텍스트.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## 예제

하이퍼링크 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


