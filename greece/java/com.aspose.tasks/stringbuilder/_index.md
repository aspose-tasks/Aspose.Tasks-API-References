---
title: "StringBuilder"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια μεταβλητή συμβολοσειρά χαρακτήρων."
type: docs
weight: 281
url: /el/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Αντιπροσωπεύει μια μεταβλητή συμβολοσειρά χαρακτήρων. Δεν μπορεί να επεκταθεί.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας την καθορισμένη χωρητικότητα. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder που ξεκινά με καθορισμένη χωρητικότητα και μπορεί να μεγαλώσει μέχρι ένα καθορισμένο μέγιστο. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας τη καθορισμένη συμβολοσειρά. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας τη καθορισμένη συμβολοσειρά και τη χωρητικότητα. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder από το καθορισμένο υποσύνολο χαρακτήρων και τη χωρητικότητα. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Προσθέτει την αναπαράσταση συμβολοσειράς μιας καθορισμένης λογικής τιμής σε αυτό το αντικείμενο. |
| [append(byte value)](#append-byte-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου byte σε αυτό το αντικείμενο. |
| [append(char value)](#append-char-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου χαρακτήρα Unicode σε αυτό το αντικείμενο. |
| [append(char value, int repeatCount)](#append-char-int-) | Προσθέτει έναν καθορισμένο αριθμό αντιγράφων της αναπαράστασης συμβολοσειράς ενός χαρακτήρα Unicode σε αυτό το αντικείμενο. |
| [append(char[] value)](#append-char---) | Προσθέτει την αναπαράσταση συμβολοσειράς των χαρακτήρων Unicode σε έναν καθορισμένο πίνακα σε αυτό το αντικείμενο. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου υποπίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο. |
| [append(double value)](#append-double-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού double σε αυτό το αντικείμενο. |
| [append(float value)](#append-float-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού float σε αυτό το αντικείμενο. |
| [append(int value)](#append-int-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού int σε αυτό το αντικείμενο. |
| [append(Object value)](#append-java.lang.Object-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αντικειμένου σε αυτό το αντικείμενο. |
| [append(String value)](#append-java.lang.String-) | Προσθέτει ένα αντίγραφο της καθορισμένης συμβολοσειράς σε αυτό το αντικείμενο. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Προσθέτει ένα αντίγραφο ενός καθορισμένου υποσυμβολοσειράς σε αυτό το αντικείμενο. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού BigDecimal σε αυτό το αντικείμενο. |
| [append(long value)](#append-long-) | Προσθέτει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου μεγάλου αριθμού σε αυτό το αντικείμενο. |
| [append(short value)](#append-short-) | Προσθέτει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου μικρού αριθμού σε αυτό το αντικείμενο. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Προσθέτει τη συμβολοσειρά που επιστρέφεται από την επεξεργασία μιας σύνθετης συμβολοσειράς μορφοποίησης, η οποία περιέχει μηδέν ή περισσότερα στοιχεία μορφοποίησης, σε αυτό το αντικείμενο. |
| [appendLine()](#appendLine--) | Προσθέτει το προεπιλεγμένο διαχωριστικό γραμμής στο τέλος του τρέχοντος αντικειμένου StringBuilder. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Προσθέτει ένα αντίγραφο της καθορισμένης συμβολοσειράς, ακολουθούμενο από το προεπιλεγμένο διαχωριστικό γραμμής, στο τέλος του τρέχοντος αντικειμένου StringBuilder. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Αντιγράφει τους χαρακτήρες από ένα καθορισμένο τμήμα αυτού του αντικειμένου σε ένα καθορισμένο τμήμα ενός πίνακα Char προορισμού. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Εξασφαλίζει ότι η χωρητικότητα αυτού του αντικειμένου StringBuilder είναι τουλάχιστον η καθορισμένη τιμή. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getCapacity()](#getCapacity--) | Λαμβάνει τον μέγιστο αριθμό χαρακτήρων που μπορούν να περιληφθούν στη μνήμη που έχει εκχωρηθεί από το τρέχον αντικείμενο. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος του τρέχοντος αντικειμένου StringBuilder. |
| [getMaxCapacity()](#getMaxCapacity--) | Λαμβάνει τη μέγιστη χωρητικότητα αυτού του αντικειμένου. |
| [hashCode()](#hashCode--) | Επιστρέφει έναν κωδικό κατακερματισμού για αυτό το StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Εισάγει την αναπαράσταση σε συμβολοσειρά μιας λογικής τιμής σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, byte value)](#insert-int-byte-) | Εισάγει την αναπαράσταση σε συμβολοσειρά μιας τιμής byte σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, char value)](#insert-int-char-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου χαρακτήρα Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, char[] value)](#insert-int-char---) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου πίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου υποπίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, double value)](#insert-int-double-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού double σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, float value)](#insert-int-float-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού float σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, int value)](#insert-int-int-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού int σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αντικειμένου σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Εισάγει μια συμβολοσειρά σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Εισάγει ένα ή περισσότερα αντίγραφα μιας καθορισμένης συμβολοσειράς σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός δεκαδικού αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, long value)](#insert-int-long-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός μεγάλου αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [insert(int index, short value)](#insert-int-short-) | Εισάγει την αναπαράσταση σε συμβολοσειρά ενός μικρού αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα. |
| [remove(int startIndex, int length)](#remove-int-int-) | Αφαιρεί το καθορισμένο εύρος χαρακτήρων από αυτό το παράδειγμα. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα σε αυτό το παράδειγμα με έναν άλλο καθορισμένο χαρακτήρα. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Αντικαθιστά, εντός μιας υποσυμβολοσειράς αυτού του παραδείγματος, όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα με έναν άλλο καθορισμένο χαρακτήρα. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς σε αυτό το παράδειγμα με μια άλλη καθορισμένη συμβολοσειρά. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Αντικαθιστά, εντός μιας υποσυμβολοσειράς αυτού του παραδείγματος, όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς με μια άλλη καθορισμένη συμβολοσειρά. |
| [setCapacity(int value)](#setCapacity-int-) | Ορίζει τον μέγιστο αριθμό χαρακτήρων που μπορούν να περιληφθούν στη μνήμη που έχει εκχωρηθεί από το τρέχον παράδειγμα. |
| [setLength(int value)](#setLength-int-) | Ορίζει το μήκος του τρέχοντος αντικειμένου StringBuilder. |
| [toString()](#toString--) | Μετατρέπει την τιμή αυτού του παραδείγματος σε String. |
| [toString(int startIndex, int length)](#toString-int-int-) | Μετατρέπει την τιμή μιας υποσυμβολοσειράς αυτού του παραδείγματος σε String. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας την καθορισμένη χωρητικότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| capacity | int | Το προτεινόμενο αρχικό μέγεθος αυτού του παραδείγματος. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder που ξεκινά με καθορισμένη χωρητικότητα και μπορεί να μεγαλώσει μέχρι ένα καθορισμένο μέγιστο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| capacity | int | Το προτεινόμενο αρχικό μέγεθος του StringBuilder. |
| maxCapacity | int | Ο μέγιστος αριθμός χαρακτήρων που μπορεί να περιέχει η τρέχουσα συμβολοσειρά. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας τη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά που χρησιμοποιείται για την αρχικοποίηση της τιμής του παραδείγματος. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder χρησιμοποιώντας τη καθορισμένη συμβολοσειρά και τη χωρητικότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά που χρησιμοποιείται για την αρχικοποίηση της τιμής του παραδείγματος. |
| capacity | int | Το προτεινόμενο αρχικό μέγεθος του StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης StringBuilder από το καθορισμένο υποσύνολο χαρακτήρων και τη χωρητικότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά που περιέχει την υποσυμβολοσειρά που χρησιμοποιείται για την αρχικοποίηση της τιμής αυτού του παραδείγματος. |
| startIndex | int | Η θέση εντός της τιμής όπου αρχίζει η υποσυμβολοσειρά. |
| length | int | Ο αριθμός των χαρακτήρων στην υποσυμβολοσειρά. |
| capacity | int | Το προτεινόμενο αρχικό μέγεθος του StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς μιας καθορισμένης λογικής τιμής σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | Η λογική τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου byte σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | byte | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου χαρακτήρα Unicode σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char | Ο χαρακτήρας Unicode που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Προσθέτει έναν καθορισμένο αριθμό αντιγράφων της αναπαράστασης συμβολοσειράς ενός χαρακτήρα Unicode σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char | Ο χαρακτήρας προς προσθήκη. |
| repeatCount | int | Ο αριθμός των φορών που θα προστεθεί η τιμή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς των χαρακτήρων Unicode σε έναν καθορισμένο πίνακα σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char[] | Ο πίνακας χαρακτήρων προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου υποπίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char[] | Ένας πίνακας χαρακτήρων. |
| startIndex | int | Η αρχική θέση στην τιμή. |
| charCount | int | Ο αριθμός των χαρακτήρων προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού double σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού float σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού int σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αντικειμένου σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Object | Το αντικείμενο προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Προσθέτει ένα αντίγραφο της καθορισμένης συμβολοσειράς σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Προσθέτει ένα αντίγραφο ενός καθορισμένου υποσυμβολοσειράς σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά που περιέχει τη δευτερεύουσα συμβολοσειρά προς προσθήκη. |
| startIndex | int | Η αρχική θέση της δευτερεύουσας συμβολοσειράς μέσα στην τιμή. |
| count | int | Ο αριθμός των χαρακτήρων στην τιμή προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Προσθέτει την αναπαράσταση συμβολοσειράς ενός καθορισμένου αριθμού BigDecimal σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Προσθέτει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου μεγάλου αριθμού σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | long | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Προσθέτει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου μικρού αριθμού σε αυτό το αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | short | Η τιμή που θα προσαρτηθεί. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Προσθέτει τη συμβολοσειρά που επιστρέφεται μετά την επεξεργασία μιας σύνθετης συμβολοσειράς μορφοποίησης, η οποία περιέχει μηδέν ή περισσότερα στοιχεία μορφοποίησης, σε αυτήν την παρουσία. Κάθε στοιχείο μορφοποίησης αντικαθίσταται από την αναπαράσταση σε συμβολοσειρά ενός αντίστοιχου ορίσματος σε έναν πίνακα παραμέτρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| format | java.lang.String | Μια σύνθετη συμβολοσειρά μορφοποίησης. |
| args | java.lang.Object[] | Ένας πίνακας αντικειμένων για μορφοποίηση. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Προσθέτει το προεπιλεγμένο διαχωριστικό γραμμής στο τέλος του τρέχοντος αντικειμένου StringBuilder.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Προσθέτει ένα αντίγραφο της καθορισμένης συμβολοσειράς, ακολουθούμενο από το προεπιλεγμένο διαχωριστικό γραμμής, στο τέλος του τρέχοντος αντικειμένου StringBuilder.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η συμβολοσειρά προς προσθήκη. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Αντιγράφει τους χαρακτήρες από ένα καθορισμένο τμήμα αυτού του αντικειμένου σε ένα καθορισμένο τμήμα ενός πίνακα Char προορισμού.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceIndex | int | Η αρχική θέση σε αυτήν την παρουσία από την οποία θα αντιγραφούν οι χαρακτήρες. Ο δείκτης είναι μηδενικής βάσης. |
| προορισμός | char[] | Ο πίνακας όπου θα αντιγραφούν οι χαρακτήρες. |
| destinationIndex | int | Η αρχική θέση στον προορισμό όπου θα αντιγραφούν οι χαρακτήρες. Ο δείκτης είναι μηδενικής βάσης. |
| count | int | Ο αριθμός των χαρακτήρων που θα αντιγραφούν. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Εξασφαλίζει ότι η χωρητικότητα αυτού του αντικειμένου StringBuilder είναι τουλάχιστον η καθορισμένη τιμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| capacity | int | Η ελάχιστη χωρητικότητα που πρέπει να διασφαλιστεί. |

**Returns:**
int - Η νέα χωρητικότητα της συγκεκριμένης παρουσίας.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Ένα αντικείμενο για σύγκριση με αυτήν την παρουσία, ή null. |

**Returns:**
boolean - true εάν αυτή η παρουσία και το sb έχουν ίσες τιμές string, Capacity και MaxCapacity· διαφορετικά, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Λαμβάνει τον μέγιστο αριθμό χαρακτήρων που μπορούν να περιληφθούν στη μνήμη που έχει εκχωρηθεί από το τρέχον αντικείμενο.

**Returns:**
int - Ο μέγιστος αριθμός χαρακτήρων που μπορεί να περιέχεται στη μνήμη που έχει εκχωρηθεί από την τρέχουσα παρουσία.
### getLength() {#getLength--}
```
public int getLength()
```


Λαμβάνει το μήκος του τρέχοντος αντικειμένου StringBuilder.

**Returns:**
int - Το μήκος της συγκεκριμένης παρουσίας.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Λαμβάνει τη μέγιστη χωρητικότητα αυτού του αντικειμένου.

**Returns:**
int - Ο μέγιστος αριθμός χαρακτήρων που μπορεί να κρατήσει αυτή η παρουσία.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει έναν κωδικό κατακερματισμού για αυτό το StringBuilder.

**Returns:**
int - Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά μιας λογικής τιμής σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | boolean | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά μιας τιμής byte σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | byte | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου χαρακτήρα Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | char | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου πίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | char[] | Ο πίνακας χαρακτήρων προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός καθορισμένου υποπίνακα χαρακτήρων Unicode σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | char[] | Ένας πίνακας χαρακτήρων. |
| startIndex | int | Ο αρχικός δείκτης εντός της τιμής. |
| charCount | int | Ο αριθμός των χαρακτήρων προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού double σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | double | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού float σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | float | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αριθμού int σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | int | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός αντικειμένου σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | java.lang.Object | Το αντικείμενο προς εισαγωγή, ή null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Εισάγει μια συμβολοσειρά σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | java.lang.String | Το string προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Εισάγει ένα ή περισσότερα αντίγραφα μιας καθορισμένης συμβολοσειράς σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | java.lang.String | Το string προς εισαγωγή. |
| count | int | Ο αριθμός των φορών για εισαγωγή της τιμής. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός δεκαδικού αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | java.math.BigDecimal | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός μεγάλου αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | long | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Εισάγει την αναπαράσταση σε συμβολοσειρά ενός μικρού αριθμού σε αυτό το αντικείμενο στη καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Η θέση σε αυτήν την παρουσία όπου αρχίζει η εισαγωγή. |
| τιμή | short | Η τιμή προς εισαγωγή. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Αφαιρεί το καθορισμένο εύρος χαρακτήρων από αυτό το παράδειγμα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Η θέση μηδενικής βάσης σε αυτήν την παρουσία όπου αρχίζει η αφαίρεση. |
| length | int | Ο αριθμός των χαρακτήρων προς αφαίρεση. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα σε αυτό το παράδειγμα με έναν άλλο καθορισμένο χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChar | char | Ο χαρακτήρας προς αντικατάσταση. |
| newChar | char | Ο χαρακτήρας που αντικαθιστά το oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Αντικαθιστά, εντός μιας υποσυμβολοσειράς αυτού του παραδείγματος, όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα με έναν άλλο καθορισμένο χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | char | Ο χαρακτήρας προς αντικατάσταση. |
| newValue | char | Ο χαρακτήρας που αντικαθιστά το oldChar. |
| startIndex | int | Η θέση σε αυτήν την περίπτωση όπου αρχίζει η υποσυμβολοσειρά. |
| count | int | Το μήκος της υποσυμβολοσειράς. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς σε αυτό το παράδειγμα με μια άλλη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | java.lang.String | Η συμβολοσειρά προς αντικατάσταση. |
| newValue | java.lang.String | Η συμβολοσειρά που αντικαθιστά το oldValue, ή null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Αντικαθιστά, εντός μιας υποσυμβολοσειράς αυτού του παραδείγματος, όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς με μια άλλη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | java.lang.String | Η συμβολοσειρά προς αντικατάσταση. |
| newValue | java.lang.String | Η συμβολοσειρά που αντικαθιστά το oldValue, ή null. |
| startIndex | int | Η θέση σε αυτήν την περίπτωση όπου αρχίζει η υποσυμβολοσειρά. |
| count | int | Το μήκος της υποσυμβολοσειράς. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Ορίζει τον μέγιστο αριθμό χαρακτήρων που μπορούν να περιληφθούν στη μνήμη που έχει εκχωρηθεί από το τρέχον παράδειγμα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Ο μέγιστος αριθμός χαρακτήρων που μπορεί να περιέχεται στη μνήμη που έχει δεσμευτεί από την τρέχουσα περίπτωση. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Ορίζει το μήκος του τρέχοντος αντικειμένου StringBuilder.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Το μήκος αυτής της περίπτωσης. |

### toString() {#toString--}
```
public String toString()
```


Μετατρέπει την τιμή αυτού του παραδείγματος σε String.

**Returns:**
java.lang.String - Μια συμβολοσειρά της οποίας η τιμή είναι η ίδια με αυτήν την περίπτωση.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Μετατρέπει την τιμή μιας υποσυμβολοσειράς αυτού του παραδείγματος σε String.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Η αρχική θέση της υποσυμβολοσειράς σε αυτήν την περίπτωση. |
| length | int | Το μήκος της υποσυμβολοσειράς. |

**Returns:**
java.lang.String - Μια συμβολοσειρά της οποίας η τιμή είναι η ίδια με την καθορισμένη υποσυμβολοσειρά αυτής της περίπτωσης.
