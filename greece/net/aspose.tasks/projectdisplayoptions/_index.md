---
title: "Κλάση ProjectDisplayOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectDisplayOptions. Αντιπροσωπεύει τις επιλογές εμφάνισης για μια παρουσία έργου"
type: docs
weight: 1450
url: /el/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Αντιπροσωπεύει τις επιλογές εμφάνισης για μια παρουσία έργου.

```csharp
public class ProjectDisplayOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `ProjectDisplayOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει αν θα προστεθεί κενό πριν από την αριθμητική τιμή και τη συντομογραφία χρόνου (1 wk αντί για 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Αποκτά ή ορίζει πώς εμφανίζεται η ετικέτα ημέρας. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Αποκτά ή ορίζει πώς εμφανίζεται η ετικέτα ώρας. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Αποκτά ή ορίζει πώς εμφανίζεται η ετικέτα λεπτού. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Αποκτά ή ορίζει πώς εμφανίζεται η ετικέτα μήνα. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζεται συνοπτική πληροφορία για ολόκληρο το έργο σε μία γραμμή με τη δική του γραμμή περίληψης εργασίας στην κορυφή της προβολής Gantt Chart. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζονται προτάσεις όταν το Project εντοπίζει πιθανή σύγκρουση χρονοπρογραμματισμού με μια χειροκίνητα προγραμματισμένη εργασία. Αυτή η επιλογή είναι διαθέσιμη για την έκδοση Project 2010 και μεταγενέστερες. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται προειδοποιήσεις όταν το Project εντοπίζει πιθανή σύγκρουση χρονοπρογραμματισμού με μια χειροκίνητα προγραμματισμένη εργασία. Αυτή η επιλογή είναι διαθέσιμη για την έκδοση Project 2010 και μεταγενέστερες. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα υπογραμμίζονται οι υπερσυνδέσεις. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Λαμβάνει ή ορίζει πώς εμφανίζεται η ετικέτα εβδομάδας. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Λαμβάνει ή ορίζει πώς εμφανίζεται η ετικέτα έτους. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


