---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Vertegenwoordigt het activiteit-id-veld, een unieke identifier van een taak die door Primavera wordt gebruikt. Alleen van toepassing op Primavera-projecten"
type: docs
weight: 10
url: /nl/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Vertegenwoordigt het activity-id-veld - een unieke identifier van een taak die door Primavera wordt gebruikt. (alleen van toepassing op Primavera-projecten).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Voorbeelden

Toont hoe te werken met het ActivityId-veld specifiek voor Primavera-projecten

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Maak Primavera-opslagopties aan en specificeer dat ActivityIds niet mogen worden overschreven tijdens het opslaan.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


