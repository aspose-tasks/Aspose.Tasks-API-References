---
title: Add
second_title: Aspose.Tasks για Αναφορά API .NET
description: Προσθέστε την καθορισμένη εργασία στην παρουσία τουTaskCollectionaspose.tasks/taskcollection/class. Εάν το ParentProject.CalculationMode είναι None ο χρήστης θα πρέπει να καλέσει το Project.Recalculate μετά τη χρήση αυτής της μεθόδου Θα επαναπρογραμματίσει όλες τις εργασίες του έργου ημερομηνίες έναρξης/ολοκλήρωσης ορίζει πρώιμες/καθυστερημένες ημερομηνίες και θα υπολογίσει τα εξαρτημένα πεδία όπως slacks work και πεδία κόστους αναγνωριστικά και επίπεδα διάρθρωσης. Εάν το ParentProject.CalculationMode είναι Manual η μέθοδος θα υπολογίζει αυτόματα μόνο το αναγνωριστικό εργασίας το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος. Εάν το ParentProject.CalculationMode είναι Automatic η μέθοδος επαναπρογραμματίζει όλες τις εργασίες του έργου αυτόματα st ημερομηνίες ορίζει πρώιμες/καθυστερημένες ημερομηνίες υπολογίζει τα πεδία slacks εργασίας και κόστους υπολογίζει εκ νέου τα αναγνωριστικά και τα επίπεδα περιγράμματος.
type: docs
weight: 50
url: /el/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Προσθέστε την καθορισμένη εργασία στην παρουσία του[`TaskCollection`](../)class. Εάν το ParentProject.CalculationMode είναι None, ο χρήστης θα πρέπει να καλέσει το Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/ολοκλήρωσης, ορίζει πρώιμες/καθυστερημένες ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως slacks, work και πεδία κόστους, αναγνωριστικά και επίπεδα διάρθρωσης). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίζει αυτόματα μόνο το αναγνωριστικό εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει όλες τις εργασίες του έργου αυτόματα st ημερομηνίες, ορίζει πρώιμες/καθυστερημένες ημερομηνίες, υπολογίζει τα πεδία slacks, εργασίας και κόστους, υπολογίζει εκ νέου τα αναγνωριστικά και τα επίπεδα περιγράμματος).

```csharp
public void Add(Task item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | Task | την καθορισμένη εργασία που πρέπει να προστεθεί σε αυτήν τη συλλογή εργασιών. |

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* χώρος ονομάτων [Aspose.Tasks](../../taskcollection/)
* συνέλευση [Aspose.Tasks](../../../)

---

## Add() {#add}

Προσθέτει νέα εργασία στη συλλογή εργασιών έργου στο ίδιο επίπεδο περιγράμματος με την τελευταία εργασία.

```csharp
public Task Add()
```

### Επιστρεφόμενη Αξία

επιστρέφει το στιγμιότυπο του που προστέθηκε πρόσφατα[`Task`](../../task/) τάξη.

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* χώρος ονομάτων [Aspose.Tasks](../../taskcollection/)
* συνέλευση [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Προσθέτει μια νέα εργασία στη συλλογή εργασιών για παιδιά.

```csharp
public Task Add(string taskName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | String | το καθορισμένο όνομα εργασίας. |

### Επιστρεφόμενη Αξία

επιστρέφει το στιγμιότυπο του που προστέθηκε πρόσφατα[`Task`](../../task/) τάξη.

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* χώρος ονομάτων [Aspose.Tasks](../../taskcollection/)
* συνέλευση [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή παιδικών εργασιών.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | String | το καθορισμένο όνομα εργασίας. |
| beforeTaskId | Int32 | Το καθορισμένο αναγνωριστικό μιας εργασίας πριν από την οποία θα εισαχθεί μια νέα εργασία. |

### Επιστρεφόμενη Αξία

επιστρέφει μια εργασία που είχε εισαχθεί πριν από μια εργασία με το καθορισμένο αναγνωριστικό.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | Το ArgumentOutOfRangeException εμφανίζεται εάν το καθορισμένο αναγνωριστικό δεν είναι έγκυρο αναγνωριστικό εργασίας. |

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* χώρος ονομάτων [Aspose.Tasks](../../taskcollection/)
* συνέλευση [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο αναγνωριστικό και στο ίδιο επίπεδο περιγράμματος.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Οι παράμετροι τις καθορισμένες παραμέτρους για τη δημιουργία επαναλαμβανόμενης εργασίας. |

### Επιστρεφόμενη Αξία

επιστρέφει το στιγμιότυπο του που προστέθηκε πρόσφατα[`Task`](../../task/) τάξη.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | Πετάγεται εάν οι καθορισμένες παράμετροι είναι μηδενικές. |
| ArgumentException | Απορρίπτεται εάν οι καθορισμένες παράμετροι δεν είναι έγκυρες. |

### Δείτε επίσης

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* χώρος ονομάτων [Aspose.Tasks](../../taskcollection/)
* συνέλευση [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
