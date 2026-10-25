---
title: "En"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Past logische EN toe op de opgegeven voorwaarden."
type: docs
weight: 10
url: /nl/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Past logische EN toe op de opgegeven voorwaarden.

T : Het type object waarop de methode‑interface moet worden toegepast.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Initialiseert een nieuw exemplaar van de And&lt;T&gt;-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [check(T el)](#check-T-) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Initialiseert een nieuw exemplaar van de And&lt;T&gt;-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Eerste voorwaarde. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Tweede voorwaarde. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Retourneert true als het opgegeven object aan de voorwaarden voldoet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

**Returns:**
boolean - True als het object aan de voorwaarden voldoet.
