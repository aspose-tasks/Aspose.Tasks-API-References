---
title: "ExtendedAttribute"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les attributs étendus."
type: docs
weight: 81
url: /fr/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Représente les attributs étendus.

--------------------

Actuellement, tous les types d'attributs étendus sont pris en charge lors de la lecture depuis MSP Xml 2003/2007 et mpp 2003. Pour MSP mpp 2007, la lecture de tous les attributs étendus est prise en charge, à l'exception des durées et des indicateurs.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Obtient la définition de l'attribut. |
| [getDateValue()](#getDateValue--) | Obtient une valeur pour les attributs de type date (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Obtient la valeur pour les attributs de type 'Duration'. |
| [getFieldId()](#getFieldId--) | Obtient l'identifiant d'un champ. |
| [getFlagValue()](#getFlagValue--) | Obtient une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Obtient une valeur pour les attributs de types numériques (Cost, Number). |
| [getTextValue()](#getTextValue--) | Obtient une valeur pour les attributs de type 'Text'. |
| [getValueGuid()](#getValueGuid--) | Obtient le guid d'une valeur de recherche. |
| [getValueReadOnly()](#getValueReadOnly--) | Obtient une valeur indiquant si la valeur de cette instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) est en lecture seule. |
| [isErrorValue()](#isErrorValue--) | Obtient si le calcul de la valeur de l'attribut étendu a entraîné une erreur. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Définit une valeur pour les attributs de types date (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Définit la valeur pour les attributs de type 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Définit une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Définit une valeur pour les attributs de types numériques (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Définit une valeur pour les attributs de type 'Text'. |
| [toString()](#toString--) | Renvoie la représentation courte sous forme de chaîne d'un attribut étendu. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Obtient la définition de l'attribut.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Obtient une valeur pour les attributs de type date (Date, Start, Finish).

**Returns:**
java.util.Date - une valeur pour les attributs de types date (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Obtient la valeur pour les attributs de type 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Obtient l'identifiant d'un champ.

**Returns:**
java.lang.String - l'identifiant d'un champ.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Obtient une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'.

**Returns:**
boolean - une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Obtient une valeur pour les attributs de types numériques (Cost, Number).

**Returns:**
java.math.BigDecimal - une valeur pour les attributs de types numériques (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Obtient une valeur pour les attributs de type 'Text'.

**Returns:**
java.lang.String - une valeur pour les attributs de type 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Obtient le guid d'une valeur de recherche.

--------------------

Ne doit pas être défini directement, utilisez plutôt ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) pour créer un attribut étendu avec une valeur de recherche.

**Returns:**
java.lang.String - le guid d'une valeur de recherche.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Obtient une valeur indiquant si la valeur de cette instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) est en lecture seule.

Valeur : renvoie true si une formule ou un regroupement est défini dans le [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) pour cet objet.

**Returns:**
boolean - une valeur indiquant si la valeur de cette instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) est en lecture seule.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Obtient si le calcul de la valeur de l'attribut étendu a entraîné une erreur.

**Returns:**
boolean - indique si le calcul de la valeur de l'attribut étendu a entraîné une erreur.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Définit une valeur pour les attributs de types date (Date, Start, Finish).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur pour les attributs de types date (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Définit la valeur pour les attributs de type 'Duration'.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | valeur pour les attributs de type 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Définit une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Définit une valeur pour les attributs de types numériques (Cost, Number).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur pour les attributs de types numériques (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Définit une valeur pour les attributs de type 'Text'.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur pour les attributs de type 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Renvoie la représentation courte sous forme de chaîne d'un attribut étendu.

**Returns:**
java.lang.String - La représentation sous forme de chaîne de l'attribut étendu.
