---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "PDF एन्क्रिप्शन के विवरण शामिल करता है।"
type: docs
weight: 189
url: /hi/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

PDF एन्क्रिप्शन के विवरण शामिल करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | एक नया उदाहरण प्रारंभ करता है [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) वर्ग का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | एन्क्रिप्शन मोड प्राप्त करता है। |
| [getOwnerPassword()](#getOwnerPassword--) | Owner पासवर्ड प्राप्त करता है। |
| [getPermissions()](#getPermissions--) | अनुमतियों को प्राप्त करता है। |
| [getUserPassword()](#getUserPassword--) | User पासवर्ड प्राप्त करता है। |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | एन्क्रिप्शन मोड सेट करता है। |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Owner पासवर्ड सेट करता है। |
| [setPermissions(int value)](#setPermissions-int-) | अनुमतियों को सेट करता है। |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | User पासवर्ड सेट करता है। |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


एक नया उदाहरण प्रारंभ करता है [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) वर्ग का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| userPassword | java.lang.String | उपयोगकर्ता पासवर्ड जो संरक्षित दस्तावेज़ खोलने की अनुमति देता है। |
| ownerPassword | java.lang.String | मालिक पासवर्ड जो संरक्षित दस्तावेज़ खोलने की अनुमति देता है। |
| encryptionAlgorithm | int | वह [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) उदाहरण जो एन्क्रिप्शन एल्गोरिद्म दर्शाता है। |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


एन्क्रिप्शन मोड प्राप्त करता है।

**Returns:**
int - एन्क्रिप्शन मोड।
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Owner पासवर्ड प्राप्त करता है।

--------------------

सही मालिक पासवर्ड के साथ दस्तावेज़ खोलना (मान लेते हुए कि यह उपयोगकर्ता पासवर्ड के समान नहीं है) दस्तावेज़ तक पूर्ण (मालिक) पहुँच की अनुमति देता है। यह असीमित पहुँच दस्तावेज़\\u2019 के पासवर्ड और पहुँच अनुमतियों को बदलने की क्षमता को शामिल करती है।

**Returns:**
java.lang.String - Owner पासवर्ड।
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


अनुमतियों को प्राप्त करता है।

**Returns:**
int - अनुमतियाँ।
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


User पासवर्ड प्राप्त करता है।

--------------------

सही उपयोगकर्ता पासवर्ड के साथ दस्तावेज़ खोलना (या ऐसे दस्तावेज़ को खोलना जिसमें उपयोगकर्ता पासवर्ड नहीं है) उपयोगकर्ता पहुँच अनुमतियों के अनुसार अतिरिक्त कार्यों को करने की अनुमति देता है जो दस्तावेज़\\u2019s एन्क्रिप्शन शब्दकोश में निर्दिष्ट हैं।

**Returns:**
java.lang.String - उपयोगकर्ता पासवर्ड।
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


एन्क्रिप्शन मोड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एन्क्रिप्शन मोड। |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Owner पासवर्ड सेट करता है।

--------------------

सही मालिक पासवर्ड के साथ दस्तावेज़ खोलना (मान लेते हुए कि यह उपयोगकर्ता पासवर्ड के समान नहीं है) दस्तावेज़ तक पूर्ण (मालिक) पहुँच की अनुमति देता है। यह असीमित पहुँच दस्तावेज़\\u2019 के पासवर्ड और पहुँच अनुमतियों को बदलने की क्षमता को शामिल करती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | मालिक पासवर्ड। |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


अनुमतियों को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | अनुमतियाँ। |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


User पासवर्ड सेट करता है।

--------------------

सही उपयोगकर्ता पासवर्ड के साथ दस्तावेज़ खोलना (या ऐसे दस्तावेज़ को खोलना जिसमें उपयोगकर्ता पासवर्ड नहीं है) उपयोगकर्ता पहुँच अनुमतियों के अनुसार अतिरिक्त कार्यों को करने की अनुमति देता है जो दस्तावेज़\\u2019s एन्क्रिप्शन शब्दकोश में निर्दिष्ट हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | उपयोगकर्ता पासवर्ड। |

