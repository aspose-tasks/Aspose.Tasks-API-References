---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API Reference"
description: "Applica l'AND logico a tutte le condizioni."
type: docs
weight: 11
url: /it/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Applica l'AND logico a tutte le condizioni. Per esempio: cond1 AND cond2 AND cond3...

T : Il tipo di oggetto a cui applicare l'interfaccia del metodo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Inizializza una nuova istanza della classe AndAllCondition&lt;T&gt;. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [check(T el)](#check-T-) | Restituisce true se l'oggetto specificato soddisfa le condizioni. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Inizializza una nuova istanza della classe AndAllCondition&lt;T&gt;.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| condizioni | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | L'elenco delle condizioni. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Restituisce true se l'oggetto specificato soddisfa le condizioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | L'oggetto da verificare. |

**Returns:**
boolean - True se l'oggetto soddisfa le condizioni.
