---
title: "StringBuilder"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक परिवर्तनीय अक्षर स्ट्रिंग का प्रतिनिधित्व करता है।"
type: docs
weight: 281
url: /hi/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

एक परिवर्तनीय अक्षर स्ट्रिंग का प्रतिनिधित्व करता है। इसे विस्तारित नहीं किया जा सकता।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
| [StringBuilder(int capacity)](#StringBuilder-int-) | निर्दिष्ट क्षमता का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | निर्दिष्ट क्षमता से शुरू होने और निर्दिष्ट अधिकतम तक बढ़ने वाली StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | निर्दिष्ट स्ट्रिंग का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | निर्दिष्ट स्ट्रिंग और क्षमता का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | निर्दिष्ट उपस्ट्रिंग और क्षमता से StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [append(boolean value)](#append-boolean-) | निर्दिष्ट बूलियन मान का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(byte value)](#append-byte-) | निर्दिष्ट बाइट का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(char value)](#append-char-) | निर्दिष्ट यूनिकोड अक्षर का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(char value, int repeatCount)](#append-char-int-) | एक यूनिकोड अक्षर के स्ट्रिंग प्रतिनिधित्व की निर्दिष्ट संख्या की प्रतियों को इस इंस्टेंस में जोड़ता है। |
| [append(char[] value)](#append-char---) | निर्दिष्ट एरे में यूनिकोड अक्षरों का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | निर्दिष्ट उपएरे में यूनिकोड अक्षरों का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(double value)](#append-double-) | निर्दिष्ट डबल संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(float value)](#append-float-) | निर्दिष्ट फ़्लोट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(int value)](#append-int-) | निर्दिष्ट इंट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(Object value)](#append-java.lang.Object-) | निर्दिष्ट ऑब्जेक्ट का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(String value)](#append-java.lang.String-) | निर्दिष्ट स्ट्रिंग की एक प्रति इस इंस्टेंस में जोड़ता है। |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | निर्दिष्ट उपस्ट्रिंग की एक प्रति इस इंस्टेंस में जोड़ता है। |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | निर्दिष्ट बिगडेसिमल संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(long value)](#append-long-) | निर्दिष्ट लाँग संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [append(short value)](#append-short-) | निर्दिष्ट शॉर्ट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है। |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | कम्पोज़िट फ़ॉर्मेट स्ट्रिंग को प्रोसेस करके प्राप्त स्ट्रिंग, जिसमें शून्य या अधिक फ़ॉर्मेट आइटम हो सकते हैं, इस इंस्टेंस में जोड़ता है। |
| [appendLine()](#appendLine--) | डिफ़ॉल्ट लाइन टर्मिनेटर को वर्तमान StringBuilder ऑब्जेक्ट के अंत में जोड़ता है। |
| [appendLine(String value)](#appendLine-java.lang.String-) | निर्दिष्ट स्ट्रिंग की एक कॉपी, उसके बाद डिफ़ॉल्ट लाइन टर्मिनेटर, को वर्तमान StringBuilder ऑब्जेक्ट के अंत में जोड़ता है। |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | इस इंस्टेंस के निर्दिष्ट खंड से अक्षरों को गंतव्य Char एरे के निर्दिष्ट खंड में कॉपी करता है। |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | सुनिश्चित करता है कि इस StringBuilder इंस्टेंस की क्षमता कम से कम निर्दिष्ट मान हो। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getCapacity()](#getCapacity--) | वर्तमान इंस्टेंस द्वारा आवंटित मेमोरी में रखे जा सकने वाले अधिकतम अक्षरों की संख्या प्राप्त करता है। |
| [getLength()](#getLength--) | वर्तमान StringBuilder ऑब्जेक्ट की लंबाई प्राप्त करता है। |
| [getMaxCapacity()](#getMaxCapacity--) | इस इंस्टेंस की अधिकतम क्षमता प्राप्त करता है। |
| [hashCode()](#hashCode--) | इस StringBuilder के लिए एक हैश कोड लौटाता है। |
| [insert(int index, boolean value)](#insert-int-boolean-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में बूलियन मान का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, byte value)](#insert-int-byte-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में बाइट मान का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, char value)](#insert-int-char-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में निर्दिष्ट Unicode अक्षर का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, char[] value)](#insert-int-char---) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में Unicode अक्षरों की निर्दिष्ट एरे का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में Unicode अक्षरों के निर्दिष्ट सबएरे का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, double value)](#insert-int-double-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में डबल संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, float value)](#insert-int-float-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में फ़्लोट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, int value)](#insert-int-int-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में इंट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में ऑब्जेक्ट का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, String value)](#insert-int-java.lang.String-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में एक स्ट्रिंग डालता है। |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में निर्दिष्ट स्ट्रिंग की एक या अधिक कॉपी डालता है। |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में डेसिमल संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, long value)](#insert-int-long-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में लाँग संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [insert(int index, short value)](#insert-int-short-) | निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में शॉर्ट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है। |
| [remove(int startIndex, int length)](#remove-int-int-) | इस उदाहरण से निर्दिष्ट अक्षरों की सीमा को हटाता है। |
| [replace(char oldChar, char newChar)](#replace-char-char-) | इस उदाहरण में निर्दिष्ट अक्षर की सभी घटनाओं को दूसरे निर्दिष्ट अक्षर से बदलता है। |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | इस उदाहरण के उपस्ट्रिंग के भीतर, निर्दिष्ट अक्षर की सभी घटनाओं को दूसरे निर्दिष्ट अक्षर से बदलता है। |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | इस उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को दूसरे निर्दिष्ट स्ट्रिंग से बदलता है। |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | इस उदाहरण के उपस्ट्रिंग के भीतर, निर्दिष्ट स्ट्रिंग की सभी घटनाओं को दूसरे निर्दिष्ट स्ट्रिंग से बदलता है। |
| [setCapacity(int value)](#setCapacity-int-) | वर्तमान उदाहरण द्वारा आवंटित मेमोरी में समाहित किए जा सकने वाले अधिकतम अक्षरों की संख्या सेट करता है। |
| [setLength(int value)](#setLength-int-) | वर्तमान StringBuilder ऑब्जेक्ट की लंबाई सेट करता है। |
| [toString()](#toString--) | इस उदाहरण के मान को स्ट्रिंग में परिवर्तित करता है। |
| [toString(int startIndex, int length)](#toString-int-int-) | इस उदाहरण के उपस्ट्रिंग के मान को स्ट्रिंग में परिवर्तित करता है। |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


निर्दिष्ट क्षमता का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्षमता | int | इस उदाहरण का सुझाया गया प्रारंभिक आकार। |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


निर्दिष्ट क्षमता से शुरू होने और निर्दिष्ट अधिकतम तक बढ़ने वाली StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्षमता | int | StringBuilder का सुझाया गया प्रारंभिक आकार। |
| अधिकतमक्षमता | int | वर्तमान स्ट्रिंग में समाहित किए जा सकने वाले अधिकतम अक्षरों की संख्या। |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


निर्दिष्ट स्ट्रिंग का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | उदाहरण के मान को आरंभ करने के लिए उपयोग की गई स्ट्रिंग। |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


निर्दिष्ट स्ट्रिंग और क्षमता का उपयोग करके StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | उदाहरण के मान को आरंभ करने के लिए उपयोग की गई स्ट्रिंग। |
| क्षमता | int | StringBuilder का सुझाया गया प्रारंभिक आकार। |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


निर्दिष्ट उपस्ट्रिंग और क्षमता से StringBuilder वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | उदाहरण के मान को आरंभ करने के लिए उपयोग किए गए उपस्ट्रिंग को शामिल करने वाली स्ट्रिंग। |
| startIndex | int | मान के भीतर वह स्थिति जहाँ उपस्ट्रिंग शुरू होती है। |
| length | int | उपस्ट्रिंग में अक्षरों की संख्या। |
| क्षमता | int | StringBuilder का सुझाया गया प्रारंभिक आकार। |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


निर्दिष्ट बूलियन मान का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | जोड़ने के लिए बूलियन मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


निर्दिष्ट बाइट का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | byte | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


निर्दिष्ट यूनिकोड अक्षर का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | char | जोड़ने के लिए यूनिकोड अक्षर। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


एक यूनिकोड अक्षर के स्ट्रिंग प्रतिनिधित्व की निर्दिष्ट संख्या की प्रतियों को इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | char | जोड़ने के लिए अक्षर। |
| repeatCount | int | मान को जोड़ने की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


निर्दिष्ट एरे में यूनिकोड अक्षरों का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | char[] | जोड़ने के लिए अक्षरों की सरणी। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


निर्दिष्ट उपएरे में यूनिकोड अक्षरों का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | char[] | एक अक्षर सरणी। |
| startIndex | int | मान में प्रारंभिक स्थिति। |
| charCount | int | जोड़ने के लिए अक्षरों की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


निर्दिष्ट डबल संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


निर्दिष्ट फ़्लोट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | float | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


निर्दिष्ट इंट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


निर्दिष्ट ऑब्जेक्ट का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.Object | जोड़ने के लिए वस्तु। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


निर्दिष्ट स्ट्रिंग की एक प्रति इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | जोड़ने के लिए स्ट्रिंग। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


निर्दिष्ट उपस्ट्रिंग की एक प्रति इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | स्ट्रिंग जिसमें जोड़ने के लिए उपस्ट्रिंग है। |
| startIndex | int | मान के भीतर उपस्ट्रिंग की प्रारंभिक स्थिति। |
| count | int | मान में जोड़ने के लिए अक्षरों की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


निर्दिष्ट बिगडेसिमल संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


निर्दिष्ट लाँग संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | long | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


निर्दिष्ट शॉर्ट संख्या का स्ट्रिंग प्रतिनिधित्व इस इंस्टेंस में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | short | जोड़ने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


संयोजित फ़ॉर्मेट स्ट्रिंग को प्रोसेस करके प्राप्त स्ट्रिंग को इस इंस्टेंस में जोड़ता है, जिसमें शून्य या अधिक फ़ॉर्मेट आइटम हो सकते हैं। प्रत्येक फ़ॉर्मेट आइटम को पैरामीटर एरे में संबंधित तर्क के स्ट्रिंग प्रतिनिधित्व से बदल दिया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| format | java.lang.String | एक संयोजित फ़ॉर्मेट स्ट्रिंग। |
| args | java.lang.Object[] | फ़ॉर्मेट करने के लिए वस्तुओं की सरणी। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


डिफ़ॉल्ट लाइन टर्मिनेटर को वर्तमान StringBuilder ऑब्जेक्ट के अंत में जोड़ता है।

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


निर्दिष्ट स्ट्रिंग की एक कॉपी, उसके बाद डिफ़ॉल्ट लाइन टर्मिनेटर, को वर्तमान StringBuilder ऑब्जेक्ट के अंत में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | जोड़ने के लिए स्ट्रिंग। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


इस इंस्टेंस के निर्दिष्ट खंड से अक्षरों को गंतव्य Char एरे के निर्दिष्ट खंड में कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceIndex | int | इस इंस्टेंस में वह प्रारंभिक स्थिति जहाँ से अक्षर कॉपी किए जाएंगे। इंडेक्स शून्य-आधारित है। |
| destination | char[] | वह ऐरे जहाँ अक्षर कॉपी किए जाएंगे। |
| destinationIndex | int | गंतव्य में वह प्रारम्भिक स्थिति जहाँ अक्षर कॉपी किए जाएंगे। सूचकांक शून्य-आधारित है। |
| count | int | कॉपी किए जाने वाले अक्षरों की संख्या। |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


सुनिश्चित करता है कि इस StringBuilder इंस्टेंस की क्षमता कम से कम निर्दिष्ट मान हो।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्षमता | int | सुनिश्चित करने के लिए न्यूनतम क्षमता। |

**Returns:**
int - इस इंस्टेंस की नई क्षमता।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस के साथ तुलना करने के लिए एक ऑब्जेक्ट, या null। |

**Returns:**
boolean - true यदि इस इंस्टेंस और sb के स्ट्रिंग, Capacity, और MaxCapacity मान समान हों; अन्यथा false।
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


वर्तमान इंस्टेंस द्वारा आवंटित मेमोरी में रखे जा सकने वाले अधिकतम अक्षरों की संख्या प्राप्त करता है।

**Returns:**
int - वर्तमान इंस्टेंस द्वारा आवंटित मेमोरी में समाहित हो सकने वाले अक्षरों की अधिकतम संख्या।
### getLength() {#getLength--}
```
public int getLength()
```


वर्तमान StringBuilder ऑब्जेक्ट की लंबाई प्राप्त करता है।

**Returns:**
int - इस इंस्टेंस की लंबाई।
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


इस इंस्टेंस की अधिकतम क्षमता प्राप्त करता है।

**Returns:**
int - इस इंस्टेंस द्वारा धारण की जा सकने वाली अक्षरों की अधिकतम संख्या।
### hashCode() {#hashCode--}
```
public int hashCode()
```


इस StringBuilder के लिए एक हैश कोड लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में बूलियन मान का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | boolean | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में बाइट मान का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | byte | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में निर्दिष्ट Unicode अक्षर का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | char | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में Unicode अक्षरों की निर्दिष्ट एरे का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | char[] | सम्मिलित करने के लिए अक्षर ऐरे। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में Unicode अक्षरों के निर्दिष्ट सबएरे का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | char[] | एक अक्षर सरणी। |
| startIndex | int | मान के भीतर प्रारम्भिक सूचकांक। |
| charCount | int | सम्मिलित करने वाले अक्षरों की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में डबल संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | double | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में फ़्लोट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | float | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में इंट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | int | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में ऑब्जेक्ट का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | java.lang.Object | सम्मिलित करने के लिए ऑब्जेक्ट, या null। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में एक स्ट्रिंग डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | java.lang.String | सम्मिलित करने के लिए स्ट्रिंग। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में निर्दिष्ट स्ट्रिंग की एक या अधिक कॉपी डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | java.lang.String | सम्मिलित करने के लिए स्ट्रिंग। |
| count | int | मान को सम्मिलित करने की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में डेसिमल संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | java.math.BigDecimal | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में लाँग संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | long | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


निर्दिष्ट अक्षर स्थिति पर इस इंस्टेंस में शॉर्ट संख्या का स्ट्रिंग प्रतिनिधित्व डालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | इस इंस्टेंस में जहाँ सम्मिलन शुरू होता है वह स्थिति। |
| मान | short | सम्मिलित करने के लिए मान। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


इस उदाहरण से निर्दिष्ट अक्षरों की सीमा को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| startIndex | int | इस इंस्टेंस में जहाँ हटाना शुरू होता है वह शून्य-आधारित स्थिति। |
| length | int | हटाने वाले अक्षरों की संख्या। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


इस उदाहरण में निर्दिष्ट अक्षर की सभी घटनाओं को दूसरे निर्दिष्ट अक्षर से बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldChar | char | बदलने के लिए अक्षर। |
| newChar | char | oldChar को बदलने वाला अक्षर। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


इस उदाहरण के उपस्ट्रिंग के भीतर, निर्दिष्ट अक्षर की सभी घटनाओं को दूसरे निर्दिष्ट अक्षर से बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldValue | char | बदलने के लिए अक्षर। |
| newValue | char | oldChar को बदलने वाला अक्षर। |
| startIndex | int | इस उदाहरण में वह स्थिति जहाँ उपस्ट्रिंग शुरू होती है। |
| count | int | उपस्ट्रिंग की लंबाई। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


इस उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को दूसरे निर्दिष्ट स्ट्रिंग से बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldValue | java.lang.String | बदलने के लिए स्ट्रिंग। |
| newValue | java.lang.String | oldValue को बदलने वाली स्ट्रिंग, या null। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


इस उदाहरण के उपस्ट्रिंग के भीतर, निर्दिष्ट स्ट्रिंग की सभी घटनाओं को दूसरे निर्दिष्ट स्ट्रिंग से बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldValue | java.lang.String | बदलने के लिए स्ट्रिंग। |
| newValue | java.lang.String | oldValue को बदलने वाली स्ट्रिंग, या null। |
| startIndex | int | इस उदाहरण में वह स्थिति जहाँ उपस्ट्रिंग शुरू होती है। |
| count | int | उपस्ट्रिंग की लंबाई। |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


वर्तमान उदाहरण द्वारा आवंटित मेमोरी में समाहित किए जा सकने वाले अधिकतम अक्षरों की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वर्तमान उदाहरण द्वारा आवंटित मेमोरी में समाहित हो सकने वाले अधिकतम अक्षरों की संख्या। |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


वर्तमान StringBuilder ऑब्जेक्ट की लंबाई सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | इस उदाहरण की लंबाई। |

### toString() {#toString--}
```
public String toString()
```


इस उदाहरण के मान को स्ट्रिंग में परिवर्तित करता है।

**Returns:**
java.lang.String - एक स्ट्रिंग जिसका मान इस उदाहरण के समान है।
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


इस उदाहरण के उपस्ट्रिंग के मान को स्ट्रिंग में परिवर्तित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| startIndex | int | इस उदाहरण में उपस्ट्रिंग की प्रारंभिक स्थिति। |
| length | int | उपस्ट्रिंग की लंबाई। |

**Returns:**
java.lang.String - एक स्ट्रिंग जिसका मान इस उदाहरण के निर्दिष्ट उपस्ट्रिंग के समान है।
