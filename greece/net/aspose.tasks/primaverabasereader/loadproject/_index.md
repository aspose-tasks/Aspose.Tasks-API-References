---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος PrimaveraBaseReader. Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό"
type: docs
weight: 30
url: /el/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectUid | Int32 | Μοναδικό αναγνωριστικό του έργου που θα φορτωθεί. |

### Τιμή Επιστροφής

Έργο με το καθορισμένο μοναδικό αναγνωριστικό από το καθορισμένο αρχείο πολλαπλών έργων. Null εάν το έργο δεν υπάρχει.

## Παραδείγματα

Δείχνει πώς να φορτώσετε ένα έργο από αρχείο Primavera XML όταν το uid του έργου είναι γνωστό.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

Δείχνει πώς να εξετάσετε τις πληροφορίες σύντομων έργων από ένα αρχείο Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Δείτε επίσης

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


