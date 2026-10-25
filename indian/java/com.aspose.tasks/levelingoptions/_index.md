---
title: "LevelingOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "रिसोर्स लेवलिंग के पैरामीटर निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 142
url: /hi/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

रिसोर्स लेवलिंग के पैरामीटर निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | नए [LevelingOptions](../../com.aspose/tasks/levelingoptions) वर्ग का एक नया उदाहरण आरंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | एक टोकन प्राप्त करता है जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |
| [getFinishDate()](#getFinishDate--) | लेवलिंग अवधि की समाप्ति तिथि प्राप्त करता है। |
| [getLevelingOrder()](#getLevelingOrder--) | लेवलिंग एल्गोरिदम द्वारा अधिक आवंटन वाले कार्यों को विलंबित करने के क्रम को प्राप्त करता है। |
| [getMessageHandler()](#getMessageHandler--) | एक संदेश हैंडलर कॉलबैक प्राप्त करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को रोकने के लिए किया जा सकता है। |
| [getMessageLevel()](#getMessageLevel--) | Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों का स्तर प्राप्त करता है। |
| [getResources()](#getResources--) | लेवल किए जाने वाले संसाधनों की सूची प्राप्त करता है। |
| [getStartDate()](#getStartDate--) | लेवलिंग अवधि की प्रारंभ तिथि प्राप्त करता है। |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | एक टोकन सेट करता है जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | लेवलिंग अवधि की समाप्ति तिथि सेट करता है। |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | लेवलिंग एल्गोरिदम उन कार्यों को विलंबित करने का क्रम जिसमें अधिक आवंटन होते हैं। |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | ऐसे संदेश हैंडलर कॉलबैक को सेट करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है। |
| [setMessageLevel(int value)](#setMessageLevel-int-) | संसाधन लेवलिंग के दौरान Aspose.Tasks द्वारा उत्पन्न लॉग संदेशों का स्तर सेट करता है। |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | लेवल किए जाने वाले संसाधनों की सूची सेट करता है। |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | लेवलिंग अवधि की प्रारंभ तिथि सेट करता है। |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


नए [LevelingOptions](../../com.aspose/tasks/levelingoptions) वर्ग का एक नया उदाहरण आरंभ करता है।

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


एक टोकन प्राप्त करता है जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है।

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


लेवलिंग अवधि की समाप्ति तिथि प्राप्त करता है। डिफ़ॉल्ट मान प्रोजेक्ट की समाप्ति तिथि है।

**Returns:**
java.util.Date - लेवलिंग अवधि की समाप्ति तिथि।
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


लेवलिंग एल्गोरिदम उन कार्यों को विलंबित करने का क्रम प्राप्त करता है जिनमें अधिक आवंटन होते हैं। ओवरएलोकेशन का कारण बनने वाले कार्यों और जिन्हें विलंबित किया जा सकता है, का निर्धारण करने के बाद, निर्दिष्ट क्रम का उपयोग किया जाता है कि कौन सा कार्य पहले विलंबित किया जाना चाहिए।

**Returns:**
int - वह क्रम जिसमें लेवलिंग एल्गोरिदम अधिक आवंटन वाले कार्यों को विलंबित करता है।
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


एक संदेश हैंडलर कॉलबैक प्राप्त करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को रोकने के लिए किया जा सकता है।

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों का स्तर प्राप्त करता है।

**Returns:**
int - Aspose द्वारा उत्पन्न लॉग संदेशों का स्तर।
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


लेवल किए जाने वाले संसाधनों की सूची प्राप्त करता है। यदि null सेट किया जाता है, तो सभी प्रोजेक्ट संसाधनों को लेवल किया जाएगा।

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - लेवल किए जाने वाले संसाधनों की सूची।
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


लेवलिंग अवधि की प्रारंभ तिथि प्राप्त करता है। डिफ़ॉल्ट मान प्रोजेक्ट की प्रारंभ तिथि है।

**Returns:**
java.util.Date - लेवलिंग अवधि की प्रारंभ तिथि।
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


एक टोकन सेट करता है जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | एक टोकन जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


लेवलिंग अवधि की समाप्ति तिथि सेट करता है। डिफ़ॉल्ट मान प्रोजेक्ट की समाप्ति तिथि है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | लेवलिंग अवधि की समाप्ति तिथि। |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


लेवलिंग एल्गोरिदम उन कार्यों को विलंबित करने का क्रम जिसमें अधिक आवंटन होते हैं। ओवरएलोकेशन का कारण बनने वाले कार्यों और जिन्हें विलंबित किया जा सकता है, का निर्धारण करने के बाद, निर्दिष्ट क्रम का उपयोग किया जाता है कि कौन सा कार्य पहले विलंबित किया जाना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वह क्रम जिसमें लेवलिंग एल्गोरिदम अधिक आवंटन वाले कार्यों को विलंबित करता है। |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


ऐसे संदेश हैंडलर कॉलबैक को सेट करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | संदेश हैंडलर कॉलबैक जिसका उपयोग Aspose द्वारा उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है। |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


संसाधन लेवलिंग के दौरान Aspose.Tasks द्वारा उत्पन्न लॉग संदेशों का स्तर सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Aspose द्वारा उत्पन्न लॉग संदेशों का स्तर। |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


लेवल किए जाने वाले संसाधनों की सूची सेट करता है। यदि null सेट किया जाता है, तो सभी प्रोजेक्ट संसाधनों को लेवल किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.List&lt;com.aspose.tasks.Resource&gt; | लेवल किए जाने वाले संसाधनों की सूची। |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


लेवलिंग अवधि की प्रारंभ तिथि सेट करता है। डिफ़ॉल्ट मान प्रोजेक्ट की प्रारंभ तिथि है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | लेवलिंग अवधि की प्रारंभ तिथि। |

