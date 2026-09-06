---
title: "Resource.TimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient ou définit une instance de la classe TimephasedDataCollection pour cet objet"
type: docs
weight: 740
url: /fr/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Obtient ou définit une instance de la classe [`TimephasedDataCollection`](../../timephaseddatacollection/) pour cet objet.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Remarques

Lecture prise en charge uniquement au format XML.

## Exemples

Montre comment lire les données temporelles d’une ressource.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// itérer sur les données temporelles de la ressource 
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


