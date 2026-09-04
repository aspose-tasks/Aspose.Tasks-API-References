---
title: "ResourceViewColumn"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση προβολής έργων που χρησιμοποιείται στην προβολή ResourceUsage και στην προβολή ResourceSheet."
type: docs
weight: 261
url: /el/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Κλάση προβολής έργου που χρησιμοποιείται στην προβολή ResourceUsage και στην προβολή ResourceSheet.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Μετατρέπει τον τρέχοντα πόρο σε κείμενο στήλης. |
| [getField()](#getField--) | Επιστρέφει το πεδίο της στήλης. |
| [setField(int value)](#setField-int-) | Ορίζει το πεδίο της στήλης. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Μετατροπέας δεδομένων πόρου σε κείμενο στήλης. |
| πεδίο | int | Πεδίο στήλης. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Μετατροπέας δεδομένων πόρου σε κείμενο στήλης. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | int | Πεδίο στήλης. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Μετατρέπει τον τρέχοντα πόρο σε κείμενο στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Τρέχων πόρος. |

**Returns:**
java.lang.String - Το κείμενο της στήλης.
### getField() {#getField--}
```
public int getField()
```


Επιστρέφει το πεδίο της στήλης. `Field`.

**Returns:**
int - τιμή πεδίου στήλης.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Ορίζει το πεδίο της στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | τιμή πεδίου στήλης. |

