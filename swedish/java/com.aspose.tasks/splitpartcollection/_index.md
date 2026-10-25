---
title: "SplitPartCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Samling som representerar delarna av en uppgift."
type: docs
weight: 279
url: /sv/java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

Samling som representerar delarna av en uppgift.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [get(int index)](#get-int-) | Hämtar en uppgifts split‑del på det angivna indexet. |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | Ställer in en uppgifts split‑del på det angivna indexet. |
| [size()](#size--) | Hämtar antalet delar i samlingen. |
| [toArray()](#toArray--) | Kopierar alla delar från samlingen till en ny array. |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


Hämtar en uppgifts split‑del på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Delens index. |

--------------------

Indexet är nollbaserat. Returnerar null om indexet ligger utanför arrayens gränser. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


Ställer in en uppgifts split‑del på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Delens index. |

--------------------

Indexet är nollbaserat. Returnerar null om indexet ligger utanför arrayens gränser. |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | en split‑del att sätta. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


Hämtar antalet delar i samlingen.

**Returns:**
int - antalet delar i samlingen.
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


Kopierar alla delar från samlingen till en ny array.

**Returns:**
com.aspose.tasks.SplitPart[] - En array av [SplitPart](../../com.aspose.tasks/splitpart) objekt.
