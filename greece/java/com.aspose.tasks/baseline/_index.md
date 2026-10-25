---
title: "Βάση"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά τις τιμές βάσης ενός πόρου."
type: docs
weight: 26
url: /el/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Αναπαριστά τις τιμές βάσης ενός πόρου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Υλοποίηση διεπαφής IComparable. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getBaselineNumber()](#getBaselineNumber--) | Αποκτά τον μοναδικό αριθμό μιας εγγραφής δεδομένων baseline. |
| [getBcwp()](#getBcwp--) | Λαμβάνει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα. |
| [getBcws()](#getBcws--) | Λαμβάνει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |
| [getCost()](#getCost--) | Λαμβάνει το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline. |
| [getWork()](#getWork--) | Λαμβάνει την εργασία που έχει ανατεθεί σε έναν πόρο όταν αποθηκεύεται το baseline. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το baseline. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Ορίζει τον μοναδικό αριθμό μιας εγγραφής δεδομένων baseline. |
| [setBcwp(double value)](#setBcwp-double-) | Ορίζει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα. |
| [setBcws(double value)](#setBcws-double-) | Ορίζει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Ορίζει το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ορίζει την εργασία που έχει ανατεθεί σε έναν πόρο όταν αποθηκεύεται το baseline. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Υλοποίηση διεπαφής IComparable. Συγκρίνει αυτήν την περίπτωση με το καθορισμένο αντικείμενο Baseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | το καθορισμένο αντικείμενο Baseline για σύγκριση με αυτήν την περίπτωση. |

**Returns:**
int - επιστρέφει -1 εάν αυτή η περίπτωση είναι μικρότερη από το καθορισμένο αντικείμενο, 1 εάν αυτή η περίπτωση είναι μεγαλύτερη από το καθορισμένο αντικείμενο· διαφορετικά επιστρέφει 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | το καθορισμένο αντικείμενο για σύγκριση με αυτήν την περίπτωση. |

**Returns:**
boolean - επιστρέφει true εάν αυτή η περίπτωση είναι ίση με το καθορισμένο αντικείμενο· διαφορετικά, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | το καθορισμένο αντικείμενο για σύγκριση με αυτήν την περίπτωση. |

**Returns:**
boolean - επιστρέφει true εάν αυτή η περίπτωση είναι ίση με το καθορισμένο αντικείμενο· διαφορετικά, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Αποκτά τον μοναδικό αριθμό μιας εγγραφής δεδομένων baseline.

**Returns:**
int - ο μοναδικός αριθμός μιας εγγραφής δεδομένων baseline.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Λαμβάνει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα.

**Returns:**
double - το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Λαμβάνει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο.

**Returns:**
double - το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Λαμβάνει το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline.

**Returns:**
java.math.BigDecimal - το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Λαμβάνει την εργασία που έχει ανατεθεί σε έναν πόρο όταν αποθηκεύεται το baseline.

Τιμή: Το ποσό της ανατεθειμένης εργασίας σε έναν πόρο όταν αποθηκεύτηκε το baseline.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το baseline.

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Το πρώτο baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Το δεύτερο baseline. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Ορίζει τον μοναδικό αριθμό μιας εγγραφής δεδομένων baseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο μοναδικός αριθμός μιας εγγραφής δεδομένων baseline. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Ορίζει το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για ένα έργο μέχρι σήμερα. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Ορίζει το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | το προϋπολογισμένο κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Ορίζει το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | το προβλεπόμενο κόστος ενός πόρου όταν αποθηκεύεται το baseline. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ορίζει την εργασία που έχει ανατεθεί σε έναν πόρο όταν αποθηκεύεται το baseline.

Τιμή: Το ποσό της ανατεθειμένης εργασίας σε έναν πόρο όταν αποθηκεύτηκε το baseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | η εργασία που έχει ανατεθεί σε έναν πόρο όταν αποθηκεύεται το baseline. |

