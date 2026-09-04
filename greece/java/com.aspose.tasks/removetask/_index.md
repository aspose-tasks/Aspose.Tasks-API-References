---
title: "RemoveTask"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αφαιρεί την καθορισμένη εργασία από ένα δέντρο εργασιών."
type: docs
weight: 246
url: /el/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Αφαιρεί την καθορισμένη εργασία από ένα δέντρο εργασιών.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [RemoveTask](../../com.aspose.tasks/removetask). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Μην κάνετε τίποτα. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Μην κάνετε τίποτα. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Αφαιρεί τη εργασία από την καθορισμένη γονική εργασία. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [RemoveTask](../../com.aspose.tasks/removetask).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Εργασία προς αφαίρεση. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Μην κάνετε τίποτα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Αντικείμενο προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Μην κάνετε τίποτα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Αντικείμενο προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Αφαιρεί τη εργασία από την καθορισμένη γονική εργασία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Γονική εργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

