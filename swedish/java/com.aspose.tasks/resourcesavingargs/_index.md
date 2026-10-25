---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API-referens"
description: "Denna klass representerar en uppsättning data som är relaterade till sparande av externa resursfiler som sker under konvertering till HTML-format."
type: docs
weight: 254
url: /sv/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Denna klass representerar en uppsättning data som är relaterade till sparande av extern resursfil som sker under konvertering till HTML-format.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Stäng strömmen om KeepStreamOpen är falskt, annars spola den. |
| [getFileName()](#getFileName--) | Hämtar det förmodade filnamnet som går från konverteraren till koden för en anpassad metod. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Hämtar ett värde som indikerar om strömmen kommer att hållas öppen efter att resurslagringen är klar. |
| [getStream()](#getStream--) | Hämtar det binära innehållet i den sparade filen. |
| [getUri()](#getUri--) | Hämtar resursens URI. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Ställer in det förmodade filnamnet som går från konverteraren till koden för en anpassad metod. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Ställer in ett värde som indikerar om strömmen kommer att hållas öppen efter att resurslagringen är klar. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Ställer in det binära innehållet i den sparade filen. |
| [setUri(String value)](#setUri-java.lang.String-) | Ställer in resursens URI. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Stäng strömmen om KeepStreamOpen är falskt, annars spola den.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Hämtar det förmodade filnamnet som går från konverteraren till koden för en anpassad metod. Kan användas i anpassad kod för att besluta hur man bearbetar eller var man sparar den filen.

**Returns:**
java.lang.String - det förmodade filnamnet som går från konverteraren till koden för en anpassad metod.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Hämtar ett värde som indikerar om strömmen kommer att hållas öppen efter att resurslagringen är klar.

**Returns:**
boolean - ett värde som indikerar om strömmen ska hållas öppen efter att resurssparandet är slutfört.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Hämtar det binära innehållet i den sparade filen.

**Returns:**
java.io.OutputStream - det binära innehållet i den sparade filen.
### getUri() {#getUri--}
```
public final String getUri()
```


Hämtar resursens URI.

**Returns:**
java.lang.String - resursens URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Ställer in det förmodade filnamnet som går från konverteraren till koden för en anpassad metod. Kan användas i anpassad kod för att bestämma hur filen ska behandlas eller var den ska sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det förmodade filnamnet som går från konverteraren till koden för en anpassad metod. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Ställer in ett värde som indikerar om strömmen kommer att hållas öppen efter att resurslagringen är klar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om strömmen ska hållas öppen efter att resurssparandet är slutfört. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Ställer in det binära innehållet i den sparade filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.io.OutputStream | det binära innehållet i den sparade filen. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Ställer in resursens URI.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | resursens URI. |

