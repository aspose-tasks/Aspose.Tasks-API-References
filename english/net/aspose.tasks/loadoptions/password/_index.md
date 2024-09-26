---
title: LoadOptions.Password
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets a protection password
type: docs
weight: 50
url: /net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Gets or sets a protection password.

```csharp
public string Password { get; set; }
```

## Examples

Shows how to load the password-protected project using &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

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

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


