---
title: "رخصة"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يوفر طرقًا لترخيص المكوّن."
type: docs
weight: 145
url: /ar/java/com.aspose.tasks/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

يوفر طرقًا لترخيص المكوّن.

--------------------

&gt; ```
&gt; في هذا المثال، سيتم محاولة العثور على ملف ترخيص باسم MyLicense.lic
&gt;   في المجلد الذي يحتوي على
&gt;   ملف jar للمكوّن:
&gt; ``````

License license = new License();
license.setLicense("MyLicense.lic");
  
```


## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of the [License](../../com.aspose.tasks/license) class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Initializes a new instance of the [License](../../com.aspose.tasks/license) class.

--------------------

&gt; ```
&gt; In this example, an attempt will be made to find a license file named MyLicense.lic
&gt;  in the folder that contains
&gt;  the component jar file:
&gt; ``````

 License license = new License();
 license.setLicense("MyLicense.lic");
 
```



### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


يرخص المكوّن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| licenseFile | java.io.File | تمثيل مسار اسم الملف |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


يرخص المكوّن.

--------------------

&gt; ```
&gt;
&gt; ``````

License license = new License();
license.setLicense(myStream);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A stream that contains the license. |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licenses the component.

Library tries to find the license in the following locations:

1. Explicit path.

2. The folder that contains the Aspose component JAR file.

3. The folder that contains the client's calling JAR file.

--------------------

In this example, an attempt will be made to find a license file named MyLicense.lic in locations listed above:

```

``````

 License license = new License();
 license.setLicense("MyLicense.lic");
 
```

--------------------

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| licenseName | java.lang.String | يمكن أن يكون اسم ملف كامل أو قصير أو اسم مورد مضمّن. استخدم سلسلة فارغة للتبديل إلى وضع التقييم. |

