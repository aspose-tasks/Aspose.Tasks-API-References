---
title: "Class SaveTemplateOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.SaveTemplateOptions class. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση ενός έργου ως πρότυπο"
type: docs
weight: 2200
url: /el/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση ενός έργου ως πρότυπο.

```csharp
public class SaveTemplateOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι πραγματικές τιμές από ένα πρότυπο έργου πρέπει να αφαιρεθούν. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι βασικές τιμές από ένα πρότυπο έργου πρέπει να αφαιρεθούν. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλα τα σταθερά κόστη από ένα πρότυπο έργου πρέπει να αφαιρεθούν. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι τιμές πόρων από ένα πρότυπο έργου πρέπει να αφαιρεθούν. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


