---
title: "Klasse Licentie"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.License‑klasse. Biedt methoden om het component te licentiëren"
type: docs
weight: 980
url: /nl/net/aspose.tasks/license/
---
## License class

Biedt methoden om het component te licentiëren.

```csharp
public sealed class License
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [License](license/)() | Initialiseert een nieuw exemplaar van de `License`‑klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Licentieert het component. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Licentieert het component. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


