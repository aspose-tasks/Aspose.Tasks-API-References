---
title: OutlineCodeDefinition
second_title: Aspose.Tasks for Java API Reference
description: Represents an outline code definition.
type: docs
weight: 164
url: /java/com.aspose.tasks/outlinecodedefinition/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCodeDefinition
```

Represents an outline code definition.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineCodeDefinition()](#OutlineCodeDefinition--) | Initializes a new instance of the [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) class. |
## Methods

| Method | Description |
| --- | --- |
| [getAlias()](#getAlias--) | Gets the alias of a custom outline code. |
| [getAllLevelsRequired()](#getAllLevelsRequired--) | Gets a value indicating whether the new codes must have all levels. |
| [getEnterprise()](#getEnterprise--) | Gets a value indicating whether a custom outline code is an enterprise custom outline code. |
| [getEnterpriseOutlineCodeAlias()](#getEnterpriseOutlineCodeAlias--) | Gets a reference to another custom field for which this outline code definition is an alias. |
| [getFieldId()](#getFieldId--) | Gets the field number of an outline code. |
| [getFieldName()](#getFieldName--) | Gets the name of a custom outline code. |
| [getGuid()](#getGuid--) | Gets the Guid of an outline code. |
| [getLeafOnly()](#getLeafOnly--) | Gets a value indicating whether the values specified in this outline code field must be leaf values. |
| [getMasks()](#getMasks--) | Gets the OutlineMaskCollection object. |
| [getOnlyTableValuesAllowed()](#getOnlyTableValuesAllowed--) | Gets a value indicating whether the values specified must come from values table. |
| [getPhoneticAlias()](#getPhoneticAlias--) | Gets the phonetic pronunciation of the alias of the custom outline code. |
| [getResourceSubstitutionEnabled()](#getResourceSubstitutionEnabled--) | Gets a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project. |
| [getShowIndent()](#getShowIndent--) | Gets a value indicating whether the indents of this outline code must be shown. |
| [getValues()](#getValues--) | Gets OutlineValueCollection object. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Sets the alias of a custom outline code. |
| [setAllLevelsRequired(boolean value)](#setAllLevelsRequired-boolean-) | Sets a value indicating whether the new codes must have all levels. |
| [setEnterprise(boolean value)](#setEnterprise-boolean-) | Sets a value indicating whether a custom outline code is an enterprise custom outline code. |
| [setEnterpriseOutlineCodeAlias(int value)](#setEnterpriseOutlineCodeAlias-int-) | Sets a reference to another custom field for which this outline code definition is an alias. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Sets the field number of an outline code. |
| [setFieldName(String value)](#setFieldName-java.lang.String-) | Sets the name of a custom outline code. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Sets the Guid of an outline code. |
| [setLeafOnly(boolean value)](#setLeafOnly-boolean-) | Sets a value indicating whether the values specified in this outline code field must be leaf values. |
| [setOnlyTableValuesAllowed(boolean value)](#setOnlyTableValuesAllowed-boolean-) | Sets a value indicating whether the values specified must come from values table. |
| [setPhoneticAlias(String value)](#setPhoneticAlias-java.lang.String-) | Sets the phonetic pronunciation of the alias of the custom outline code. |
| [setResourceSubstitutionEnabled(boolean value)](#setResourceSubstitutionEnabled-boolean-) | Sets a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project. |
| [setShowIndent(boolean value)](#setShowIndent-boolean-) | Sets a value indicating whether the indents of this outline code must be shown. |
### OutlineCodeDefinition() {#OutlineCodeDefinition--}
```
public OutlineCodeDefinition()
```


Initializes a new instance of the [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) class.

### getAlias() {#getAlias--}
```
public final String getAlias()
```


Gets the alias of a custom outline code.

**Returns:**
java.lang.String - the alias of a custom outline code.
### getAllLevelsRequired() {#getAllLevelsRequired--}
```
public final boolean getAllLevelsRequired()
```


Gets a value indicating whether the new codes must have all levels. Not available for Enterprise Codes.

**Returns:**
boolean - a value indicating whether the new codes must have all levels.
### getEnterprise() {#getEnterprise--}
```
public final boolean getEnterprise()
```


Gets a value indicating whether a custom outline code is an enterprise custom outline code.

**Returns:**
boolean - a value indicating whether a custom outline code is an enterprise custom outline code.
### getEnterpriseOutlineCodeAlias() {#getEnterpriseOutlineCodeAlias--}
```
public final int getEnterpriseOutlineCodeAlias()
```


Gets a reference to another custom field for which this outline code definition is an alias.

**Returns:**
int - a reference to another custom field for which this outline code definition is an alias.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets the field number of an outline code.

**Returns:**
java.lang.String - the field number of an outline code.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the name of a custom outline code.

**Returns:**
java.lang.String - the name of a custom outline code.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets the Guid of an outline code.

**Returns:**
java.lang.String - the Guid of an outline code.
### getLeafOnly() {#getLeafOnly--}
```
public final boolean getLeafOnly()
```


Gets a value indicating whether the values specified in this outline code field must be leaf values.

**Returns:**
boolean - a value indicating whether the values specified in this outline code field must be leaf values.
### getMasks() {#getMasks--}
```
public final OutlineMaskCollection getMasks()
```


Gets the OutlineMaskCollection object. The table of entries that define the outline code mask. Read-only [OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection) instance.

**Returns:**
[OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection) - the OutlineMaskCollection object.
### getOnlyTableValuesAllowed() {#getOnlyTableValuesAllowed--}
```
public final boolean getOnlyTableValuesAllowed()
```


Gets a value indicating whether the values specified must come from values table.

**Returns:**
boolean - a value indicating whether the values specified must come from values table.
### getPhoneticAlias() {#getPhoneticAlias--}
```
public final String getPhoneticAlias()
```


Gets the phonetic pronunciation of the alias of the custom outline code.

**Returns:**
java.lang.String - the phonetic pronunciation of the alias of the custom outline code.
### getResourceSubstitutionEnabled() {#getResourceSubstitutionEnabled--}
```
public final boolean getResourceSubstitutionEnabled()
```


Gets a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project.

**Returns:**
boolean - a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project.
### getShowIndent() {#getShowIndent--}
```
public final boolean getShowIndent()
```


Gets a value indicating whether the indents of this outline code must be shown.

--------------------

This is new for MS Project 2010 property.

**Returns:**
boolean - a value indicating whether the indents of this outline code must be shown.
### getValues() {#getValues--}
```
public final OutlineValueCollection getValues()
```


Gets OutlineValueCollection object. The values of the table associated with this outline code.

**Returns:**
[OutlineValueCollection](../../com.aspose.tasks/outlinevaluecollection) - OutlineValueCollection object.
### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Sets the alias of a custom outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the alias of a custom outline code. |

### setAllLevelsRequired(boolean value) {#setAllLevelsRequired-boolean-}
```
public final void setAllLevelsRequired(boolean value)
```


Sets a value indicating whether the new codes must have all levels. Not available for Enterprise Codes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the new codes must have all levels. |

### setEnterprise(boolean value) {#setEnterprise-boolean-}
```
public final void setEnterprise(boolean value)
```


Sets a value indicating whether a custom outline code is an enterprise custom outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a custom outline code is an enterprise custom outline code. |

### setEnterpriseOutlineCodeAlias(int value) {#setEnterpriseOutlineCodeAlias-int-}
```
public final void setEnterpriseOutlineCodeAlias(int value)
```


Sets a reference to another custom field for which this outline code definition is an alias.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a reference to another custom field for which this outline code definition is an alias. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets the field number of an outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the field number of an outline code. |

### setFieldName(String value) {#setFieldName-java.lang.String-}
```
public final void setFieldName(String value)
```


Sets the name of a custom outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of a custom outline code. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Sets the Guid of an outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Guid of an outline code. |

### setLeafOnly(boolean value) {#setLeafOnly-boolean-}
```
public final void setLeafOnly(boolean value)
```


Sets a value indicating whether the values specified in this outline code field must be leaf values.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the values specified in this outline code field must be leaf values. |

### setOnlyTableValuesAllowed(boolean value) {#setOnlyTableValuesAllowed-boolean-}
```
public final void setOnlyTableValuesAllowed(boolean value)
```


Sets a value indicating whether the values specified must come from values table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the values specified must come from values table. |

### setPhoneticAlias(String value) {#setPhoneticAlias-java.lang.String-}
```
public final void setPhoneticAlias(String value)
```


Sets the phonetic pronunciation of the alias of the custom outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the phonetic pronunciation of the alias of the custom outline code. |

### setResourceSubstitutionEnabled(boolean value) {#setResourceSubstitutionEnabled-boolean-}
```
public final void setResourceSubstitutionEnabled(boolean value)
```


Sets a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project. |

### setShowIndent(boolean value) {#setShowIndent-boolean-}
```
public final void setShowIndent(boolean value)
```


Sets a value indicating whether the indents of this outline code must be shown.

--------------------

This is new for MS Project 2010 property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the indents of this outline code must be shown. |

