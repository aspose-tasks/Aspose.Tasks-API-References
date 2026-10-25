---
title: "Απαρίθμηση ConstraintType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η απαρίθμηση Aspose.Tasks.ConstraintType. Καθορίζει τον περιορισμό στην ημερομηνία έναρξης ή λήξης μιας εργασίας"
type: docs
weight: 330
url: /el/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Καθορίζει τον περιορισμό στην ημερομηνία έναρξης ή λήξης μιας εργασίας.

```csharp
public enum ConstraintType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
| AsSoonAsPossible | `0` | Οι ημερομηνίες [`Start`](../tsk/start/) και [`Finish`](../tsk/finish/) του [`Task`](../task/) προγραμματίζονται το συντομότερο δυνατό σε σχέση με τις γονικές ημερομηνίες [`Start`](../tsk/start/) και [`Finish`](../tsk/finish/) και λαμβάνοντας υπόψη τα [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) και [`Finish`](../tsk/finish/) ημερομηνίες του [`Task`](../task/) προγραμματίζονται ALAP σε σχέση με τις γονικές [`Start`](../tsk/start/) και [`Finish`](../tsk/finish/) ημερομηνίες και λαμβάνοντας υπόψη τα [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Πρέπει να ξεκινήσει στις |
| MustFinishOn | `3` | Πρέπει να ολοκληρωθεί στις |
| StartNoEarlierThan | `4` | Έναρξη όχι νωρίτερα από |
| StartNoLaterThan | `5` | Έναρξη όχι αργότερα από |
| FinishNoEarlierThan | `6` | Ολοκλήρωση όχι νωρίτερα από |
| FinishNoLaterThan | `7` | Ολοκλήρωση όχι αργότερα από |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να ορίσετε τον περιορισμό &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible για μια εργασία.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Ορίστε τον περιορισμό As Soon As Possible για εργασία με Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


