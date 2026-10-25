---
title: "Aspose::Tasks::License classe"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks per C++"
description: "Fornisce metodi per licenziare il componente."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/license/
---

## License class

Fornisce metodi per licenziare il componente.

In questo esempio, si cercherà di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene <ms> il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di ingresso e poi nelle risorse incorporate dell'assembly chiamante.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> il file jar del componente:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](./license/) | Inizializza una nuova istanza della classe License. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Concede la licenza al componente. |

