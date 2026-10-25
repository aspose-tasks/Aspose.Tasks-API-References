---
title: "E"
second_title: "Aspose.Tasks for Java API Reference"
description: "Applica l'AND logico alle condizioni specificate."
type: docs
weight: 10
url: /it/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Applica l'AND logico alle condizioni specificate.

T : Il tipo di oggetto a cui applicare l'interfaccia del metodo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Inizializza una nuova istanza della classe And&lt;T&gt;. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [check(T el)](#check-T-) | Restituisce true se l'oggetto specificato soddisfa le condizioni. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Inizializza una nuova istanza della classe And&lt;T&gt;.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Prima condizione. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Seconda condizione. |

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
