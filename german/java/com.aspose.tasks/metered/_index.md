---
title: "Metered"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Methoden zum Festlegen eines gemessenen Schlüssels bereit."
type: docs
weight: 152
url: /de/java/com.aspose.tasks/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Stellt Methoden zum Festlegen eines gemessenen Schlüssels bereit.

--------------------

In diesem Beispiel wird versucht, den öffentlichen und privaten Schlüssel für metered in der Komponenten‑Jar‑Datei zu setzen:

```

``````

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
```


## Constructors

| Constructor | Description |
| --- | --- |
| [Metered()](#Metered--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getConsumptionCredit()](#getConsumptionCredit--) | Gets consumption credit. |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Gets consumption file size. |
| [isLicensed()](#isLicensed--) | Checks whether the product is successfully licensed using Metered license. |
| [resetMeteredKey()](#resetMeteredKey--) | Removes previously setup license. |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Sets metered public and private keys. |
### Metered() {#Metered--}
```
public Metered()
```


### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Gets consumption credit.

**Returns:**
java.math.BigDecimal - Returns the number of consumed credit points.
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Gets consumption file size.

**Returns:**
java.math.BigDecimal - Returns the number of consumed bytes.
### isLicensed() {#isLicensed--}
```
public final boolean isLicensed()
```


Checks whether the product is successfully licensed using Metered license.

**Returns:**
boolean - true or false
### resetMeteredKey() {#resetMeteredKey--}
```
public final void resetMeteredKey()
```


Removes previously setup license.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Sets metered public and private keys.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | The public key. |
| privateKey | java.lang.String | The private key.

--------------------

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again. |

