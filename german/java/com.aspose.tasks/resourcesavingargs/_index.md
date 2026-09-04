---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Diese Klasse repräsentiert eine Menge von Daten, die mit dem Speichern externer Ressourcendateien zusammenhängen, das während der Konvertierung ins HTML-Format auftritt."
type: docs
weight: 254
url: /de/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Diese Klasse stellt einen Datensatz dar, der sich auf das Speichern externer Ressourcendateien bezieht, das während der Konvertierung in das HTML-Format erfolgt.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Schließe den Stream, wenn KeepStreamOpen false ist, andernfalls spüle ihn. |
| [getFileName()](#getFileName--) | Gibt den erwarteten Dateinamen zurück, der vom Konverter zum Code der benutzerdefinierten Methode geht. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Gibt einen Wert zurück, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns offen gehalten wird. |
| [getStream()](#getStream--) | Gibt den binären Inhalt der gespeicherten Datei zurück. |
| [getUri()](#getUri--) | Gibt die Ressourcen-URI zurück. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Setzt den vermuteten Dateinamen, der vom Konverter zum Code der benutzerdefinierten Methode übergeht. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Setzt einen Wert, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns geöffnet bleibt. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Setzt den Binärinhalt der gespeicherten Datei. |
| [setUri(String value)](#setUri-java.lang.String-) | Setzt die Ressourcen-URI. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Schließe den Stream, wenn KeepStreamOpen false ist, andernfalls spüle ihn.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Liest den vermuteten Dateinamen, der vom Konverter zum Code der benutzerdefinierten Methode übergeht. Kann im benutzerdefinierten Code verwendet werden, um zu entscheiden, wie die Datei verarbeitet oder wo sie gespeichert wird.

**Returns:**
java.lang.String - der vermutete Dateiname, der vom Konverter zum Code der benutzerdefinierten Methode übergeht.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Gibt einen Wert zurück, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns offen gehalten wird.

**Returns:**
boolean - ein Wert, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns geöffnet bleibt.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Gibt den binären Inhalt der gespeicherten Datei zurück.

**Returns:**
java.io.OutputStream - der Binärinhalt der gespeicherten Datei.
### getUri() {#getUri--}
```
public final String getUri()
```


Gibt die Ressourcen-URI zurück.

**Returns:**
java.lang.String - die Ressourcen-URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Setzt den vermuteten Dateinamen, der vom Konverter zum Code der benutzerdefinierten Methode übergeht. Kann im benutzerdefinierten Code verwendet werden, um zu entscheiden, wie die Datei verarbeitet oder wo sie gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der vermutete Dateiname, der vom Konverter zum Code der benutzerdefinierten Methode übergeht. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Setzt einen Wert, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns geöffnet bleibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob der Stream nach Abschluss des Ressourcenspeicherns geöffnet bleibt. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Setzt den Binärinhalt der gespeicherten Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.io.OutputStream | der Binärinhalt der gespeicherten Datei. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Setzt die Ressourcen-URI.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Ressourcen-URI. |

