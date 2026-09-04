---
title: "Nicht"
second_title: "Aspose.Tasks for Java API Reference"
description: "Wendet logisches NOT auf die angegebene Bedingung an."
type: docs
weight: 162
url: /de/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Wendet logisches NOT auf die angegebene Bedingung an.

T : Der Typ des Objekts, auf das die Methodenschnittstelle angewendet werden soll.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Initialisiert eine neue Instanz der Not&lt;T&gt;-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [check(T el)](#check-T-) | Gibt true zurück, wenn das angegebene Objekt die Bedingung erfüllt. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Initialisiert eine neue Instanz der Not&lt;T&gt;-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Angegebene Bedingung. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Gibt true zurück, wenn das angegebene Objekt die Bedingung erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Das zu prüfende Objekt. |

**Returns:**
boolean - True, wenn das Objekt die Bedingung erfüllt.
