---
title: "Niet"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Past logische NOT toe op de opgegeven voorwaarde."
type: docs
weight: 162
url: /nl/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Past logische NOT toe op de opgegeven voorwaarde.

T : Het type object waarop de methode‑interface moet worden toegepast.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Initialiseert een nieuw exemplaar van de Not&lt;T&gt; klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [check(T el)](#check-T-) | Retourneert true als het opgegeven object aan de voorwaarde voldoet. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Initialiseert een nieuw exemplaar van de Not&lt;T&gt; klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Opgegeven voorwaarde. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Retourneert true als het opgegeven object aan de voorwaarde voldoet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

**Returns:**
boolean - True als het object aan de voorwaarde voldoet.
