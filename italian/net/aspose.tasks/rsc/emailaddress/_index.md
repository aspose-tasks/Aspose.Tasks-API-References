---
title: "Rsc.EMailAddress"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'indirizzo email di una risorsa"
type: docs
weight: 280
url: /it/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

L'indirizzo email di una risorsa.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## Esempi

Mostra come impostare le proprietà meta della risorsa.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Aggiungi risorsa e imposta i metadati della risorsa
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


