---
title: "Rsc.WindowsUserAccount"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'account NT associato a una risorsa"
type: docs
weight: 680
url: /it/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

L'account NT associato a una risorsa.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
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


