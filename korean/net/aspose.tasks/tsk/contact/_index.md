---
title: "Tsk.Contact"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 책임이 있는 개인의 이름"
type: docs
weight: 220
url: /ko/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

작업에 책임이 있는 개인의 이름.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## 예제

Tsk.Contact 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


