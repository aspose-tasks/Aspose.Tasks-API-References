---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LoadOptions-eigenschap. Haalt op of stelt een beschermingswachtwoord in."
type: docs
weight: 50
url: /nl/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Haalt een beschermingswachtwoord op of stelt dit in.

```csharp
public string Password { get; set; }
```

## Voorbeelden

Toont hoe een wachtwoordbeveiligd project te laden met een &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instantie.

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

### Zie ook

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


