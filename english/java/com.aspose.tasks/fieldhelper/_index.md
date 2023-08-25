---
title: FieldHelper
second_title: Aspose.Tasks for Java API Reference
description: Helper class which provides useful operations with fields.
type: docs
weight: 88
url: /java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Helper class which provides useful operations with fields.
## Constructors

| Constructor | Description |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Returns a default title of the specific task field. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Returns a default title of the specific task field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskKey | byte | Task field to get a default title. |

**Returns:**
java.lang.String - A default title of the specific task field if the field can be displayed in MS Project's view, null otherwise.
