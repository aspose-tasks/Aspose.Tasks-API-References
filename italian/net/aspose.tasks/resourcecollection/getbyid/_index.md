---
title: "ResourceCollection.GetById"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceCollection. Restituisce una risorsa con l'id specificato"
type: docs
weight: 60
url: /it/net/aspose.tasks/resourcecollection/getbyid/
---
## ResourceCollection.GetById method

Restituisce una risorsa con l'id specificato.

```csharp
public Resource GetById(int id)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | Int32 | L'id specificato. |

### Valore di ritorno

Risorsa con l'id specificato se presente; altrimenti, null.

## Osservazioni

Complessità O(1).

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


