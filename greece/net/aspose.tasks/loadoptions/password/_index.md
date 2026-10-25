---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα LoadOptions. Λαμβάνει ή ορίζει έναν κωδικό προστασίας."
type: docs
weight: 50
url: /el/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Λαμβάνει ή ορίζει έναν κωδικό προστασίας.

```csharp
public string Password { get; set; }
```

## Παραδείγματα

Δείχνει πώς να φορτώσετε το έργο με προστασία κωδικού χρησιμοποιώντας την παρουσία &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Δείτε επίσης

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


