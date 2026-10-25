---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Fornisce argomenti per il callback che viene invocato quando il carattere è risolto."
type: docs
weight: 99
url: /it/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Fornisce argomenti per il callback che viene invocato quando il carattere è risolto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Ottiene il nome del carattere richiesto. |
| [getResolvedFontName()](#getResolvedFontName--) | Ottiene il nome del carattere risolto. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Imposta il nome del carattere risolto. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Ottiene il nome del carattere richiesto.

**Returns:**
java.lang.String - il nome del carattere richiesto.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Ottiene il nome del carattere risolto. Può essere impostato per controllare i caratteri usati per rendere una vista.

**Returns:**
java.lang.String - Nome del carattere richiesto se il carattere è trovato o nome del carattere di riserva o null se il carattere non può essere trovato.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Imposta il nome del carattere risolto. Può essere impostato per controllare i caratteri usati per rendere una vista.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome del carattere risolto. |

