---
title: "Classe ResourceCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.ResourceCollection class. Rappresenta una collezione di oggetti Resource"
type: docs
weight: 1770
url: /it/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Rappresenta una collezione di oggetti [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Ottiene il numero di elementi contenuti nella ResourceCollection. Int32 di sola lettura. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Ottiene il progetto genitore dell'oggetto ResourceCollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Aggiunge una nuova risorsa nella posizione specificata della collezione di risorse di un progetto. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | La cancellazione diretta non è supportata, questo metodo lancia semplicemente NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Restituisce una risorsa con l'id specificato. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Restituisce una risorsa con l'Uid specificato. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Questa è l'implementazione stub del metodo Remove di ICollection, che lancia solo NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Converte l'oggetto ResourceCollection in un elenco di oggetti [`Resource`](../resource/). |

## Esempi

Mostra come lavorare con le collezioni di risorse.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// aggiungi risorsa vuota
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// aggiungi risorsa con un nome
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// aggiungi risorsa prima della risorsa con ID specificato
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// ottieni risorsa per id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// le collezioni di risorse non supportano l'operazione Clear
// project.Resources.Clear();
// usa il prossimo esempio di codice invece
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Vedi anche

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


