---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskLink ιδιότητα. Λαμβάνει ή ορίζει τη διάρκεια καθυστέρησης ανάλογα με το LagFormat"
type: docs
weight: 50
url: /el/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Λαμβάνει ή ορίζει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Κατά την προσπάθεια ορισμού της τιμής για TaskLinks όπου το LagFormat είναι TimeUnitType.Percent. |

## Παρατηρήσεις

Η καθυστέρηση σύνδεσης μπορεί να είναι τιμή ποσοστού (LagFormat είναι TimeUnitType.Percent). Σε αυτήν την περίπτωση η διάρκεια υπολογίζεται ως ποσοστό της διάρκειας του PredTask. Διαφορετικά η μέθοδος επιστρέφει τιμή TimeSpan που αντιπροσωπεύει την καθυστέρηση του TaskLink.

### Δείτε επίσης

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


