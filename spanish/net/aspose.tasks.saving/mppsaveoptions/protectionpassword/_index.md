---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece una contraseña que se usa para proteger el archivo MPP resultante. Actualmente es compatible con los formatos MS Project 2010 y posteriores. Un valor nulo indica que el archivo del proyecto no está protegido."
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Obtiene o establece una contraseña que se utiliza para proteger el archivo MPP resultante. Actualmente se admite para los formatos de MS Project 2010 y posteriores. Un valor nulo indica que el archivo del proyecto no está protegido.

```csharp
public string ProtectionPassword { get; set; }
```

## Ejemplos

Muestra cómo guardar un proyecto en un archivo MPP protegido con contraseña.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### Ver también

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


