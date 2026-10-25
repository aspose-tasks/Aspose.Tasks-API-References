---
title: "Und"
second_title: "Aspose.Tasks for Java API Reference"
description: "Wendet logisches UND auf die angegebenen Bedingungen an."
type: docs
weight: 10
url: /de/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Wendet logisches UND auf die angegebenen Bedingungen an.

T : Der Typ des Objekts, auf das die Methodenschnittstelle angewendet werden soll.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Initialisiert eine neue Instanz der Klasse And&lt;T&gt;. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [check(T el)](#check-T-) | Gibt true zurück, wenn das angegebene Objekt die Bedingungen erfüllt. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Initialisiert eine neue Instanz der Klasse And&lt;T&gt;.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Erste Bedingung. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Zweite Bedingung. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Gibt true zurück, wenn das angegebene Objekt die Bedingungen erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Das zu prüfende Objekt. |

**Returns:**
boolean - True, wenn das Objekt die Bedingungen erfüllt.
