---
title: "License.License"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "License constructor. Initialiseert een nieuw exemplaar van de License-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/license/license/
---
## License constructor

Initialiseert een nieuw exemplaar van de [`License`](../) klasse.

```csharp
public License()
```

## Voorbeelden

In dit voorbeeld wordt geprobeerd een licentiebestand met de naam MyLicense.lic te vinden in de map die het component bevat, in de map die de aanroepende assembly bevat, in de map van de entry‑assembly en vervolgens in de ingebedde resources van de aanroepende assembly.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

het component‑jar‑bestand:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Toont hoe een licentie van Aspose.Tasks toe te passen.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Zie ook

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


