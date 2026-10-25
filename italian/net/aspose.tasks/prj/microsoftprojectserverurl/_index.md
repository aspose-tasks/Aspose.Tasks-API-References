---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se un progetto è stato creato da un utente Project Server rispetto a un utente NT"
type: docs
weight: 460
url: /it/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Determina se un progetto è stato creato da un utente Project Server rispetto a un utente NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


