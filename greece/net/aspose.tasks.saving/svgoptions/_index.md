---
title: "Κλάση SvgOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.SvgOptions κλάση. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε SVG"
type: docs
weight: 2230
url: /el/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε SVG.

```csharp
public class SvgOptions : SaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SvgOptions](svgoptions/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `SvgOptions` που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή SVG. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Λαμβάνει ή ορίζει τη λίστα των στιγμιοτύπων της κλάσης [`BarStyle`](../../aspose.tasks.visualization/barstyle/) που εμφανίζονται στην προβολή του έργου. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Αποκτά ή ορίζει το προσαρμοσμένο μέγεθος σελίδας σε points (1 point = 1/72 ίντσας). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (Η προεπιλεγμένη τιμή είναι TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Αποκτά ή ορίζει μια ημερομηνία για την ολοκλήρωση της απόδοσης. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Αποκτά ή ορίζει μια λίστα των [`Gridline`](../../aspose.tasks.visualization/gridline/) που εμφανίζονται στην προβολή του έργου. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι τοπίο. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Αποκτά ή ορίζει μια τιμή που καθορίζει πώς θα αποδοθεί ένα υπόμνημα. Η προεπιλεγμένη τιμή είναι LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Αποκτά ή ορίζει έναν πίνακα των PageLegendItem που καθορίζουν ποιες μπάρες πρέπει να αποδοθούν στο υπόμνημα της σελίδας. Εάν είναι null, αποδίδονται τα προεπιλεγμένα στοιχεία. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Αποκτά ή ορίζει το χρώμα του μη εργάσιμου χρόνου. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Αποκτά ή ορίζει τον αριθμό των σελίδων του έργου. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | Λαμβάνει ή ορίζει μια callback υλοποίησης ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση μιας ροής εξόδου για κάθε αποδομένη σελίδα. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Αποκτά ή ορίζει το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Αποκτά ή ορίζει το [`PresentationFormat`](../saveoptions/presentationformat/) με το οποίο θα αποθηκευτεί το έγγραφο. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει ώστε το αποδοθέν έργο να χωράει σε μία σελίδα. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν οι υποεργασίες στη μπάρα της συνολικής εργασίας πρέπει να σημειωθούν. Για τις υποεργασίες, το πεδίο Rollup υποδεικνύει εάν οι πληροφορίες στις μπαρ Gantt των υποεργασιών θα ενσωματωθούν στη μπάρα της συνολικής εργασίας. Για τις συνολικές εργασίες, το πεδίο Rollup υποδεικνύει εάν η μπάρα της συνολικής εργασίας εμφανίζει ενσωματωμένες μπαρ. Πρέπει να έχετε το πεδίο Rollup για τις συνολικές εργασίες ορισμένο σε Yes ώστε οποιεσδήποτε υποεργασίες να ενσωματωθούν σε αυτές. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία από την οποία θα ξεκινήσει η απόδοση. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Λαμβάνει ή ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης συνδέσμων εργασιών. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Λαμβάνει ή ορίζει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Λαμβάνει ή ορίζει την τιμή του [`Timescale`](../saveoptions/timescale/) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Λαμβάνει ή ορίζει μια συμπεριφορά που καθορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το τέλος της σελίδας. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής που θα αποδοθούν ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Εάν δεν οριστεί, τότε αποδίδονται μόνο τα IDs εργασιών, τα ονόματα εργασιών, η έναρξη και η λήξη. Εάν τόσο η ιδιότητα View όσο και οι ιδιότητες του [`ViewSettings`](../saveoptions/viewsettings/) οριστούν, οι στήλες από το View υπερισχύουν των στηλών από το ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Λαμβάνει ή ορίζει μια προβολή ([`View`](../saveoptions/view/)) για απόδοση. Μπορείτε να χρησιμοποιήσετε αυτήν την επιλογή για να καθορίσετε ρητά ποια προβολή πρέπει να αποθηκευτεί σε μορφές PDF, HTML ή Image. Εάν αυτή η ιδιότητα οριστεί, η ιδιότητα [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) αγνοείται όταν το έργο αποθηκεύεται. Η προβολή πρέπει να προέρχεται από μία από τις παρακάτω οθόνες (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως αρχείο SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο
                            PresentationFormat = PresentationFormat.GanttChart,

                            // ορίστε μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της
                            FitContent = true,

                            // ορίστε την ελάχιστη χρονική περίοδο για απόδοση. Η προεπιλεγμένη τιμή είναι <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου
                            // Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Δείτε επίσης

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


