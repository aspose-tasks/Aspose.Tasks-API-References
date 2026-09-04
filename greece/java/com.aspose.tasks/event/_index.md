---
title: "Συμβάν"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Ένα συμβάν."
type: docs
weight: 374
url: /el/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Ένα συμβάν.

`TArgs`: επιχειρήματα συμβάντος.

TArgs :
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Αυτή η μέθοδος καλείται όταν το συμβάν εκδίδεται. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Αυτή η μέθοδος καλείται όταν το συμβάν εκδίδεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αποστολέας | java.lang.Object | ένα αντικείμενο που ξεκινά αυτό το συμβάν. |
| args | TArgs | προσαρμοσμένα επιχειρήματα. |

