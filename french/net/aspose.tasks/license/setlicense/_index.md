---
title: "License.SetLicense"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode License. Accorde une licence au composant"
type: docs
weight: 20
url: /fr/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licence le composant.

```csharp
public void SetLicense(string licenseName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| licenseName | Chaîne | Peut être un nom de fichier complet ou court ou le nom d'une ressource intégrée. Utilisez une chaîne vide pour passer en mode d'évaluation. |

## Remarques

Recherche la licence aux emplacements suivants :

1. Chemin explicite.

2. Le dossier qui contient l'assembly du composant Aspose.

3. Le dossier qui contient l'assembly appelant du client.

4. Le dossier qui contient l'assembly d'entrée (démarrage).

5. Une ressource intégrée dans l'assembly appelant du client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Chemin explicite.

2. Une ressource intégrée dans l'assembly appelant du client.

2. Le dossier qui contient le fichier JAR du composant Aspose.

3. Le dossier qui contient le fichier JAR appelant du client.

## Exemples

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier contenant le composant, dans le dossier contenant l’assembly appelant, dans le dossier de l’assembly d’entrée, puis dans les ressources incorporées de l’assembly appelant.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

---

## SetLicense(Stream) {#setlicense}

Licence le composant.

```csharp
public void SetLicense(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Un flux qui contient la licence. |

## Remarques

Utilisez cette méthode pour charger une licence depuis un flux.

## Exemples

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Montre comment appliquer une licence d'Aspose.Tasks lue depuis &lt;see cref="System.IO.FileStream" /&gt;.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### Voir aussi

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


