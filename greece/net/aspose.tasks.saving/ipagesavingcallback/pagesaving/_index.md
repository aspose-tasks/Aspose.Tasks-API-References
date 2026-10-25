---
title: "IPageSavingCallback.PageSaving"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος IPageSavingCallback. Η μέθοδος που θα κληθεί όταν μια σελίδα αποθηκευτεί σε ροή"
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

Η μέθοδος που θα κληθεί όταν μια σελίδα αποθηκευτεί σε ροή.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| args | PageSavingArgs | Τα επιχειρήματα αποθήκευσης σελίδας. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο πολλαπλών σελίδων σε ροές που παρέχονται από τον χρήστη χρησιμοποιώντας την κλήση επιστροφής αποθήκευσης σελίδας.

```csharp
[Test] 
public void UsePageSavingCallbackToSavePageToSeparateStreams()
{
    var project = new Project(DataDir + "Homemoveplan.mpp");

    var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png);

    var callback = new CustomPageSavingCallback();
    imageSaveOptions.PageSavingCallback = callback;
    imageSaveOptions.RenderToSinglePage = false;
    project.Save(Stream.Null, imageSaveOptions);

    foreach (var streams in callback.PageStreams)
    {
        // επεξεργαστείτε κάθε ροή σελίδας
    }
}

private sealed class CustomPageSavingCallback : IPageSavingCallback
{
    public List<MemoryStream> PageStreams { get; } = new List<MemoryStream>();

    public void PageSaving(PageSavingArgs args)
    {
        var memoryStream = new MemoryStream();
        args.Stream = memoryStream;
        args.KeepStreamOpen = false;
        this.PageStreams.Add(memoryStream);
    }

    public void OnFinish()
    {
    }
}
```

### Δείτε επίσης

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


