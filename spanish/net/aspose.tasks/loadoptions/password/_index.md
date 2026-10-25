---
title: "LoadOptions.Password"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad LoadOptions. Obtiene o establece una contraseña de protección."
type: docs
weight: 50
url: /es/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Obtiene o establece una contraseña de protección.

```csharp
public string Password { get; set; }
```

## Ejemplos

Muestra cómo cargar el proyecto protegido con contraseña usando una instancia de &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

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

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


