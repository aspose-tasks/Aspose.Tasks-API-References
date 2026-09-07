---
title: "SaveTemplateOptions.RemoveBaselineValues"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveTemplateOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι τιμές βάσης από ένα πρότυπο έργου πρέπει να αφαιρεθούν"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/savetemplateoptions/removebaselinevalues/
---
## SaveTemplateOptions.RemoveBaselineValues property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι βασικές τιμές από ένα πρότυπο έργου πρέπει να αφαιρεθούν.

```csharp
public bool RemoveBaselineValues { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως πρότυπο χρησιμοποιώντας επιλογές.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// δημιουργήστε επιλογές αποθήκευσης προτύπου
// και ρυθμίστε τις ιδιότητές του
var options = new SaveTemplateOptions
{
    // ορίστε μια τιμή που υποδεικνύει εάν όλα τα σταθερά κόστη από ένα πρότυπο έργου πρέπει να αφαιρεθούν
    RemoveFixedCosts = true,

    // ορίστε μια τιμή που υποδεικνύει εάν όλες οι πραγματικές τιμές από ένα πρότυπο έργου πρέπει να αφαιρεθούν
    RemoveActualValues = true,

    // ορίστε μια τιμή που υποδεικνύει εάν οι τιμές πόρων από ένα πρότυπο έργου πρέπει να αφαιρεθούν
    RemoveResourceRates = true,

    // ορίστε μια τιμή που υποδεικνύει εάν όλες οι βασικές τιμές από ένα πρότυπο έργου πρέπει να αφαιρεθούν
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Δείτε επίσης

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


