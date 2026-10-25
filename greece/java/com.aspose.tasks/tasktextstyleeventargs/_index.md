---
title: "TaskTextStyleEventArgs"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την απόδοση του περιεχομένου των κελιών του πίνακα."
type: docs
weight: 302
url: /el/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την απόδοση του περιεχομένου των κελιών του πίνακα.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Λαμβάνει το TextStyle που θα χρησιμοποιηθεί για τη σχεδίαση του περιεχομένου του κελιού. |
| [getColumn()](#getColumn--) | Λαμβάνει το [ViewColumn](../../com.aspose.tasks/viewcolumn) στο οποίο ανήκει το τρέχον εμφανιζόμενο κελί. |
| [getTask()](#getTask--) | Λαμβάνει `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) που αντιστοιχεί στη τρέχουσα εμφανιζόμενη σειρά. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Ορίζει το TextStyle που θα χρησιμοποιηθεί για τη σχεδίαση του περιεχομένου του κελιού. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Λαμβάνει το TextStyle που θα χρησιμοποιηθεί για τη σχεδίαση του περιεχομένου του κελιού. Αυτό το αντικείμενο μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης ενός κελιού πίνακα.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Λαμβάνει το [ViewColumn](../../com.aspose.tasks/viewcolumn) στο οποίο ανήκει το τρέχον εμφανιζόμενο κελί.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Λαμβάνει `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) που αντιστοιχεί στη τρέχουσα εμφανιζόμενη σειρά.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Ορίζει το TextStyle που θα χρησιμοποιηθεί για τη σχεδίαση του περιεχομένου του κελιού. Αυτό το αντικείμενο μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης ενός κελιού πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle που θα χρησιμοποιηθεί για τη σχεδίαση του περιεχομένου του κελιού. |

