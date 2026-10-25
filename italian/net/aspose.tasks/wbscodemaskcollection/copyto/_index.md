---
title: "WBSCodeMaskCollection.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo WBSCodeMaskCollection. Copia gli elementi di questa collezione nell'array specificato a partire dall'indice specificato"
type: docs
weight: 60
url: /it/net/aspose.tasks/wbscodemaskcollection/copyto/
---
## WBSCodeMaskCollection.CopyTo method

Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato.

```csharp
public void CopyTo(WBSCodeMask[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | WBSCodeMask[] | l'array monodimensionale specificato a cui copiare gli elementi |
| arrayIndex | Int32 | l'indice basato su zero dell'array specificato al quale inizia la copia. |

## Esempi

Mostra come lavorare con la collezione di maschere di codice WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

project.WBSCodeDefinition.CodeMaskCollection.Clear();

var mask1 = new WBSCodeMask();
mask1.Length = 2;
mask1.Separator = "-";
mask1.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask1);

var mask2 = new WBSCodeMask();
mask2.Length = 1;
mask2.Separator = "-";
mask2.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask2);

Console.WriteLine("WBS Code mask's count: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
Console.WriteLine("Is WBS Code mask collection read-only?: " + project.WBSCodeDefinition.CodeMaskCollection.IsReadOnly);
Console.WriteLine("Masks: ");
Console.WriteLine();
foreach (var wbsMask in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var task1 = project.RootTask.Children.Add("Task 1");
task1.Children.Add("Task 2");

project.Recalculate();

IEnumerable<Task> childTasks = project.RootTask.SelectAllChildTasks();
foreach (var childTask in childTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}

project.WBSCodeDefinition.CodeMaskCollection.Remove(mask2);

if (project.WBSCodeDefinition.CodeMaskCollection.Contains(mask2))
{
    throw new InvalidOperationException("WBS code mask wasn't removed.");
}

var otherProject = new Project();
otherProject.WBSCodeDefinition = new WBSCodeDefinition();
otherProject.WBSCodeDefinition.GenerateWBSCode = true;
otherProject.WBSCodeDefinition.VerifyUniqueness = true;
otherProject.WBSCodeDefinition.CodePrefix = "CRS-";

// copia le maschere di codice in un altro progetto
var masks = new WBSCodeMask[project.WBSCodeDefinition.CodeMaskCollection.Count];
project.WBSCodeDefinition.CodeMaskCollection.CopyTo(masks, 0);

foreach (var mask in masks)
{
    otherProject.WBSCodeDefinition.CodeMaskCollection.Add(mask);
}

List<WBSCodeMask> wbsMasks = otherProject.WBSCodeDefinition.CodeMaskCollection.ToList();
foreach (var wbsMask in wbsMasks)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var otherTask1 = project.RootTask.Children.Add("Other task 1");
otherTask1.Children.Add("Other task 2");

otherProject.Recalculate();

Console.WriteLine("Print WBS codes of the other project: ");
IEnumerable<Task> otherChildTasks = otherProject.RootTask.SelectAllChildTasks();
foreach (var childTask in otherChildTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}
```

### Vedi anche

* class [WBSCodeMask](../../wbscodemask/)
* class [WBSCodeMaskCollection](../)
* namespace [Aspose.Tasks](../../wbscodemaskcollection/)
* assembly [Aspose.Tasks](../../../)


