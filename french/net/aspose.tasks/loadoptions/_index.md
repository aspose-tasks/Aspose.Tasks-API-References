---
title: "Classe LoadOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.LoadOptions. Permet de spécifier des paramètres de chargement supplémentaires lors du chargement d'un projet à partir d'un fichier ou d'un flux."
type: docs
weight: 990
url: /fr/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Permet de spécifier des paramètres de chargement supplémentaires lors du chargement d'un projet depuis un fichier ou un flux.

```csharp
public class LoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LoadOptions](loadoptions/)() | Initialise une nouvelle instance de la classe `LoadOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Obtient ou définit un jeton qui peut être utilisé pour annuler une opération de chargement de projet. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Obtient ou définit l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. L'encodage par défaut est UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Obtient ou définit une méthode de rappel pour gérer les erreurs d'analyse XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Obtient ou définit un mot de passe de protection. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Obtient ou définit une instance spécifiée de la classe [`PrimaveraReadOptions`](../primaverareadoptions/) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Obtient ou définit le rappel à invoquer pendant les opérations de chargement de projet. Actuellement pris en charge pour les formats MPP et XER. |

## Exemples

Montre comment charger le projet protégé par mot de passe en utilisant une instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


