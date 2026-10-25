---
title: "Διεπαφή IPageSavingCallback"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.IPageSavingCallback διεπαφή. Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν κάθε σελίδα σε έγγραφο πολλαπλών σελίδων αποθηκεύεται σε ξεχωριστό stream."
type: docs
weight: 2020
url: /el/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν κάθε σελίδα σε έγγραφο πολλαπλών σελίδων αποθηκεύεται σε ξεχωριστό ρεύμα.

```csharp
public interface IPageSavingCallback
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Μέθοδος που θα κληθεί όταν όλες οι σελίδες έχουν γραφτεί. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | Η μέθοδος που θα κληθεί όταν μια σελίδα αποθηκευτεί σε ροή. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


