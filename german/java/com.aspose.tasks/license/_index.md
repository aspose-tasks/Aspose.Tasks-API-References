---
title: "Lizenz"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Methoden zur Lizenzierung der Komponente bereit."
type: docs
weight: 145
url: /de/java/com.aspose.tasks/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Stellt Methoden zur Lizenzierung der Komponente bereit.

--------------------

&gt; ```
&gt; In diesem Beispiel wird versucht, eine Lizenzdatei mit dem Namen MyLicense.lic zu finden.
&gt;   im Ordner, der enthält
&gt;   die Komponenten-Jar-Datei:
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


Lizenziert die Komponente.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| licenseFile | java.io.File | Darstellung des Dateipfads |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Lizenziert die Komponente.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| licenseName | java.lang.String | Kann ein voller oder kurzer Dateiname oder der Name einer eingebetteten Ressource sein. Verwenden Sie eine leere Zeichenkette, um in den Evaluierungsmodus zu wechseln. |

