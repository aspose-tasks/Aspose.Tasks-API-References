---
title: "Non"
second_title: "Aspose.Tasks for Java API Reference"
description: "Applica il NOT logico alla condizione specificata."
type: docs
weight: 162
url: /it/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Applica il NOT logico alla condizione specificata.

T : Il tipo di oggetto a cui applicare l'interfaccia del metodo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Inizializza una nuova istanza della classe Not&lt;T&gt;. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [check(T el)](#check-T-) | Restituisce true se l'oggetto specificato soddisfa la condizione. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Inizializza una nuova istanza della classe Not&lt;T&gt;.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Condizione specificata. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Restituisce true se l'oggetto specificato soddisfa la condizione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | L'oggetto da verificare. |

**Returns:**
boolean - True se l'oggetto soddisfa la condizione.
