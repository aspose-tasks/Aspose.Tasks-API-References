---
title: "Classe License"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.License. Fournit des méthodes pour licencier le composant"
type: docs
weight: 980
url: /fr/net/aspose.tasks/license/
---
## License class

Fournit des méthodes pour licencier le composant.

```csharp
public sealed class License
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [License](license/)() | Initialise une nouvelle instance de la classe `License`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Licence le composant. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Licence le composant. |

## Exemples

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier contenant le composant, dans le dossier contenant l’assembly appelant, dans le dossier de l’assembly d’entrée, puis dans les ressources incorporées de l’assembly appelant.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

le fichier jar du composant:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Montre comment appliquer une licence d’Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


