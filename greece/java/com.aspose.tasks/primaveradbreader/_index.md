---
title: "PrimaveraDbReader"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά έναν αναγνώστη για την ανάγνωση πληροφοριών έργου από τη βάση δεδομένων Primavera"
type: docs
weight: 200
url: /el/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Αναπαριστά έναν αναγνώστη για την ανάγνωση πληροφοριών έργου από τη βάση δεδομένων Primavera
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Ρυθμίσεις που καθορίζουν πώς να συνδεθείτε στη βάση δεδομένων Primavera. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectUid | int | Μοναδικό αναγνωριστικό του έργου για φόρτωση. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
