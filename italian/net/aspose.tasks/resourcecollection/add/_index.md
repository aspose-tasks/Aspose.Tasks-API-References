---
title: "ResourceCollection.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceCollection. Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto"
type: docs
weight: 40
url: /it/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto.

```csharp
public Resource Add()
```

### Valore di ritorno

Risorsa aggiunta.

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

---

## Add(string) {#add_1}

Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto.

```csharp
public Resource Add(string resourceName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| resourceName | Stringa | Nome di una risorsa. |

### Valore di ritorno

Risorsa aggiunta.

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

---

## Add(string, int) {#add_2}

Aggiunge una nuova risorsa nella posizione specificata della collezione di risorse di un progetto.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| resourceName | Stringa | Nome di una risorsa. |
| beforeResourceId | Int32 | Posizione della risorsa precedente in una raccolta di risorse del progetto. |

### Valore di ritorno

Risorsa aggiunta.

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


