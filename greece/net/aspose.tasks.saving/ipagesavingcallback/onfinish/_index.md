---
title: "IPageSavingCallback.OnFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος IPageSavingCallback. Η μέθοδος που θα κληθεί όταν όλες οι σελίδες έχουν γραφτεί"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Μέθοδος που θα κληθεί όταν όλες οι σελίδες έχουν γραφτεί.

```csharp
public void OnFinish()
```

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

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


