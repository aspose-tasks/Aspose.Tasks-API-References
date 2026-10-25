---
title: "License.License"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "License constructor. Initialise une nouvelle instance de la classe License"
type: docs
weight: 10
url: /fr/net/aspose.tasks/license/license/
---
## License constructor

Initialise une nouvelle instance de la classe [`License`](../).

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


