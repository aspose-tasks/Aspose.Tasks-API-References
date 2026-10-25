---
title: "PrimaveraBaseReader"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά έναν βασικό αναγνώστη που μπορεί να χρησιμοποιηθεί για την ανάγνωση των UID έργου από αρχεία Primavera XER ή XML πολλαπλών έργων."
type: docs
weight: 196
url: /el/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Αναπαριστά έναν βασικό αναγνώστη που μπορεί να χρησιμοποιηθεί για την ανάγνωση των UID έργου από αρχεία Primavera XER ή XML πολλαπλών έργων.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Επιστρέφει μια λίστα των σύντομων αντικειμένων πληροφοριών του έργου. |
| [getProjectUids()](#getProjectUids--) | Επιστρέφει μια λίστα των μοναδικών αναγνωριστικών των έργων. |
| [loadProject(int projectUid)](#loadProject-int-) | Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Επιστρέφει μια λίστα των σύντομων αντικειμένων πληροφοριών του έργου.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - μια λίστα των σύντομων αντικειμένων πληροφοριών του έργου
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Επιστρέφει μια λίστα των μοναδικών αναγνωριστικών των έργων.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Λίστα των μοναδικών αναγνωριστικών των έργων.
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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
