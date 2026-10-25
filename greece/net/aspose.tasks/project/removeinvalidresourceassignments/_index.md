---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Απομακρύνει τις μη έγκυρες εκχωρήσεις πόρων από τη λίστα εκχωρήσεων πόρων του έργου."
type: docs
weight: 1170
url: /el/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Καταργεί τις μη έγκυρες εκχωρήσεις πόρων από τη λίστα εκχωρήσεων πόρων του έργου.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Παρατηρήσεις

Το MS Project δημιουργεί μια κενή εκχώρηση πόρου για κάθε εργασία. Καλέστε τη μέθοδο για να τις αφαιρέσετε.

## Παραδείγματα

Δείχνει πώς να αφαιρέσετε τις μη έγκυρες εκχωρήσεις.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// αφαιρέστε τις μη έγκυρες εκχωρήσεις
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


