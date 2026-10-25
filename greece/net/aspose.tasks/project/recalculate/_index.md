---
title: "Project.Recalculate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επαναπρογραμματίζει όλα τα IDs εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις πρώιμες/αργίες ημερομηνίες, υπολογίζει τα περιθώρια, την εργασία και τα πεδία κόστους."
type: docs
weight: 1150
url: /el/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Αναπρογραμματίζει όλα τα IDs εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις έγκαιρες/αργές ημερομηνίες, υπολογίζει τα περιθώρια, την εργασία και τα πεδία κόστους.

```csharp
public void Recalculate()
```

## Παραδείγματα

Δείχνει πώς να επαναπρογραμματίσετε το έργο από την ημερομηνία έναρξης αντί για την ημερομηνία λήξης.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Τώρα όλες οι ημερομηνίες των εργασιών (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) υπολογίζονται. Για να λάβουμε τη κρίσιμη διαδρομή πρέπει να υπολογίσουμε τα περιθώρια (μπορούν να κληθούν σε ξεχωριστό νήμα, αλλά μόνο μετά τον υπολογισμό όλων των πρώιμων/τελευταίων ημερομηνιών).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Αναπρογραμματίζει όλα τα IDs εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις έγκαιρες/αργές ημερομηνίες, υπολογίζει τα περιθώρια, την εργασία και τα πεδία κόστους με προαιρετική επικύρωση.

```csharp
public void Recalculate(bool validate)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| validate | Boolean | Εάν είναι true, θα εκτελεστεί η επικύρωση της επανυπολογισμού. Ποια δεδομένα επικυρώνονται: Προς το παρόν έχει υλοποιηθεί μόνο η βασική επικύρωση των εύρους ημερομηνιών εργασίας και συνδέσμου εργασίας. Τα εύρη ημερομηνιών της εργασίας (π.χ. ActualStart - ActualFinish, EarlyStart - EarlyFinish κ.λπ.) καθώς και οι ημερομηνίες των Συνδέσμων Εργασίας θα ελεγχθούν σύμφωνα με το κριτήριο ότι η ημερομηνία έναρξης είναι μικρότερη ή ίση με την ημερομηνία λήξης. Εάν οποιαδήποτε από τις παραπάνω συνθήκες αποτύχει, τότε θα εξαχθεί το [`RecalculationValidationException`](../../recalculationvalidationexception/). |

## Παραδείγματα

Δείχνει πώς να επανυπολογίσετε το έργο με μετα-επικύρωση.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // επαναυπολογίστε το έργο με μετα-επικύρωση
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


