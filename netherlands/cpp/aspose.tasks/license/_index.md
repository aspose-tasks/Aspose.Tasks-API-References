---
title: "Aspose::Tasks::License klasse"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks voor C++"
description: "Biedt methoden om het component te licentiëren."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/license/
---

## License class

Biedt methoden om het component te licentiëren.

In dit voorbeeld wordt geprobeerd een licentiebestand met de naam MyLicense.lic te vinden in de map die <ms> de component bevat, in de map die de aanroepende assembly bevat, in de map van de entry‑assembly en vervolgens in de ingesloten bronnen van de aanroepende assembly.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> het component-jarbestand:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [License](./license/) | Initialiseert een nieuw exemplaar van de License‑klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Licentieert de component. |

