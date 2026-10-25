---
title: "ExtendedAttributeDefinition"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili definisi atribut tambahan yang terkait dengan proyek."
type: docs
weight: 83
url: /id/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Mewakili definisi atribut tambahan yang terkait dengan proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Menambahkan nilai ke daftar lookup internal. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Membandingkan objek ini dengan instance lain dari kelas @\{code ExtendedAttributeDefinition\}. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai flag yang ditentukan. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai durasi yang ditentukan. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Membuat atribut ekstended baru yang terhubung dengan item [Value](../../com.aspose.tasks/value) yang ditentukan. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai teks yang ditentukan. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai numerik yang ditentukan. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai tanggal yang ditentukan. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended dengan lookup. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended dengan lookup. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended dengan lookup. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended dengan lookup. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai "None". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai "None". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai "None". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Metode pabrik yang membuat definisi atribut ekstended sederhana, yang ditampilkan Microsoft Project sebagai "None". |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getAlias()](#getAlias--) | Mendapatkan alias dari bidang khusus. |
| [getAppendNewValues()](#getAppendNewValues--) | Mendapatkan nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar. |
| [getAutoRollDown()](#getAutoRollDown--) | Mendapatkan nilai yang menunjukkan apakah roll down otomatis ke penugasan diaktifkan. |
| [getCalculationType()](#getCalculationType--) | Mendapatkan tipe perhitungan nilai atribut khusus. |
| [getCfType()](#getCfType--) | Mendapatkan tipe dari bidang khusus. |
| [getDefault()](#getDefault--) | Mendapatkan nilai default dalam daftar. |
| [getDefaultGuid()](#getDefaultGuid--) | Mendapatkan Guid dari entri tabel lookup default. |
| [getElementType()](#getElementType--) | Mendapatkan atribut ekstended yang terkait dengan tugas, sumber daya, atau penugasan. |
| [getFieldId()](#getFieldId--) | Mendapatkan yang sesuai dengan ID proyek dari bidang khusus. |
| [getFieldName()](#getFieldName--) | Mendapatkan nama dari bidang khusus. |
| [getFormula()](#getFormula--) | Mendapatkan formula yang digunakan Microsoft Project untuk mengisi bidang tugas khusus. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Mendapatkan informasi indikator grafis yang terkait dengan atribut ekstended. |
| [getGuid()](#getGuid--) | Mendapatkan Guid dari bidang khusus. |
| [getLookupUid()](#getLookupUid--) | Mendapatkan Guid dari tabel lookup yang terkait dengan bidang khusus. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Mendapatkan jumlah maksimum nilai yang dapat Anda atur dalam daftar pilihan. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk untuk instance [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Mendapatkan pengucapan fonetik dari alias bidang khusus. |
| [getRestrictValues()](#getRestrictValues--) | Mendapatkan nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Mendapatkan cara rollup dihitung. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Mendapatkan guid sekunder dari atribut ekstended. |
| [getSecondaryPid()](#getSecondaryPid--) | Mendapatkan PID sekunder dari bidang khusus. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Mendapatkan tipe perhitungan nilai atribut khusus untuk baris ringkasan. |
| [getUserDef()](#getUserDef--) | Mendapatkan nilai yang menunjukkan apakah bidang khusus didefinisikan pengguna. |
| [getValueList()](#getValueList--) | Mendapatkan List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Mendapatkan cara daftar nilai diurutkan. |
| [hashCode()](#hashCode--) | Mengembalikan kode hash untuk instance dari kelas [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Menghapus nilai dari daftar lookup internal. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Mengatur alias dari bidang khusus. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Mengatur nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Mengatur nilai yang menunjukkan apakah roll down otomatis ke penugasan diaktifkan. |
| [setCalculationType(int value)](#setCalculationType-int-) | Mengatur jenis perhitungan nilai atribut khusus. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Mengatur nilai default dalam daftar. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Mengatur Guid dari entri tabel lookup default. |
| [setElementType(int value)](#setElementType-int-) | Mengatur atribut ekstended terkait dengan tugas, sumber daya, atau penugasan. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Mengatur yang sesuai dengan ID proyek dari bidang khusus. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Mengatur formula yang digunakan Microsoft Project untuk mengisi bidang tugas khusus. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Mengatur informasi indikator grafis yang terkait dengan atribut ekstended. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Mengatur Guid dari bidang khusus. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Mengatur jumlah maksimum nilai yang dapat Anda atur dalam daftar pilihan. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Mengatur pelafalan fonetik alias dari bidang khusus. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Mengatur nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Mengatur cara perhitungan rollup. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Mengatur guid sekunder dari atribut ekstended. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Mengatur PID sekunder dari bidang khusus. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Mengatur jenis perhitungan nilai atribut khusus untuk baris ringkasan. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Mengatur nilai yang menunjukkan apakah bidang khusus didefinisikan pengguna. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Mengatur cara daftar nilai diurutkan. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Menambahkan nilai ke daftar lookup internal. Ini adalah cara yang lebih disarankan untuk manipulasi dengan `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Gunakan kode ini untuk menambahkan Nilai baru ke daftar lookup:
&gt; ``````

taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to add into lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### compareTo(ExtendedAttributeDefinition o) {#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public int compareTo(ExtendedAttributeDefinition o)
```


Compares this object with another instance of the @\{code ExtendedAttributeDefinition\} class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | the object to be compared. |

**Returns:**
int - a negative integer, zero, or a positive integer as this object is less than, equal to, or greater than the specified object.
### createExtendedAttribute() {#createExtendedAttribute--}
```
public final ExtendedAttribute createExtendedAttribute()
```


Creates a new extended attribute with the field ID which equals to this object's field ID value.

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(boolean flagValue) {#createExtendedAttribute-boolean-}
```
public final ExtendedAttribute createExtendedAttribute(boolean flagValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | boolean | The specified flag value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Duration durationValue) {#createExtendedAttribute-com.aspose.tasks.Duration-}
```
public final ExtendedAttribute createExtendedAttribute(Duration durationValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | The specified duration value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Value lookupValue) {#createExtendedAttribute-com.aspose.tasks.Value-}
```
public final ExtendedAttribute createExtendedAttribute(Value lookupValue)
```


Creates new extended attribute linked with specified [Value](../../com.aspose.tasks/value) item.

--------------------

&gt; ```
&gt; Use this code to create new [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) using specific value:
&gt; ``````

 taskTextAttr.addLookupValue(value1);
 taskTextAttr.addLookupValue(value2);
 ExtendedAttribute extendedAttribute = taskTextAttr.createExtendedAttribute(value2);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | Item [Value](../../com.aspose.tasks/value) yang ditentukan. |

--------------------

`lookupValue` harus sebelumnya ditambahkan ke [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) menggunakan metode [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) . |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai teks yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| textValue | java.lang.String | Nilai teks yang ditentukan. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai numerik yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | Nilai numerik yang ditentukan. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Membuat atribut ekstended baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dateTimeValue | java.util.Date | Nilai datetime yang ditentukan. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Metode pabrik yang membuat definisi atribut ekstended dengan lookup. Ia memiliki `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) sama dengan [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) dan hanya dapat digunakan pada Resources. Anda harus menentukan `customFieldType`, `fieldId`, dan `alias` saat memanggil metode ini.

--------------------

&gt; ```
&gt; Gunakan contoh ini untuk membuat definisi bidang khusus untuk sumber daya dengan lookup dan kemudian mengisinya dengan nilai teks:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupResourceDefinition(int fieldId, String alias) {#createLookupResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Resources only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a resource with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(1);
         this.setVal("Text value 1");
         this.setDescription("Text value description 1");
     }});
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(2);
         this.setVal("Text value 2");
         this.setDescription("Text value description 2");
     }});
     project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | int | ID bidang [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) yang ditentukan. |
| alias | java.lang.String | String alias yang ditentukan. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Metode pabrik yang membuat definisi atribut tambahan dengan lookup. Ia memiliki `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) yang sama dengan [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) dan hanya dapat digunakan pada Tasks. Anda harus menentukan `customFieldType`, `fieldId`, dan `alias` saat memanggil metode ini.

--------------------

&gt; ```
&gt; Gunakan contoh ini untuk membuat definisi bidang khusus untuk tugas dengan lookup dan kemudian mengisinya dengan nilai teks:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupTaskDefinition(int fieldId, String alias) {#createLookupTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a task with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(1);
     this.setVal("Text value 1");
     this.setDescription("Text value description 1");
 }});
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(2);
     this.setVal("Text value 2");
     this.setDescription("Text value description 2");
 }});
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | int | ID bidang [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) yang ditentukan. |
| alias | java.lang.String | String alias yang ditentukan. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "None". Ia memiliki `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) yang sama dengan [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) dan hanya dapat digunakan pada Resource. Anda harus menentukan `customFieldType`, `fieldId`, dan `alias` saat memanggil metode ini.

--------------------

&gt; ```
&gt; Gunakan contoh ini untuk membuat definisi bidang teks khusus:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createResourceDefinition(int fieldId, String alias) {#createResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Resource only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
 project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | int | ID bidang [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) yang ditentukan. |
| alias | java.lang.String | String alias yang ditentukan. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "None". Ia memiliki `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) yang sama dengan [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) dan hanya dapat digunakan pada Tasks. Anda harus menentukan `customFieldType`, `fieldId`, dan `alias` saat memanggil metode ini.

--------------------

&gt; ```
&gt; Gunakan contoh ini untuk membuat definisi bidang teks khusus:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createTaskDefinition(int fieldId, String alias) {#createTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when calling this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fieldId | int | ID bidang [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) yang ditentukan. |
| alias | java.lang.String | String alias yang ditentukan. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | objek yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - sebuah flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Mendapatkan alias dari bidang khusus.

**Returns:**
java.lang.String - alias dari bidang khusus.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Mendapatkan nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar.

--------------------

Saat ini didukung untuk format MSP 2003/2007 Xml dan MSP 2003 mpp.

**Returns:**
boolean - nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Mendapatkan nilai yang menunjukkan apakah roll down otomatis ke penugasan diaktifkan.

**Returns:**
boolean - nilai yang menunjukkan apakah roll down otomatis ke penugasan diaktifkan.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Mendapatkan tipe perhitungan nilai atribut khusus.

**Returns:**
int - tipe perhitungan nilai atribut khusus.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Mendapatkan tipe dari bidang khusus.

**Returns:**
int - tipe dari bidang khusus.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Mendapatkan nilai default dalam daftar.

--------------------

Saat ini didukung untuk format MSP 2003/2007 Xml dan MSP 2003 mpp.

**Returns:**
java.lang.String - nilai default dalam daftar.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Mendapatkan Guid dari entri tabel lookup default.

**Returns:**
java.lang.String - Guid dari entri tabel lookup default.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Mendapatkan atribut ekstended yang terkait dengan tugas, sumber daya, atau penugasan.

**Returns:**
int - atribut yang diperluas terkait dengan tugas, sumber daya, atau penugasan.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets sesuai dengan id proyek dari bidang khusus. Gunakan representasi string dari konstanta dari kelas [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) untuk menentukan properti `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)).

--------------------

&gt; ```
&gt;
&gt; ``````

customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Preferable way to set `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property is to create [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) using one of the dedicated factory methods like [createTaskDefinition(int, String)](../../com.aspose.tasks/extendedattributedefinition\#createTaskDefinition-int--String-) or [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Returns:**
java.lang.String - corresponds to the project id of a custom field.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the name of a custom field.

--------------------

Should not be set directly, instead create ExtendedAttributeDefinition using strongly typed static factory methods named like create\*Definition().

**Returns:**
java.lang.String - the name of a custom field.
### getFormula() {#getFormula--}
```
public final String getFormula()
```


Gets the formula that Microsoft Project uses to populate a custom task field.

**Returns:**
java.lang.String - the formula that Microsoft Project uses to populate a custom task field.
### getGraphicalIndicator() {#getGraphicalIndicator--}
```
public final GraphicalIndicatorsInfo getGraphicalIndicator()
```


Gets a graphical indicators info associated with the extended attribute. Applicable to MPP format.

**Returns:**
[GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) - a graphical indicators info associated with the extended attribute.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets the Guid of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the Guid of a custom field.
### getLookupUid() {#getLookupUid--}
```
public final String getLookupUid()
```


Gets a Guid of the lookup table associated with a custom field.

--------------------

In order to create a custom field with lookup, use one of the factory methods: [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) or [createLookupResourceDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupResourceDefinition-int--int--String-).

**Returns:**
java.lang.String - a Guid of the lookup table associated with a custom field.
### getMaxMultiValues() {#getMaxMultiValues--}
```
public final int getMaxMultiValues()
```


Gets the maximum number of values you can set in a pick list.

--------------------

Currently supported for Xml format only.

**Returns:**
int - the maximum number of values you can set in a pick list.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.
### getPhoneticsAlias() {#getPhoneticsAlias--}
```
public final String getPhoneticsAlias()
```


Gets the phonetic pronunciation of the alias of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the phonetic pronunciation of the alias of a custom field.
### getRestrictValues() {#getRestrictValues--}
```
public final boolean getRestrictValues()
```


Gets a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Returns:**
boolean - a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).
### getRollupType() {#getRollupType--}
```
public final int getRollupType()
```


Gets the way rollups are calculated.

--------------------

Writing currently supported for Xml format only.

**Returns:**
int - the way rollups are calculated.
### getSecondaryGuid() {#getSecondaryGuid--}
```
public final String getSecondaryGuid()
```


Gets the secondary guid of extended attribute.

--------------------

This is new for MS Project 2010 property.

**Returns:**
java.lang.String - the secondary guid of extended attribute.
### getSecondaryPid() {#getSecondaryPid--}
```
public final String getSecondaryPid()
```


Gets the secondary PID of a custom field.

**Returns:**
java.lang.String - the secondary PID of a custom field.
### getSummaryRowsCalculationType() {#getSummaryRowsCalculationType--}
```
public final int getSummaryRowsCalculationType()
```


Gets the type of calculation of the custom attribute's value for summary rows.

**Returns:**
int - the type of calculation of the custom attribute's value for summary rows.
### getUserDef() {#getUserDef--}
```
public final boolean getUserDef()
```


Gets a value indicating whether a custom field is user defined.

--------------------

Currently supported for Xml format only.

**Returns:**
boolean - a value indicating whether a custom field is user defined.
### getValueList() {#getValueList--}
```
public final List<Value> getValueList()
```


Gets the List&lt;Value&gt; ValueList.

--------------------

When values of extended attributes are specified as properties of elements in the schema, they may either be specified by values or by references to the values contained in this list. Applications may assume ordering of the list by ordering specified here. Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats. Do not change this list directly. Use ExtendedAttributeDefinition.addLookupValue/removeLookupValue methods instead.

**Returns:**
java.util.List&lt;com.aspose.tasks.Value&gt; - the List&lt;Value&gt; ValueList.
### getValuelistSortOrder() {#getValuelistSortOrder--}
```
public final int getValuelistSortOrder()
```


Gets the way value lists are sorted. Values are: 0=Descending, 1=Ascending.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Returns:**
int - the way value lists are sorted.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class.

**Returns:**
int - a hash code for this object.
### removeLookupValue(Value value) {#removeLookupValue-com.aspose.tasks.Value-}
```
public final void removeLookupValue(Value value)
```


Removes a value from the internal lookup list. This is a preferable way for manipulations with the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to remove from lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Sets the alias of a custom field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the alias of a custom field. |

### setAppendNewValues(boolean value) {#setAppendNewValues-boolean-}
```
public final void setAppendNewValues(boolean value)
```


Sets a value indicating whether new values added to a project are automatically added to the list.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether new values added to a project are automatically added to the list. |

### setAutoRollDown(boolean value) {#setAutoRollDown-boolean-}
```
public final void setAutoRollDown(boolean value)
```


Sets a value indicating whether an automatic roll down to assignments is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether an automatic roll down to assignments is enabled. |

### setCalculationType(int value) {#setCalculationType-int-}
```
public final void setCalculationType(int value)
```


Sets the type of calculation of the custom attribute's value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of calculation of the custom attribute's value. |

### setDefault(String value) {#setDefault-java.lang.String-}
```
public final void setDefault(String value)
```


Sets the default value in the list.

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default value in the list. |

### setDefaultGuid(String value) {#setDefaultGuid-java.lang.String-}
```
public final void setDefaultGuid(String value)
```


Sets the Guid of the default lookup table entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Guid of the default lookup table entry. |

### setElementType(int value) {#setElementType-int-}
```
public final void setElementType(int value)
```


Sets the extended attribute is associated with a task, a resource or an assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the extended attribute is associated with a task, a resource or an assignment. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets corresponds to the project id of a custom field. Use string representation of a constant from [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) class to specify `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property.

--------------------

&gt; ```
&gt; 
&gt; ``````

 customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Cara yang disarankan untuk mengatur `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) properti adalah dengan membuat [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) menggunakan salah satu metode pabrik khusus seperti [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) atau [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | mengacu pada id proyek dari bidang khusus. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Mengatur formula yang digunakan Microsoft Project untuk mengisi bidang tugas khusus.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | rumus yang digunakan Microsoft Project untuk mengisi bidang tugas khusus. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Mengatur informasi indikator grafis yang terkait dengan atribut ekstensi. Berlaku untuk format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | informasi indikator grafis yang terkait dengan atribut ekstensi. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Mengatur Guid dari bidang khusus.

--------------------

Saat ini hanya didukung untuk format Xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Guid dari bidang khusus. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Mengatur jumlah maksimum nilai yang dapat Anda atur dalam daftar pilihan.

--------------------

Saat ini hanya didukung untuk format Xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah maksimum nilai yang dapat Anda atur dalam daftar pilihan. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Mengatur pelafalan fonetik alias dari bidang khusus.

--------------------

Saat ini hanya didukung untuk format Xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | pelafalan fonetik alias dari bidang khusus. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Mengatur nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Mengatur cara perhitungan rollup.

--------------------

Penulisan saat ini hanya didukung untuk format Xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | cara perhitungan rollup. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Mengatur guid sekunder dari atribut ekstended.

--------------------

Ini baru untuk properti MS Project 2010.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | guid sekunder dari atribut ekstensi. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Mengatur PID sekunder dari bidang khusus.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | PID sekunder dari bidang khusus. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Mengatur jenis perhitungan nilai atribut khusus untuk baris ringkasan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe perhitungan nilai atribut khusus untuk baris ringkasan. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Mengatur nilai yang menunjukkan apakah bidang khusus didefinisikan pengguna.

--------------------

Saat ini hanya didukung untuk format Xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah bidang khusus didefinisikan pengguna. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Mengatur cara daftar nilai diurutkan. Nilai: 0=Menurun, 1=Naik.

--------------------

Saat ini didukung untuk format MSP 2003/2007 Xml dan MSP 2003 mpp.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | cara daftar nilai diurutkan. |

