---
title: "LoadOptions.Password"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta una password di protezione."
type: docs
weight: 50
url: /it/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Ottiene o imposta una password di protezione.

```csharp
public string Password { get; set; }
```

## Esempi

Mostra come caricare il progetto protetto da password usando l'istanza &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

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

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


