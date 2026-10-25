---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare i parametri del livellamento delle risorse."
type: docs
weight: 142
url: /it/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Consente di specificare i parametri del livellamento delle risorse.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Inizializza una nuova istanza della classe [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Ottiene un token che può essere usato per annullare un'operazione di livellamento del progetto. |
| [getFinishDate()](#getFinishDate--) | Ottiene la data di fine del periodo di livellamento. |
| [getLevelingOrder()](#getLevelingOrder--) | Ottiene l'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. |
| [getMessageHandler()](#getMessageHandler--) | Ottiene la callback del gestore dei messaggi che può essere usata per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse. |
| [getMessageLevel()](#getMessageLevel--) | Ottiene il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse. |
| [getResources()](#getResources--) | Ottiene l'elenco delle risorse che saranno livellate. |
| [getStartDate()](#getStartDate--) | Ottiene la data di inizio del periodo di livellamento. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Imposta un token che può essere usato per annullare un'operazione di livellamento del progetto. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Imposta la data di fine del periodo di livellamento. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | L'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Imposta il callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Imposta il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Imposta l'elenco delle risorse che saranno livellate. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Imposta la data di inizio del periodo di livellamento. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Inizializza una nuova istanza della classe [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Ottiene un token che può essere usato per annullare un'operazione di livellamento del progetto.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Ottiene la data di fine del periodo di livellamento. Il valore predefinito è la data di conclusione del progetto.

**Returns:**
java.util.Date - data di fine del periodo di livellamento.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Ottiene l'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. Dopo aver determinato le attività che causano la sovrallocazione e quali attività possono essere ritardate, l'ordine specificato viene utilizzato per stabilire quale attività deve essere ritardata per prima.

**Returns:**
int - l'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Ottiene la callback del gestore dei messaggi che può essere usata per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Ottiene il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse.

**Returns:**
int - livello dei messaggi di log emessi da Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Ottiene l'elenco delle risorse che saranno livellate. Se viene impostato null, tutte le risorse del progetto saranno livellate.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - l'elenco delle risorse che saranno livellate.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Ottiene la data di inizio del periodo di livellamento. Il valore predefinito è la data di inizio del progetto.

**Returns:**
java.util.Date - data di inizio del periodo di livellamento.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Imposta un token che può essere usato per annullare un'operazione di livellamento del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un token che può essere usato per annullare un'operazione di livellamento del progetto. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Imposta la data di fine del periodo di livellamento. Il valore predefinito è la data di conclusione del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | data di fine del periodo di livellamento. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


L'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. Dopo aver determinato le attività che causano la sovrallocazione e quali attività possono essere ritardate, l'ordine specificato viene utilizzato per stabilire quale attività deve essere ritardata per prima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'ordine in cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Imposta il callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Imposta il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | livello dei messaggi di log emessi da Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Imposta l'elenco delle risorse che saranno livellate. Se viene impostato null, tutte le risorse del progetto saranno livellate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.List&lt;com.aspose.tasks.Resource&gt; | l'elenco delle risorse che saranno livellate. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Imposta la data di inizio del periodo di livellamento. Il valore predefinito è la data di inizio del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | data di inizio del periodo di livellamento. |

