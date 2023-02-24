---
title: WorkingTime
second_title: Aspose.Tasks για Αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουWorkingTimeaspose.tasks/workingtime/ τάξη με ένα διάστημα με τους καθορισμένους χρόνους έναρξης και λήξης.
type: docs
weight: 10
url: /el/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`WorkingTime`](../) τάξη με ένα διάστημα με τους καθορισμένους χρόνους έναρξης και λήξης.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromTime | DateTime | μεσοδιάστημα ώρα έναρξης |
| toTime | DateTime | χρόνος λήξης διαστήματος |

### Δείτε επίσης

* class [WorkingTime](../)
* χώρος ονομάτων [Aspose.Tasks](../../workingtime/)
* συνέλευση [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`WorkingTime`](../) τάξη με ένα στοιχείο διαστήματος με τους καθορισμένους χρόνους έναρξης και λήξης.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromTime | TimeSpan | Η ώρα έναρξης του διαστήματος αντιπροσωπεύεται απόTimeSpan struct. |
| toTime | TimeSpan | Η ώρα λήξης του διαστήματος αντιπροσωπεύεται απόTimeSpan struct. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | Όταν το toTime είναι μικρότερο από ίσο με το όρισμα χρόνου ή όταν το διάστημα μεταξύ fromTime και toTime είναι μεγαλύτερο από 24 ώρες. |

### Παραδείγματα

Η υπερφόρτωση του WorkingTime ctor μπορεί να χρησιμοποιηθεί για την προετοιμασία της έναρξης και του τερματισμού του διαστήματος χρησιμοποιώντας TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Δείτε επίσης

* class [WorkingTime](../)
* χώρος ονομάτων [Aspose.Tasks](../../workingtime/)
* συνέλευση [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`WorkingTime`](../) τάξη με ένα στοιχείο διαστήματος με τους καθορισμένους χρόνους έναρξης και λήξης.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromHours | Int32 | Η ώρα έναρξης του διαστήματος αντιπροσωπεύεται από ακέραιο αριθμό ωρών (0-24). |
| toHours | Int32 | Η ώρα λήξης του διαστήματος αντιπροσωπεύεται από ακέραιο αριθμό ωρών (0-24). |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | Όταν το toTime είναι μικρότερο από ίσο με το όρισμα χρόνου ή όταν το διάστημα μεταξύ fromTime και toTime είναι μεγαλύτερο από 24 ώρες. |

### Παραδείγματα

Η υπερφόρτωση του WorkTime ctor μπορεί να χρησιμοποιηθεί για να αρχικοποιήσει την έναρξη και το τέλος του διαστήματος χρησιμοποιώντας ολόκληρες ώρες:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### Δείτε επίσης

* class [WorkingTime](../)
* χώρος ονομάτων [Aspose.Tasks](../../workingtime/)
* συνέλευση [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->