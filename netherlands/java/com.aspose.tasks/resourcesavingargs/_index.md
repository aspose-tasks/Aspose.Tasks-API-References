---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Deze klasse vertegenwoordigt een set gegevens die gerelateerd zijn aan het opslaan van externe hulpbronbestanden dat plaatsvindt tijdens de conversie naar HTML-indeling."
type: docs
weight: 254
url: /nl/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Deze klasse vertegenwoordigt een set gegevens die verband houden met het opslaan van een extern resourcebestand dat plaatsvindt tijdens de conversie naar HTML-indeling.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Sluit de stream als KeepStreamOpen false is, anders flush deze. |
| [getFileName()](#getFileName--) | Haalt de veronderstelde bestandsnaam op die van de converter naar de code van de aangepaste methode gaat. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Haalt een waarde op die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid. |
| [getStream()](#getStream--) | Haalt de binaire inhoud van het opgeslagen bestand op. |
| [getUri()](#getUri--) | Haalt de resource-URI op. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Stelt de veronderstelde bestandsnaam in die van de converter naar de code van de aangepaste methode gaat. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Stelt een waarde in die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Stelt de binaire inhoud van het opgeslagen bestand in. |
| [setUri(String value)](#setUri-java.lang.String-) | Stelt de resource-URI in. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Sluit de stream als KeepStreamOpen false is, anders flush deze.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Haalt de veronderstelde bestandsnaam op die van de converter naar de code van de aangepaste methode gaat. Kan worden gebruikt in aangepaste code om te bepalen hoe te verwerken of waar dat bestand op te slaan.

**Returns:**
java.lang.String - de veronderstelde bestandsnaam die van de converter naar de code van de aangepaste methode gaat.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Haalt een waarde op die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid.

**Returns:**
boolean - een waarde die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Haalt de binaire inhoud van het opgeslagen bestand op.

**Returns:**
java.io.OutputStream - de binaire inhoud van het opgeslagen bestand.
### getUri() {#getUri--}
```
public final String getUri()
```


Haalt de resource-URI op.

**Returns:**
java.lang.String - de resource-URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Stelt de veronderstelde bestandsnaam in die van de converter naar de code van de aangepaste methode gaat. Kan worden gebruikt in aangepaste code om te bepalen hoe te verwerken of waar dat bestand op te slaan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de veronderstelde bestandsnaam die van de converter naar de code van de aangepaste methode gaat. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Stelt een waarde in die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de stream open blijft nadat het opslaan van de hulpbron is voltooid. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Stelt de binaire inhoud van het opgeslagen bestand in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.io.OutputStream | de binaire inhoud van het opgeslagen bestand. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Stelt de resource-URI in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de resource-URI. |

