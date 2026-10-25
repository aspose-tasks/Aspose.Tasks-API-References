---
title: "LevelingOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό παραμέτρων εξισορρόπησης πόρων."
type: docs
weight: 142
url: /el/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Επιτρέπει τον καθορισμό παραμέτρων εξισορρόπησης πόρων.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Λαμβάνει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας εξισορρόπησης έργου. |
| [getFinishDate()](#getFinishDate--) | Λαμβάνει την ημερομηνία λήξης της περιόδου εξισορρόπησης. |
| [getLevelingOrder()](#getLevelingOrder--) | Λαμβάνει τη σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί εργασίες που έχουν υπερκατανομές. |
| [getMessageHandler()](#getMessageHandler--) | Λαμβάνει την κλήση επανάκλησης του διαχειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρέμβαση στα μηνύματα καταγραφής που παράγονται από το Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [getMessageLevel()](#getMessageLevel--) | Λαμβάνει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από το Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [getResources()](#getResources--) | Λαμβάνει τη λίστα των πόρων που θα εξισορροπηθούν. |
| [getStartDate()](#getStartDate--) | Λαμβάνει την ημερομηνία έναρξης της περιόδου εξισορρόπησης. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας εξισορρόπησης έργου. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Ορίζει την ημερομηνία λήξης της περιόδου εξισορρόπησης. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | Η σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί τις εργασίες που έχουν υπερκατανομές. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Ορίζει την κλήση επανάκλησης του χειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρεμβολή στα μηνύματα καταγραφής που παράγονται από Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Ορίζει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Ορίζει τη λίστα των πόρων που θα εξισορροπηθούν. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ορίζει την ημερομηνία έναρξης της περιόδου εξισορρόπησης. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Λαμβάνει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας εξισορρόπησης έργου.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Λαμβάνει την ημερομηνία λήξης της περιόδου εξισορρόπησης. Η προεπιλεγμένη τιμή είναι η ημερομηνία λήξης του έργου`s.

**Returns:**
java.util.Date - ημερομηνία λήξης περιόδου εξισορρόπησης.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Λαμβάνει τη σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί τις εργασίες που έχουν υπερκατανομές. Μετά τον προσδιορισμό των εργασιών που προκαλούν την υπερκατανομή και ποιες εργασίες μπορούν να καθυστερήσουν, χρησιμοποιείται η καθορισμένη σειρά για το ποια εργασία πρέπει να καθυστερήσει πρώτα.

**Returns:**
int - η σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί τις εργασίες που έχουν υπερκατανομές.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Λαμβάνει την κλήση επανάκλησης του διαχειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρέμβαση στα μηνύματα καταγραφής που παράγονται από το Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Λαμβάνει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από το Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων.

**Returns:**
int - επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Λαμβάνει τη λίστα των πόρων που θα εξισορροπηθούν. Εάν οριστεί null, όλοι οι πόροι του έργου θα εξισορροπηθούν.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - η λίστα των πόρων που θα εξισορροπηθούν.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Λαμβάνει την ημερομηνία έναρξης της περιόδου εξισορρόπησης. Η προεπιλεγμένη τιμή είναι η ημερομηνία έναρξης του έργου`s.

**Returns:**
java.util.Date - ημερομηνία έναρξης περιόδου εξισορρόπησης.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας εξισορρόπησης έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας εξισορρόπησης έργου. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Ορίζει την ημερομηνία λήξης της περιόδου εξισορρόπησης. Η προεπιλεγμένη τιμή είναι η ημερομηνία λήξης του έργου`s.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | ημερομηνία λήξης περιόδου εξισορρόπησης. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


Η σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί τις εργασίες που έχουν υπερκατανομές. Μετά τον προσδιορισμό των εργασιών που προκαλούν την υπερκατανομή και ποιες εργασίες μπορούν να καθυστερήσουν, χρησιμοποιείται η καθορισμένη σειρά για το ποια εργασία πρέπει να καθυστερήσει πρώτα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η σειρά με την οποία ο αλγόριθμος εξισορρόπησης καθυστερεί τις εργασίες που έχουν υπερκατανομές. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Ορίζει την κλήση επανάκλησης του χειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρεμβολή στα μηνύματα καταγραφής που παράγονται από Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | κλήση επανάκλησης του χειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρεμβολή στα μηνύματα καταγραφής που παράγονται από Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Ορίζει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από Aspose.Tasks κατά τη διάρκεια της εξισορρόπησης πόρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Ορίζει τη λίστα των πόρων που θα ισοσταθμιστούν. Εάν οριστεί null, όλοι οι πόροι του έργου θα ισοσταθμιστούν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;com.aspose.tasks.Resource&gt; | η λίστα των πόρων που θα ισοσταθμιστούν. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ορίζει την ημερομηνία έναρξης της περιόδου ισοστάθμισης. Η προεπιλεγμένη τιμή είναι η ημερομηνία έναρξης του έργου`s.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | ημερομηνία έναρξης περιόδου ισοστάθμισης. |

