---
title: "Rsc.WindowsUserAccount"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cuenta NT asociada a un recurso"
type: docs
weight: 680
url: /es/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

La cuenta NT asociada a un recurso.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
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


