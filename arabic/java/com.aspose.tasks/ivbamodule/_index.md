---
title: "IVbaModule"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل وحدة تحتوي على شفرة VBA."
type: docs
weight: 385
url: /ar/java/com.aspose.tasks/ivbamodule/
---
```
public interface IVbaModule
```

يمثل وحدة تحتوي على شفرة VBA.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAttributes()](#getAttributes--) | يحصل على مجموعة من [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection). |
| [getName()](#getName--) | يسترجع اسم وحدة VBA |
| [getSourceCode()](#getSourceCode--) | يسترجع شفرة المصدر لوحدة VBA |
### getAttributes() {#getAttributes--}
```
public abstract VbaModuleAttributeCollection getAttributes()
```


يحصل على مجموعة من [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection).

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of [VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection)
### getName() {#getName--}
```
public abstract String getName()
```


يسترجع اسم وحدة VBA

**Returns:**
java.lang.String - اسم وحدة VBA
### getSourceCode() {#getSourceCode--}
```
public abstract String getSourceCode()
```


يسترجع شفرة المصدر لوحدة VBA

**Returns:**
java.lang.String - شفرة المصدر لوحدة VBA
