---
title: "OleObjectCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή που περιέχει τις παρουσίες της κλάσης."
type: docs
weight: 165
url: /el/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Αντιπροσωπεύει μια συλλογή που περιέχει τις παρουσίες της κλάσης [OleObject](../../com.aspose/tasks/oleobject).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \\{@inheritDoc\\} |
| [clear()](#clear--) | Καθαρίζει τη συλλογή. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Επιστρέφει τον αριθμό των στοιχείων σε αυτή τη συλλογή. |
| [toList()](#toList--) | Μετατρέπει την παρουσία της κλάσης [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) σε μια λίστα που περιέχει τις παρουσίες της κλάσης [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Καθαρίζει τη συλλογή. Για να διατηρηθούν αυτές οι αλλαγές, πρέπει να κληθεί το project.Save με νέο MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Πώς να καθαρίσετε τα αντικείμενα OLE και να διατηρήσετε αυτές τις αλλαγές.
&gt; ``````

 [C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
 
```



### get(int index) {#get-int-}
```
public OleObject get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[OleObject](../../com.aspose.tasks/oleobject) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Returns the number of elements in this collection.

**Returns:**
int - the number of elements in this collection.
### toList() {#toList--}
```
public final List<OleObject> toList()
```


Converts the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class to a list containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.

**Returns:**
java.util.List&lt;com.aspose.tasks.OleObject&gt; - Converted to list the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.
