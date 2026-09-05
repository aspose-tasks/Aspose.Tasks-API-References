---
title: "GlobalizationSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "परियोजनाओं की वैश्वीकरण सेटिंग्स का प्रतिनिधित्व करता है।"
type: docs
weight: 114
url: /hi/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

प्रोजेक्ट की ग्लोबलाइज़ेशन सेटिंग्स का प्रतिनिधित्व करता है।

परियोजना में culture-invariant लिटरल या फ़ॉर्मेट का उपयोग करना अनुशंसित तरीका है। हालांकि, यदि कोई परियोजना culture-specific लिटरल का उपयोग करती है, तो इस क्लास का उपयोग formula-calculation engine को उन लिटरलों को पार्स करने में मदद करने के लिए किया जा सकता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | फ़ॉर्मूला में उपयोग किए जाने वाले बूलियन 'false' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है। |
| [getFormulaDateNA()](#getFormulaDateNA--) | तारीख फ़ील्ड के फ़ॉर्मूला में उपयोग किए जाने वाले "NA" (खाली मान) लिटरल के लिए एक स्ट्रिंग प्राप्त करता है। |
| [getTrueLiteral()](#getTrueLiteral--) | फ़ॉर्मूला में उपयोग किए जाने वाले बूलियन 'true' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है। |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


फ़ॉर्मूला में उपयोग किए जाने वाले बूलियन 'false' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है।

**Returns:**
java.lang.String - एक स्ट्रिंग जो बूलियन 'false' लिटरल को फ़ॉर्मूला में उपयोग करती है।
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


तारीख फ़ील्ड के फ़ॉर्मूला में उपयोग किए जाने वाले "NA" (खाली मान) लिटरल के लिए एक स्ट्रिंग प्राप्त करता है।

**Returns:**
java.lang.String - "NA" (खाली मान) लिटरल जो डेट फ़ील्ड के फ़ॉर्मूला में उपयोग होता है।
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


फ़ॉर्मूला में उपयोग किए जाने वाले बूलियन 'true' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है।

**Returns:**
java.lang.String - एक स्ट्रिंग जो बूलियन 'true' लिटरल को फ़ॉर्मूला में उपयोग करती है।
