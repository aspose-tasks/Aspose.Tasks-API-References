---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Wert eines Gliederungscodes dar."
type: docs
weight: 167
url: /de/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Stellt einen Wert eines Gliederungscodes dar.

--------------------

Zwei Datenstücke sind erforderlich – ein Zeiger auf die Gliederungscode-Tabelle, die durch die FieldId angegeben wird, und der Wert, der entweder durch den ValueId oder den ValueGuid‑Zeiger auf die Werteliste angegeben wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Initialisiert eine neue Instanz der [OutlineCode](../../com.aspose.tasks/outlinecode)-Klasse. |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Initialisiert eine neue Instanz der [OutlineCode](../../com.aspose.tasks/outlinecode)-Klasse unter Verwendung des angegebenen Outline Code und eines seiner Werte. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFieldId()](#getFieldId--) | Liest den Zahlenwert des benutzerdefinierten Felds project Id. |
| [getValueGuid()](#getValueGuid--) | Liest die GUID des Wertes in der Werteliste. |
| [getValueId()](#getValueId--) | Liest die Id in der Werteliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Setzt den Zahlenwert des benutzerdefinierten Felds project Id. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Setzt die GUID des Wertes in der Werteliste. |
| [setValueId(int value)](#setValueId-int-) | Setzt die Id in der Werteliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Initialisiert eine neue Instanz der [OutlineCode](../../com.aspose.tasks/outlinecode)-Klasse.

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Initialisiert eine neue Instanz der [OutlineCode](../../com.aspose.tasks/outlinecode)-Klasse unter Verwendung des angegebenen Outline Code und eines seiner Werte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | Outline‑Code‑Definition. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | einer der Outline‑Code‑Definitionswerte. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Liest den Zahlenwert des benutzerdefinierten Felds project Id.

**Returns:**
java.lang.String – der Zahlenwert des benutzerdefinierten Felds project Id.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Liest die GUID des Wertes in der Werteliste. Der ValueGuid stimmt mit dem FieldGuid in der Werteliste überein.

**Returns:**
java.lang.String – die GUID des Wertes in der Werteliste.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Liest die Id in der Werteliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist.

**Returns:**
int – die Id in der Werteliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Setzt den Zahlenwert des benutzerdefinierten Felds project Id.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Zahlenwert des benutzerdefinierten Felds project Id. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Setzt die GUID des Wertes in der Werteliste. Der ValueGuid stimmt mit dem FieldGuid in der Werteliste überein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die GUID des Wertes in der Werteliste. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Setzt die Id in der Werteliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Id in der Wertliste, die mit der Definition in der Outline‑Code‑Sammlung verknüpft ist. |

