---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API Reference"
description: "Wendet logisches UND auf alle Bedingungen an."
type: docs
weight: 11
url: /de/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Wendet logisches UND auf alle Bedingungen an. Zum Beispiel: cond1 AND cond2 AND cond3...

T : Der Typ des Objekts, auf das die Methodenschnittstelle angewendet werden soll.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Initialisiert eine neue Instanz der Klasse AndAllCondition&lt;T&gt;. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [check(T el)](#check-T-) | Gibt true zurück, wenn das angegebene Objekt die Bedingungen erfüllt. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Initialisiert eine neue Instanz der Klasse AndAllCondition&lt;T&gt;.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bedingungen | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | Die Liste der Bedingungen. |

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
