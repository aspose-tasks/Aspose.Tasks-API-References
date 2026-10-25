---
title: "ProjectDisplayOptions.DayLabel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectDisplayOptions ιδιότητα. Λαμβάνει ή ορίζει πώς εμφανίζεται η ετικέτα ημέρας"
type: docs
weight: 30
url: /el/net/aspose.tasks/projectdisplayoptions/daylabel/
---
## ProjectDisplayOptions.DayLabel property

Αποκτά ή ορίζει πώς εμφανίζεται η ετικέτα ημέρας.

```csharp
public DayLabelDisplay DayLabel { get; set; }
```

## Παραδείγματα

Εμφανίζει πώς να χρησιμοποιήσετε τις επιλογές εμφάνισης του έργου.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται προειδοποιήσεις όταν το Project εντοπίζει πιθανή σύγκρουση χρονοπρογραμματισμού με μια χειροκίνητα προγραμματισμένη εργασία.
// Αυτή η επιλογή είναι διαθέσιμη για την έκδοση Project 2010 και μεταγενέστερες.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// μια τιμή που υποδεικνύει εάν θα προστεθεί κενό πριν από την αριθμητική τιμή και τη συντομογραφία χρόνου (1 wk αντί για 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// ορίστε πώς εμφανίζεται η ετικέτα λεπτών
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// ορίστε πώς εμφανίζεται η ετικέτα ώρας
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// ορίστε πώς εμφανίζεται η ετικέτα ημέρας
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// ορίστε πώς εμφανίζεται η ετικέτα εβδομάδας
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// ορίστε πώς εμφανίζεται η ετικέτα του μήνα
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// ορίστε πώς εμφανίζεται η ετικέτα έτους
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζεται συνοπτική πληροφορία για ολόκληρο το έργο σε μία γραμμή με τη δική της γραμμή σύνοψης εργασιών στην κορυφή της προβολής Gantt Chart.
project.DisplayOptions.ShowProjectSummaryTask = true;

// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται προτάσεις όταν το Project εντοπίζει πιθανή σύγκρουση χρονοπρογραμματισμού με μια χειροκίνητα προγραμματισμένη εργασία.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// ορίστε μια τιμή που υποδεικνύει εάν θα υπογραμμίζονται οι υπερσυνδέσεις.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* enum [DayLabelDisplay](../../daylabeldisplay/)
* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


