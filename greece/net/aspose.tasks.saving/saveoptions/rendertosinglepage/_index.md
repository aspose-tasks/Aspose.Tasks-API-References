---
title: "SaveOptions.RenderToSinglePage"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει ώστε το αποδοθέν έργο να χωράει σε μία σελίδα."
type: docs
weight: 150
url: /el/net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει ώστε το αποδοθέν έργο να χωράει σε μία σελίδα.

```csharp
public bool RenderToSinglePage { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε επιλεγμένες σελίδες ενός έργου σε αρχείο PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// ας ελέγξουμε τον αριθμό των σελίδων που μπορούν να εξαχθούν
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

Δείχνει πώς να χρησιμοποιήσετε την ιδιότητα RenderToSinglePage για να καθορίσετε ότι το έργο πρέπει να αποθηκευτεί σε PDF 1-σελίδας.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.TaskUsage;
options.Timescale = Timescale.DefinedInView;
options.RenderToSinglePage = true;
options.StartDate = new DateTime(2012, 12, 22);
options.EndDate = new DateTime(2013, 05, 10);

project.Save(OutDir + "WorkWithRenderToSinglePage_out.pdf", options);
```

Δείχνει πώς να αποθηκεύσετε τις επιλεγμένες σελίδες ως εικόνα.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

Δείχνει πώς να αποθηκεύσετε τη διάταξη σε ξεχωριστά αρχεία.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Αποθήκευση διάταξης έργου σε ξεχωριστά αρχεία
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


