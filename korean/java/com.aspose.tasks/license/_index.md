---
title: "라이선스"
second_title: "Aspose.Tasks for Java API Reference"
description: "구성 요소에 대한 라이선스를 부여하는 메서드를 제공합니다."
type: docs
weight: 145
url: /ko/java/com.aspose.tasks/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

구성 요소에 대한 라이선스를 부여하는 메서드를 제공합니다.

--------------------

&gt; ```
&gt; 이 예제에서는 MyLicense.lic이라는 라이선스 파일을 찾으려고 시도합니다.
&gt;   포함하는 폴더에
&gt;   구성 요소 jar 파일:
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


구성 요소에 라이선스를 적용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| licenseFile | java.io.File | 파일 경로 이름의 표현 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


구성 요소에 라이선스를 적용합니다.

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| licenseName | java.lang.String | 전체 파일 이름이거나 짧은 파일 이름, 또는 포함된 리소스의 이름일 수 있습니다. 빈 문자열을 사용하면 평가 모드로 전환됩니다. |

