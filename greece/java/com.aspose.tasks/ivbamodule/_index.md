---
title: "IVbaModule"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια μονάδα με κώδικα VBA."
type: docs
weight: 385
url: /el/java/com.aspose.tasks/ivbamodule/
---
```
public interface IVbaModule
```

Αντιπροσωπεύει μια μονάδα με κώδικα VBA.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAttributes()](#getAttributes--) | Λαμβάνει μια συλλογή των [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) |
| [getName()](#getName--) | Λαμβάνει το όνομα της μονάδας VBA. |
| [getSourceCode()](#getSourceCode--) | Λαμβάνει τον πηγαίο κώδικα της μονάδας VBA. |
### getAttributes() {#getAttributes--}
```
public abstract VbaModuleAttributeCollection getAttributes()
```


Λαμβάνει μια συλλογή των [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection)

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection)
### getName() {#getName--}
```
public abstract String getName()
```


Λαμβάνει το όνομα της μονάδας VBA.

**Returns:**
java.lang.String - ένα όνομα της μονάδας VBA.
### getSourceCode() {#getSourceCode--}
```
public abstract String getSourceCode()
```


Λαμβάνει τον πηγαίο κώδικα της μονάδας VBA.

**Returns:**
java.lang.String - κώδικας πηγής του VBA module
