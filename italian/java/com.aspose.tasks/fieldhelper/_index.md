---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di supporto che fornisce operazioni utili sui campi."
type: docs
weight: 88
url: /it/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Classe di supporto che fornisce operazioni utili sui campi.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Restituisce un titolo predefinito del campo specifico. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Restituisce un titolo predefinito del campo attività specifico. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Restituisce un titolo predefinito del campo specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| campo | int | Campo per ottenere un titolo predefinito. |

**Returns:**
java.lang.String - Un titolo predefinito del campo specifico se il campo può essere visualizzato nella vista di MS Project, altrimenti null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Restituisce un titolo predefinito del campo attività specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskKey | byte | Campo attività per ottenere un titolo predefinito. |

**Returns:**
java.lang.String - Un titolo predefinito del campo attività specifico se il campo può essere visualizzato nella vista di MS Project, altrimenti null.
