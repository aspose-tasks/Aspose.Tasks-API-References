---
title: "RiskPattern"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει ένα πρότυπο κινδύνου για μια εργασία έργου."
type: docs
weight: 268
url: /el/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Αντιπροσωπεύει ένα πρότυπο κινδύνου για μια εργασία έργου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [RiskPattern](../../com.aspose.tasks/riskpattern). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Λαμβάνει το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων. |
| [getDistribution()](#getDistribution--) | Λαμβάνει την κατανομή πιθανοτήτων που χρησιμοποιείται στη προσομοίωση Monte Carlo. |
| [getOptimistic()](#getOptimistic--) | Λαμβάνει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου. |
| [getPessimistic()](#getPessimistic--) | Λαμβάνει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου. |
| [getTask()](#getTask--) | Λαμβάνει μια εργασία έργου στην οποία εφαρμόζεται αυτό το πρότυπο κινδύνου. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Ορίζει το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων. |
| [setDistribution(int value)](#setDistribution-int-) | Ορίζει την κατανομή πιθανότητας που χρησιμοποιείται στη προσομοίωση Monte Carlo. |
| [setOptimistic(int value)](#setOptimistic-int-) | Ορίζει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου. |
| [setPessimistic(int value)](#setPessimistic-int-) | Ορίζει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | η καθορισμένη εργασία έργου για την οποία θα εφαρμοστεί αυτός ο κίνδυνος στη προσομοίωση Monte Carlo. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Λαμβάνει το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων. Η προεπιλεγμένη τιμή είναι CL99.

--------------------

Μπορεί να είναι μία από τις τιμές που ορίζονται στην `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) απαρίθμηση.

**Returns:**
int - το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Λαμβάνει την κατανομή πιθανότητας που χρησιμοποιείται στη προσομοίωση Monte Carlo. Η προεπιλεγμένη τιμή είναι ProbabilityDistributionType.Normal.

--------------------

Μπορεί να είναι μία από τις τιμές που ορίζονται στην [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype) απαρίθμηση.

**Returns:**
int - η κατανομή πιθανότητας που χρησιμοποιείται στη προσομοίωση Monte Carlo.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Λαμβάνει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου. Η προεπιλεγμένη τιμή είναι 75, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η αισιόδοξη διάρκεια θα είναι 3 ημέρες.

**Returns:**
int - το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Λαμβάνει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου. Η προεπιλεγμένη τιμή είναι 125, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η απαισιόδοξη διάρκεια θα είναι 5 ημέρες.

**Returns:**
int - το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου.
### getTask() {#getTask--}
```
public final Task getTask()
```


Λαμβάνει μια εργασία έργου στην οποία εφαρμόζεται αυτό το πρότυπο κινδύνου.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Ορίζει το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων. Η προεπιλεγμένη τιμή είναι CL99.

--------------------

Μπορεί να είναι μία από τις τιμές που ορίζονται στην `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) απαρίθμηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές παραγόμενες τιμές θα βρίσκονται εντός των αισιόδοξων και απαισιόδοξων εκτιμήσεων. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Ορίζει την κατανομή πιθανότητας που χρησιμοποιείται στη προσομοίωση Monte Carlo. Η προεπιλεγμένη τιμή είναι ProbabilityDistributionType.Normal.

--------------------

Μπορεί να είναι μία από τις τιμές που ορίζονται στην [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype) απαρίθμηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η κατανομή πιθανότητας που χρησιμοποιείται στη προσομοίωση Monte Carlo. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Ορίζει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου. Η προεπιλεγμένη τιμή είναι 75, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η αισιόδοξη διάρκεια θα είναι 3 ημέρες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Ορίζει το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου. Η προεπιλεγμένη τιμή είναι 125, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η απαισιόδοξη διάρκεια θα είναι 5 ημέρες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου. |

