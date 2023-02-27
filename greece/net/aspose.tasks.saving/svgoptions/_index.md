---
title: SvgOptions
second_title: Aspose.Tasks για Αναφορά API .NET
description: Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων έργου σε SVG.
type: docs
weight: 1950
url: /el/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων έργου σε SVG.

```csharp
public class SvgOptions : SaveOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [SvgOptions](svgoptions/)() | Αρχικοποιεί μια νέα παρουσία του`SvgOptions` κλάση που μπορεί να χρησιμοποιηθεί για την αποθήκευση έργου σε μορφή SVG. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Λαμβάνει ή ορίζει τη λίστα των παρουσιών του[`BarStyle`](../../aspose.tasks.visualization/barstyle/) κλάση που εμφανίζεται στην προβολή έργου. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Λαμβάνει ή ορίζει το προσαρμοσμένο μέγεθος σελίδας σε πόντους (1 σημείο = 1/72 της ίντσας). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν πρέπει να τραβηχτεί ο μη εργάσιμος χρόνος (Η προεπιλεγμένη τιμή είναι TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Λαμβάνει ή ορίζει μια ημερομηνία για να ολοκληρωθεί η απόδοση. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ύψος της σειράς πρέπει να αυξηθεί για να ταιριάζει στο περιεχόμενό της. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Λαμβάνει ή ορίζει εάν μια ενότητα ημερολογίου μιας προβολής θα πρέπει να αποδίδεται στο τέλος (δεξιά πλευρά) της τελευταίας σελίδας. Εάν η τιμή είναι ψευδής, η ενότητα ημερολογίου αποδίδεται ακριβώς στην Ημερομηνία λήξης, ακόμη και εάν υπάρχει κενός χώρος σε μια σελίδα. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα με[`Gridline`](../../aspose.tasks.visualization/gridline/) που εμφανίζονται στην προβολή έργου. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το υπόμνημα πρέπει να εμφανίζεται σε κάθε σελίδα (Η προεπιλεγμένη τιμή είναι TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του χρόνου που δεν λειτουργεί. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων του έργου. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | Λαμβάνει ή ορίζει μια επιστροφή κλήσης υλοποίησης που ορίζεται από το χρήστη, η οποία χρησιμοποιείται για τη λήψη μιας ροής εξόδου για κάθε σελίδα που αποδίδεται. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Λαμβάνει ή ορίζει το[`PresentationFormat`](../saveoptions/presentationformat/) στο οποίο θα αποθηκευτεί το έγγραφο. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει, ώστε το έργο που αποδίδεται να μπορεί να χωρέσει σε μία σελίδα. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι δευτερεύουσες εργασίες στη γραμμή εργασιών σύνοψης πρέπει να επισημαίνονται. Για δευτερεύουσες εργασίες, το πεδίο Συνάθροιση υποδεικνύει εάν οι πληροφορίες για τις γραμμές Gantt δευτερευουσών εργασιών θα ενσωματωθούν στη γραμμή εργασιών σύνοψης. Για εργασίες σύνοψης, η Σύναψη Το πεδίο υποδεικνύει εάν η γραμμή εργασιών σύνοψης εμφανίζει τυλιγμένες ράβδους. Πρέπει να έχετε το πεδίο Συνάθροιση για εργασίες σύνοψης που έχει οριστεί σε Ναι για τυχόν δευτερεύουσες εργασίες να συγκεντρωθούν σε αυτές. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιείται αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία από την οποία ξεκινά η απόδοση. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ρυθμίζει το εργαλείο σύγκρισης για ταξινόμηση εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα εργασιών που αποδίδονται σε γραφήματα Gantt, Task Sheet και Task Usage. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Λαμβάνει ή ορίζει τη λίστα των παρουσιών του[`TextStyle`](../../aspose.tasks.visualization/textstyle/) κλάση που εμφανίζεται στην προβολή έργου. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Λαμβάνει ή ορίζει το[`Timescale`](../saveoptions/timescale/) τιμή που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | Καθορίζει εάν θα χρησιμοποιηθεί ντεγκραντέ πινέλο κατά την απόδοση της διάταξης του έργου. Επί του παρόντος, η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα με τις στήλες προβολής προς απόδοση ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Εάν δεν έχει οριστεί, τότε τα αναγνωριστικά εργασιών, τα ονόματα εργασιών, η αρχή και το τέλος αποδίδονται μόνο. Εάν και οι δύο Προβολή και[`ViewSettings`](../saveoptions/viewsettings/)οι ιδιότητες έχουν οριστεί, οι στήλες από την Προβολή αντικαθιστούν τις στήλες από τις Ρυθμίσεις Προβολής. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Λαμβάνει ή ορίζει μια προβολή ([`View`](../saveoptions/view/) ) καθιστώ. Μπορείτε να χρησιμοποιήσετε αυτές τις επιλογές για να καθορίσετε ρητά ποια προβολή θα αποθηκευτεί σε μορφές PDF, HTML ή Εικόνας. Εάν έχει οριστεί αυτή η ιδιότητα,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) Η ιδιότητα αγνοείται όταν αποθηκεύεται το έργο. Η προβολή πρέπει να προέρχεται από μία από τις ακόλουθες οθόνες (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, Task Sheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Δείτε επίσης

* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* συνέλευση [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
