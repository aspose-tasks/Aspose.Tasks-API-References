---
title: "Τιμή"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά τον ορισμό μιας χρονικής περιόδου και των τιμών που ισχύουν για έναν πόρο κατά τη διάρκεια αυτής της περιόδου."
type: docs
weight: 232
url: /el/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Αναπαριστά τον ορισμό μιας χρονικής περιόδου και των τιμών που ισχύουν για έναν πόρο κατά τη διάρκεια αυτής της περιόδου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Λαμβάνει το κόστος ανά χρήση ενός πόρου. |
| [getOvertimeRate()](#getOvertimeRate--) | Λαμβάνει το ωριαίο ποσοστό υπερωρίας για έναν πόρο. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Λαμβάνει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας. |
| [getRateTable()](#getRateTable--) | Λαμβάνει το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο. |
| [getRatesFrom()](#getRatesFrom--) | Λαμβάνει την ημερομηνία που η τιμή τίθεται σε ισχύ. |
| [getRatesTo()](#getRatesTo--) | Λαμβάνει την τελευταία ημερομηνία που η τιμή είναι σε ισχύ. |
| [getStandardRate()](#getStandardRate--) | Λαμβάνει το τυπικό ωριαίο ποσοστό για έναν πόρο. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Λαμβάνει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Ορίζει το κόστος ανά χρήση ενός πόρου. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Ορίζει το ωριαίο ποσοστό υπερωρίας για έναν πόρο. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας. |
| [setRateTable(int value)](#setRateTable-int-) | Ορίζει το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Ορίζει την ημερομηνία κατά την οποία η τιμή τίθεται σε ισχύ. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Ορίζει την τελευταία ημερομηνία κατά την οποία η τιμή είναι σε ισχύ. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Ορίζει το τυπικό ωριαίο ποσοστό για έναν πόρο. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Λαμβάνει το κόστος ανά χρήση ενός πόρου. Αυτή η τιμή ανακτάται από την τρέχουσα ημερομηνία εάν υπάρχει πίνακας τιμών για έναν πόρο.

**Returns:**
java.math.BigDecimal - το κόστος ανά χρήση ενός πόρου.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Λαμβάνει το ωριαίο ποσοστό υπερωρίας για έναν πόρο.

**Returns:**
java.math.BigDecimal - το ωριαίο ποσοστό υπερωρίας για έναν πόρο.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Λαμβάνει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας.

**Returns:**
int - οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Λαμβάνει το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο.

**Returns:**
int - το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Λαμβάνει την ημερομηνία που η τιμή τίθεται σε ισχύ.

**Returns:**
java.util.Date - η ημερομηνία κατά την οποία η τιμή τίθεται σε ισχύ.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Λαμβάνει την τελευταία ημερομηνία που η τιμή είναι σε ισχύ.

**Returns:**
java.util.Date - η τελευταία ημερομηνία κατά την οποία η τιμή είναι σε ισχύ.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Λαμβάνει το τυπικό ωριαίο ποσοστό για έναν πόρο.

**Returns:**
java.math.BigDecimal - το τυπικό ωριαίο ποσοστό για έναν πόρο.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Λαμβάνει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού.

**Returns:**
int - οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Ορίζει το κόστος ανά χρήση ενός πόρου. Αυτή η τιμή ανακτάται από την τρέχουσα ημερομηνία εάν υπάρχει πίνακας τιμών για έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | το κόστος ανά χρήση ενός πόρου. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Ορίζει το ωριαίο ποσοστό υπερωρίας για έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | το ωριαίο ποσοστό υπερωρίας για έναν πόρο. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Ορίζει το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Ορίζει την ημερομηνία κατά την οποία η τιμή τίθεται σε ισχύ.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία κατά την οποία η τιμή τίθεται σε ισχύ. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Ορίζει την τελευταία ημερομηνία κατά την οποία η τιμή είναι σε ισχύ.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η τελευταία ημερομηνία κατά την οποία η τιμή είναι σε ισχύ. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Ορίζει το τυπικό ωριαίο ποσοστό για έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | το τυπικό ωριαίο ποσοστό για έναν πόρο. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ρυθμού. |

