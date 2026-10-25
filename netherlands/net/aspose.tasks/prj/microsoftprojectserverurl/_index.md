---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of een project is gemaakt door een Project Server-gebruiker in plaats van een NT-gebruiker"
type: docs
weight: 460
url: /nl/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Bepaalt of een project is aangemaakt door een Project Server-gebruiker in plaats van een NT-gebruiker.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Voorbeelden

Toont hoe de eigenschap Prj.MicrosoftProjectServerURL te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


