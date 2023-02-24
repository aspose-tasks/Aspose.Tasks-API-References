---
title: Recalculate
second_title: Aspose.Tasks για Αναφορά API .NET
description: Επαναπρογραμματίζει όλα τα αναγνωριστικά εργασιών του έργου τα επίπεδα περιγράμματος τις ημερομηνίες έναρξης/λήξης ορίζει ημερομηνίες πρώιμης/καθυστέρησης υπολογίζει τα πεδία slacks εργασίας και κόστους.
type: docs
weight: 1120
url: /el/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Επαναπρογραμματίζει όλα τα αναγνωριστικά εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει ημερομηνίες πρώιμης/καθυστέρησης, υπολογίζει τα πεδία slacks, εργασίας και κόστους.

```csharp
public void Recalculate()
```

### Δείτε επίσης

* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Επαναπρογραμματίζει όλα τα αναγνωριστικά εργασιών έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει ημερομηνίες πρώιμης/καθυστέρησης, υπολογίζει τα πεδία slacks, εργασίας και κόστους με προαιρετική επικύρωση.

```csharp
public void Recalculate(bool validate)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| validate | Boolean | Εάν είναι αληθές, θα εκτελεστεί η επικύρωση του εκ νέου υπολογισμού. Ποια δεδομένα επικυρώνονται: Προς το παρόν εφαρμόζεται μόνο η βασική επικύρωση των περιοχών ημερομηνιών σύνδεσης εργασιών. Τα εύρη ημερομηνιών της εργασίας (π.χ. ActualStart - ActualFinish, EarlyFinish, EarlyFinish, Ear. ) καθώς και οι ημερομηνίες των συνδέσμων εργασιών θα ελεγχθούν με βάση τα κριτήρια ημερομηνίας ότι η ημερομηνία έναρξης είναι μικρότερη ή ίση με την ημερομηνία λήξης. Εάν κάποια από τις συνθήκες που περιγράφονται παραπάνω αποτύχει, τότε[`RecalculationValidationException`](../../recalculationvalidationexception/)θα πεταχτεί. |

### Δείτε επίσης

* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->