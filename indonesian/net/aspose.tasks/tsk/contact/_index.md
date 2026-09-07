---
title: "Tsk.Contact"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Nama individu yang bertanggung jawab atas sebuah tugas"
type: docs
weight: 220
url: /id/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Nama individu yang bertanggung jawab atas sebuah tugas.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


