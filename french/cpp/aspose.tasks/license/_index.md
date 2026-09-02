---
title: "Aspose::Tasks::License classe"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks pour C++"
description: "Fournit des méthodes pour licencier le composant."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/license/
---

## License class

Fournit des méthodes pour licencier le composant.

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier contenant <ms> le composant, dans le dossier contenant l'assembly appelant, dans le dossier de l'assembly d'entrée puis dans les ressources intégrées de l'assembly appelant.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> le fichier jar du composant :

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Constructeurs

| Nom | Description |
| --- | --- |
| [License](./license/) | Initialise une nouvelle instance de la classe License. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Licence le composant. |

