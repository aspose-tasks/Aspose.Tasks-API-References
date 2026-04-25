---
title: GlobalizationSettings
second_title: Aspose.Tasks for Java API Reference
description: Represents the projects globalization settings.
type: docs
weight: 114
url: /java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Represents the project's globalization settings.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the formula-calculation engine parse those literals.
## Constructors

| Constructor | Description |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | Gets a string for boolean 'false' literal used in a formula. |
| [getFormulaDateNA()](#getFormulaDateNA--) | Gets "NA" (empty value) literal used in a formula for a date field. |
| [getTrueLiteral()](#getTrueLiteral--) | Gets a string for boolean 'true' literal used in a formula. |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


Gets a string for boolean 'false' literal used in a formula.

**Returns:**
java.lang.String - a string for boolean 'false' literal used in a formula.
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


Gets "NA" (empty value) literal used in a formula for a date field.

**Returns:**
java.lang.String - "NA" (empty value) literal used in a formula for a date field.
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


Gets a string for boolean 'true' literal used in a formula.

**Returns:**
java.lang.String - a string for boolean 'true' literal used in a formula.
