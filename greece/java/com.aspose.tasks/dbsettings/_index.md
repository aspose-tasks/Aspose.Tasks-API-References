---
title: "DbSettings"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό ρυθμίσεων για ανάγνωση από τη βάση δεδομένων του έργου."
type: docs
weight: 75
url: /el/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Επιτρέπει τον καθορισμό ρυθμίσεων για ανάγνωση από τη βάση δεδομένων του έργου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Λαμβάνει τη συμβολοσειρά σύνδεσης. |
| [getDriverClassName()](#getDriverClassName--) | Επιστρέφει ένα όνομα κλάσης οδηγού JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Ορίζει τη συμβολοσειρά σύνδεσης. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Ορίζει ένα όνομα κλάσης οδηγού JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Λαμβάνει τη συμβολοσειρά σύνδεσης.

**Returns:**
java.lang.String - η συμβολοσειρά σύνδεσης.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Επιστρέφει ένα όνομα κλάσης οδηγού JDBC. Το προεπιλεγμένο όνομα κλάσης οδηγού είναι "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - συμβολοσειρά κλάσης οδηγού.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Ορίζει τη συμβολοσειρά σύνδεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η συμβολοσειρά σύνδεσης. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Ορίζει ένα όνομα κλάσης οδηγού JDBC. Το προεπιλεγμένο όνομα κλάσης οδηγού είναι "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ένα όνομα κλάσης οδηγού JDBC. |

