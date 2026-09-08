---
title: "Rsc.EMailAddress"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La dirección de correo electrónico de un recurso"
type: docs
weight: 280
url: /es/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

La dirección de correo electrónico de un recurso.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## Ejemplos

Muestra cómo establecer las meta propiedades de un recurso.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Agregar recurso y establecer los metadatos del recurso
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


