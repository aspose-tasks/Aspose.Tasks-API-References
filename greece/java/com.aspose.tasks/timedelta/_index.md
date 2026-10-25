---
title: "TimeDelta"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά τη διαφορά μεταξύ δύο χρονικών σημείων."
type: docs
weight: 317
url: /el/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Αναπαριστά τη διαφορά μεταξύ δύο χρονικών σημείων.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Αρχικοποιεί μια νέα παρουσία του TimeDelta στον καθορισμένο αριθμό ωρών, λεπτών και δευτερολέπτων. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Αρχικοποιεί μια νέα παρουσία του TimeDelta στον καθορισμένο αριθμό ημερών, ωρών, λεπτών, δευτερολέπτων και χιλιοστών του δευτερολέπτου. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Επιστρέφει ένα νέο αντικείμενο TimeDelta του οποίου η τιμή είναι το άθροισμα αυτής και της άλλης παρουσίας. |
| [clone()](#clone--) | \\{@inheritDoc\\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Συγκρίνει δύο τιμές TimeDelta και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η πρώτη τιμή είναι μικρότερη, ίση ή μεγαλύτερη από τη δεύτερη τιμή. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Συγκρίνει αυτή την παρουσία με ένα καθορισμένο αντικείμενο TimeDelta και επιστρέφει έναν ακέραιο που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη, ίση ή μεγαλύτερη από το αντικείμενο TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Δηλώνει εάν κάποιο `other` διάστημα χρόνου είναι ίσο με αυτό. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Ελέγχει δύο στιγμιότυπα για ισότητα. |
| [equals(Object other)](#equals-java.lang.Object-) | \\{@inheritDoc\\} |
| [fromDays(double value)](#fromDays-double-) | Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό ημερών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου). |
| [fromHours(double value)](#fromHours-double-) | Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό ωρών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό χιλιοστών του δευτερολέπτου (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου). |
| [fromMinutes(double value)](#fromMinutes-double-) | Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό λεπτών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου). |
| [fromSeconds(double value)](#fromSeconds-double-) | Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό δευτερολέπτων (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου). |
| [getDays()](#getDays--) | Επιστρέφει το στοιχείο ημερών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο. |
| [getHours()](#getHours--) | Επιστρέφει το στοιχείο ωρών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο. |
| [getMilliseconds()](#getMilliseconds--) | Επιστρέφει το στοιχείο χιλιοστών του δευτερολέπτου του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο. |
| [getMinutes()](#getMinutes--) | Επιστρέφει το στοιχείο λεπτών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο. |
| [getSeconds()](#getSeconds--) | Επιστρέφει το στοιχείο δευτερολέπτων του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο. |
| [getTotalDays()](#getTotalDays--) | Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές ημέρες. |
| [getTotalHours()](#getTotalHours--) | Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές ώρες. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές χιλιοστά του δευτερολέπτου. |
| [getTotalMinutes()](#getTotalMinutes--) | Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρα και κλασματικά λεπτά. |
| [getTotalSeconds()](#getTotalSeconds--) | Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρα και κλασματικά δευτερόλεπτα. |
| [hashCode()](#hashCode--) | \\{@inheritDoc\\} |
| [negate()](#negate--) | Επιστρέφει ένα νέο `TimeDelta` του οποίου η τιμή είναι η αρνητική τιμή αυτού του στιγμιότυπου. |
| [parse(String s)](#parse-java.lang.String-) | Μετατρέπει την αναπαράσταση συμβολοσειράς ενός χρονικού διαστήματος στην ισοδύναμη `TimeDelta` του. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Επιστρέφει ένα νέο αντικείμενο TimeDelta του οποίου η τιμή είναι η διαφορά μεταξύ αυτού και των στιγμιότυπων `other`. |
| [toString()](#toString--) | \\{@inheritDoc\\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Μετατρέπει την αναπαράσταση συμβολοσειράς ενός χρονικού διαστήματος στην ισοδύναμη TimeDelta και επιστρέφει μια τιμή που υποδεικνύει αν η μετατροπή πέτυχε. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Αρχικοποιεί μια νέα παρουσία του TimeDelta στον καθορισμένο αριθμό ωρών, λεπτών και δευτερολέπτων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ώρες | int | αριθμός ωρών. |
| λεπτά | int | αριθμός λεπτών. |
| δευτερόλεπτα | int | αριθμός δευτερολέπτων. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Αρχικοποιεί μια νέα παρουσία του TimeDelta στον καθορισμένο αριθμό ημερών, ωρών, λεπτών, δευτερολέπτων και χιλιοστών του δευτερολέπτου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημέρες | int | αριθμός ημερών. |
| ώρες | int | αριθμός ωρών. |
| λεπτά | int | αριθμός λεπτών. |
| δευτερόλεπτα | int | αριθμός δευτερολέπτων. |
| χιλιοστά του δευτερολέπτου | int | αριθμός χιλιοστών του δευτερολέπτου. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Επιστρέφει ένα νέο αντικείμενο TimeDelta του οποίου η τιμή είναι το άθροισμα αυτής και της άλλης παρουσίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | το αντικείμενο για άθροιση. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


Συγκρίνει δύο τιμές TimeDelta και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η πρώτη τιμή είναι μικρότερη, ίση ή μεγαλύτερη από τη δεύτερη τιμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | το πρώτο χρονικό διάστημα για σύγκριση. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | το δεύτερο χρονικό διάστημα για σύγκριση. |

**Returns:**
int - \-1 αν το `t1` είναι μικρότερο από το `t2`, 0 αν το `t1` είναι ίσο με το `t2` και 1 αν το `t1` είναι μεγαλύτερο από το `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Συγκρίνει αυτή την παρουσία με ένα καθορισμένο αντικείμενο TimeDelta και επιστρέφει έναν ακέραιο που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη, ίση ή μεγαλύτερη από το αντικείμενο TimeSpan.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | ένα αντικείμενο για σύγκριση. |

**Returns:**
int - \-1 αν αυτό το αντικείμενο είναι μικρότερο από το `other`, 0 αν αυτό το αντικείμενο είναι ίσο με το `other` και 1 αν αυτό το αντικείμενο είναι μεγαλύτερο από το `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Δηλώνει εάν κάποιο `other` διάστημα χρόνου είναι ίσο με αυτό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | χρονικό διάστημα για σύγκριση. |

**Returns:**
boolean - `true` αν τα διαστήματα είναι ίσα· `false` διαφορετικά.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Ελέγχει δύο στιγμιότυπα για ισότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | πρώτο αντικείμενο. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | δεύτερο αντικείμενο. |

**Returns:**
boolean - `true` αν τα αντικείμενα είναι ίσα· `false` διαφορετικά.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό ημερών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | αριθμός ημερών. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό ωρών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | αριθμός ωρών. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό χιλιοστών του δευτερολέπτου (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | αριθμός χιλιοστών του δευτερολέπτου. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό λεπτών (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | αριθμός λεπτών. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Επιστρέφει ένα TimeDelta που αντιπροσωπεύει έναν καθορισμένο αριθμό δευτερολέπτων (στρογγυλοποιημένο στο πλησιέστερο χιλιοστό του δευτερολέπτου).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | αριθμός δευτερολέπτων. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Επιστρέφει το στοιχείο ημερών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο.

**Returns:**
int - το στοιχείο ημερών του χρονικού διαστήματος. Μπορεί να είναι θετικό ή αρνητικό.
### getHours() {#getHours--}
```
public int getHours()
```


Επιστρέφει το στοιχείο ωρών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο.

**Returns:**
int - το στοιχείο ωρών του χρονικού διαστήματος στο εύρος από -23 έως 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Επιστρέφει το στοιχείο χιλιοστών του δευτερολέπτου του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο.

**Returns:**
int - το στοιχείο χιλιοστών του δευτερολέπτου του χρονικού διαστήματος στο εύρος από -999 έως 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Επιστρέφει το στοιχείο λεπτών του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο.

**Returns:**
int - το στοιχείο λεπτών του χρονικού διαστήματος στο εύρος από -59 έως 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Επιστρέφει το στοιχείο δευτερολέπτων του χρονικού διαστήματος, που αντιπροσωπεύεται από αυτό το στιγμιότυπο.

**Returns:**
int - το στοιχείο δευτερολέπτων του χρονικού διαστήματος στο εύρος από -59 έως 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές ημέρες.

**Returns:**
double - ο συνολικός αριθμός ημερών που αντιπροσωπεύει αυτή η παρουσία.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές ώρες.

**Returns:**
double - ο συνολικός αριθμός ωρών που αντιπροσωπεύει αυτή η παρουσία.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρες και κλασματικές χιλιοστά του δευτερολέπτου.

**Returns:**
double - ο συνολικός αριθμός χιλιοστών του δευτερολέπτου που αντιπροσωπεύει αυτή η παρουσία.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρα και κλασματικά λεπτά.

**Returns:**
double - ο συνολικός αριθμός λεπτών που αντιπροσωπεύει αυτή η παρουσία.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Επιστρέφει την τιμή του τρέχοντος στιγμιότυπου εκφρασμένη σε ολόκληρα και κλασματικά δευτερόλεπτα.

**Returns:**
double - ο συνολικός αριθμός δευτερολέπτων που αντιπροσωπεύει αυτή η παρουσία.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Επιστρέφει ένα νέο `TimeDelta` του οποίου η τιμή είναι η αρνητική τιμή αυτού του στιγμιότυπου.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Μετατρέπει την αναπαράσταση συμβολοσειράς ενός χρονικού διαστήματος στην ισοδύναμη `TimeDelta` του.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| s | java.lang.String | μια συμβολοσειρά που καθορίζει το χρονικό διάστημα προς μετατροπή. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Επιστρέφει ένα νέο αντικείμενο TimeDelta του οποίου η τιμή είναι η διαφορά μεταξύ αυτού και των στιγμιότυπων `other`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | η παρουσία προς αφαίρεση. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Μετατρέπει την αναπαράσταση συμβολοσειράς ενός χρονικού διαστήματος στην ισοδύναμη TimeDelta και επιστρέφει μια τιμή που υποδεικνύει αν η μετατροπή πέτυχε.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| s | java.lang.String | μια συμβολοσειρά που καθορίζει το χρονικό διάστημα προς μετατροπή. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | Αυτός ο πίνακας πρέπει να έχει τουλάχιστον ένα στοιχείο. Όταν αυτή η μέθοδος επιστρέψει, `result[0]` περιέχει ένα αντικείμενο που αντιπροσωπεύει το χρονικό διάστημα που καθορίζεται από το `s`, ή ένα χρονικό διάστημα μηδενικού μήκους εάν η μετατροπή απέτυχε. |

**Returns:**
boolean - `true` εάν το s μετατράπηκε επιτυχώς· διαφορετικά, `false`.
