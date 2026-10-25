---
title: "Tsk.Contact"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το όνομα ενός ατόμου που είναι υπεύθυνο για μια εργασία"
type: docs
weight: 220
url: /el/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Το όνομα ενός ατόμου υπεύθυνου για μια εργασία.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


