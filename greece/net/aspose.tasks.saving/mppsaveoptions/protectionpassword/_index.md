---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης που χρησιμοποιείται για την προστασία του τελικού αρχείου MPP. Αυτή τη στιγμή υποστηρίζεται για MS Project 2010 και νεότερες μορφές. Μια τιμή null υποδεικνύει ότι το αρχείο έργου δεν είναι προστατευμένο."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης που χρησιμοποιείται για την προστασία του τελικού αρχείου MPP. Προς το παρόν υποστηρίζεται για τα φορμά MS Project 2010 και νεότερα. Μια τιμή null υποδεικνύει ότι το αρχείο έργου δεν είναι προστατευμένο.

```csharp
public string ProtectionPassword { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο σε αρχείο MPP προστατευμένο με κωδικό πρόσβασης.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### Δείτε επίσης

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


