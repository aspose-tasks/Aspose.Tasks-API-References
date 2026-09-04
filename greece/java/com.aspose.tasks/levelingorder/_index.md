---
title: "LevelingOrder"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Ορίζει τις πιθανές τιμές της σειράς εξισορρόπησης."
type: docs
weight: 143
url: /el/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Ορίζει τις πιθανές τιμές της σειράς εξισορρόπησης.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [IdOnly](#IdOnly) | Οι εργασίες καθυστερούν με αύξουσα σειρά Id. |
| [PriorityThenStandard](#PriorityThenStandard) | Η προτεραιότητα λαμβάνεται υπόψη πρώτα, έπειτα οι ίδιες ιδιότητες όπως στο Standard. |
| [Standard](#Standard) | Λαμβάνονται υπόψη οι ακόλουθες ιδιότητες: σχέσεις προγόνων, συνολικό περιθώριο (μια εργασία με μεγαλύτερο συνολικό περιθώριο καθυστερεί πρώτη), ημερομηνία έναρξης, προτεραιότητα. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Οι εργασίες καθυστερούν με αύξουσα σειρά Id.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


Η προτεραιότητα λαμβάνεται υπόψη πρώτα, έπειτα οι ίδιες ιδιότητες όπως στο Standard.

### Standard {#Standard}
```
public static final int Standard
```


Λαμβάνονται υπόψη οι ακόλουθες ιδιότητες: σχέσεις προγόνων, συνολικό περιθώριο (μια εργασία με μεγαλύτερο συνολικό περιθώριο καθυστερεί πρώτη), ημερομηνία έναρξης, προτεραιότητα. Αυτή είναι η προεπιλεγμένη τιμή.

