---
title: "Classe ViewCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ViewCollection. Contiene un elenco di oggetti View. Implementa l'interfaccia ICollectionView"
type: docs
weight: 2900
url: /it/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Contiene un elenco di oggetti [`View`](../view/). Implementa l'interfaccia ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Ottiene il genitore dell'oggetto View. Solo lettura [`Project`](../project/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Cerca una View con il nome e restituisce la prima occorrenza nella collezione. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Cerca una View con la proprietà Screen specificata e restituisce la prima occorrenza nella collezione. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Converte una collezione di view in un elenco di oggetti [`View`](../view/). |

## Esempi

Mostra come lavorare con le collezioni di view.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// converti in un semplice elenco di view
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// aggiungi una nuova view
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// itera sulle view
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// rimuovi tutte le view in una volta
project.Views.Clear();

// oppure una alla volta
{
    // approccio 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // approccio 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### Vedi anche

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


