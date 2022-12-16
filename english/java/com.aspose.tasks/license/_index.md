---
title: License
second_title: Aspose.Tasks for Java API Reference
description: Provides methods to license the component.
type: docs
weight: 134
url: /java/com.aspose.tasks/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Provides methods to license the component.

--------------------

&gt; ```
&gt; In this example, an attempt will be made to find a license file named MyLicense.lic
&gt;   in the folder that contains
&gt;   
&gt;   the component, in the folder that contains the calling assembly,
&gt;   in the folder of the entry assembly and then in the embedded resources of the calling assembly.
&gt;   ```
&gt; 
&gt;   [C#]
&gt; 
&gt;   License license = new License();
&gt;   license.SetLicense("MyLicense.lic");
&gt;   [Visual Basic]
&gt;   Dim license As license = New license
&gt;   License.SetLicense("MyLicense.lic")
&gt;   
&gt; ```
&gt;   
&gt;   
&gt;   the component jar file:
&gt;   ```
&gt; 
&gt;   License license = new License();
&gt;   license.setLicense("MyLicense.lic");
&gt;   
&gt; ```
&gt; ```
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
&gt;  
&gt;  the component, in the folder that contains the calling assembly,
&gt;  in the folder of the entry assembly and then in the embedded resources of the calling assembly.
&gt;  ```
&gt; 
&gt;  [C#]
&gt;  License license = new License();
&gt;  license.SetLicense("MyLicense.lic");
&gt;  [Visual Basic]
&gt;  Dim license As license = New license
&gt;  License.SetLicense("MyLicense.lic")
&gt;  
&gt; ```
&gt;  
&gt;  
&gt;  the component jar file:
&gt;  ```
&gt; 
&gt;  License license = new License();
&gt;  license.setLicense("MyLicense.lic");
&gt;  
&gt; ```
&gt; ```

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseFile | java.io.File | representation of file pathname |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Licenses the component.

--------------------

&gt; ```
&gt; ```
&gt; 
&gt;  
&gt;  [C#]
&gt;  License license = new License();
&gt;  license.SetLicense(myStream);
&gt;  [Visual Basic]
&gt;  Dim license as License = new License
&gt;  license.SetLicense(myStream)
&gt;  
&gt;  
&gt;  License license = new License();
&gt;  license.setLicense(myStream);
&gt;  
&gt;  
&gt; ```
&gt; ```

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

 License license = new License();
 license.setLicense("MyLicense.lic");
 
```

--------------------

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | java.lang.String | Can be a full or short file name or name of an embedded resource. Use an empty string to switch to evaluation mode. |
