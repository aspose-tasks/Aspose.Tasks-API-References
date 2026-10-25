---
title: "MspDbSettings"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον ορισμό των απαραίτητων επιλογών για την ανάγνωση δεδομένων έργου από τη βάση δεδομένων του MS Project Server."
type: docs
weight: 161
url: /el/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Επιτρέπει τον ορισμό των απαραίτητων επιλογών για την ανάγνωση δεδομένων έργου από τη βάση δεδομένων του MS Project Server.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Λαμβάνει το guid του έργου για ανάγνωση. |
| [getSchema()](#getSchema--) | Λαμβάνει το σχήμα του MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Ορίζει το σχήμα του MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connectionString | java.lang.String | η καθορισμένη συμβολοσειρά σύνδεσης. |
| projectGuid | java.util.UUID | το καθορισμένο guid ενός έργου για ανάγνωση. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Λαμβάνει το guid του έργου για ανάγνωση.

**Returns:**
java.util.UUID - το guid του έργου για ανάγνωση.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Λαμβάνει το σχήμα του MS Project Server. Η προεπιλεγμένη τιμή είναι "pub".

**Returns:**
java.lang.String - το σχήμα του MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Ορίζει το σχήμα του MS Project Server. Η προεπιλεγμένη τιμή είναι "pub".

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το σχήμα του MS Project Server. |

