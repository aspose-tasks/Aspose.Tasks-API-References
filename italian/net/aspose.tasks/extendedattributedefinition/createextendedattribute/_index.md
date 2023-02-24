---
title: ExtendedAttributeDefinition.CreateExtendedAttribute
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Crea un nuovo attributo esteso con lID campo uguale al valore dellID campo di questo oggetto.
type: docs
weight: 300
url: /it/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Crea un nuovo attributo esteso con l'ID campo uguale al valore dell'ID campo di questo oggetto.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore di testo specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| textValue | String | Il valore di testo specificato. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se attuale[`CfType`](../cftype/) non è "Testo" |

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore numerico specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| numericValue | Decimal | Il valore numerico specificato. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se attuale[`CfType`](../cftype/) non è 'Numero' o 'Costo' |

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore data specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTimeValue | DateTime | Il valore di data e ora specificato. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se attuale[`CfType`](../cftype/) non è 'Data', 'Inizio' o 'Fine' |

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Crea un nuovo attributo esteso con l'ID campo uguale al valore dell'ID campo di questo oggetto e al valore di durata specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| durationValue | Duration | Il valore di durata specificato. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se attuale[`CfType`](../cftype/) non è 'Durata' |

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore flag specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flagValue | Boolean | Il valore del flag specificato. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/)class con il fieldID uguale al valore fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se attuale[`CfType`](../cftype/) non è 'Bandiera' |

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Crea un nuovo attributo esteso collegato a specificato[`Value`](../../value/) oggetto.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lookupValue | Value | Il specificato[`Value`](../../value/) articolo. |

### Valore di ritorno

restituisce l'istanza creata di[`ExtendedAttribute`](../../extendedattribute/) classe collegata con specificato[`Value`](../../value/) articolo.

### Osservazioni

*lookupValue* dovrebbe essere precedentemente aggiunto al[`ExtendedAttributeDefinition`](../) utilizzando[`AddLookupValue`](../addlookupvalue/) metodo.

### Esempi

Usa questo codice per crearne di nuovi[`ExtendedAttribute`](../../extendedattribute/) utilizzando un valore specifico:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

### Guarda anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


