---
title: "RiskPattern"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "परियोजना कार्य के लिए जोखिम पैटर्न का प्रतिनिधित्व करता है।"
type: docs
weight: 268
url: /hi/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

परियोजना कार्य के लिए जोखिम पैटर्न का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | नया उदाहरण प्रारंभ करता है [RiskPattern](../../com.aspose/tasks/riskpattern) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | वास्तविक उत्पन्न मानों के आशावादी और निराशावादी अनुमान के भीतर रहने के समय प्रतिशत के अनुरूप विश्वास स्तर प्राप्त करता है। |
| [getDistribution()](#getDistribution--) | Monte Carlo सिमुलेशन में उपयोग किए गए प्रायिकता वितरण को प्राप्त करता है। |
| [getOptimistic()](#getOptimistic--) | सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है जो सर्वोत्तम संभव प्रोजेक्ट परिदृश्य में हो सकता है। |
| [getPessimistic()](#getPessimistic--) | सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है जो सबसे खराब संभव प्रोजेक्ट परिदृश्य में हो सकता है। |
| [getTask()](#getTask--) | इस जोखिम पैटर्न को लागू किया गया प्रोजेक्ट टास्क प्राप्त करता है। |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | वह विश्वास स्तर सेट करता है जो वास्तविक उत्पन्न मानों के समय प्रतिशत के अनुरूप होता है, जो आशावादी और निराशावादी अनुमान के भीतर होते हैं। |
| [setDistribution(int value)](#setDistribution-int-) | Monte Carlo सिमुलेशन में उपयोग किए जाने वाले प्रायिकता वितरण को सेट करता है। |
| [setOptimistic(int value)](#setOptimistic-int-) | सबसे संभावित कार्य अवधि का वह प्रतिशत सेट करता है जो सबसे बेहतर प्रोजेक्ट परिदृश्य में हो सकता है। |
| [setPessimistic(int value)](#setPessimistic-int-) | सबसे संभावित कार्य अवधि का वह प्रतिशत सेट करता है जो सबसे खराब प्रोजेक्ट परिदृश्य में हो सकता है। |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


नया उदाहरण प्रारंभ करता है [RiskPattern](../../com.aspose/tasks/riskpattern) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Monte Carlo सिमुलेशन में इस जोखिम को लागू किए जाने वाले निर्दिष्ट प्रोजेक्ट टास्क। |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


वास्तविक उत्पन्न मानों के समय प्रतिशत के अनुरूप विश्वास स्तर प्राप्त करता है, जो आशावादी और निराशावादी अनुमान के भीतर होते हैं। डिफ़ॉल्ट मान CL99 है।

--------------------

निम्नलिखित में से एक हो सकता है: `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeration.

**Returns:**
int - वह विश्वास स्तर जो वास्तविक उत्पन्न मानों के समय प्रतिशत के अनुरूप है, जो आशावादी और निराशावादी अनुमान के भीतर होते हैं।
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Monte Carlo सिमुलेशन में उपयोग किए जाने वाले प्रायिकता वितरण को प्राप्त करता है। डिफ़ॉल्ट मान ProbabilityDistributionType.Normal है।

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeration में परिभाषित मानों में से एक हो सकता है।

**Returns:**
int - Monte Carlo सिमुलेशन में उपयोग किया गया प्रायिकता वितरण।
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है जो सबसे बेहतर प्रोजेक्ट परिदृश्य में हो सकता है। डिफ़ॉल्ट मान 75 है, जिसका अर्थ है कि यदि अनुमानित निर्दिष्ट कार्य अवधि 4 दिन है तो आशावादी अवधि 3 दिन होगी।

**Returns:**
int - सबसे बेहतर प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत।
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है जो सबसे खराब प्रोजेक्ट परिदृश्य में हो सकता है। डिफ़ॉल्ट मान 125 है, जिसका अर्थ है कि यदि अनुमानित निर्दिष्ट कार्य अवधि 4 दिन है तो निराशावादी अवधि 5 दिन होगी।

**Returns:**
int - सबसे खराब प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत।
### getTask() {#getTask--}
```
public final Task getTask()
```


इस जोखिम पैटर्न को लागू किया गया प्रोजेक्ट टास्क प्राप्त करता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


वास्तविक उत्पन्न मानों के समय प्रतिशत के अनुरूप विश्वास स्तर सेट करता है, जो आशावादी और निराशावादी अनुमान के भीतर होते हैं। डिफ़ॉल्ट मान CL99 है।

--------------------

निम्नलिखित में से एक हो सकता है: `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeration.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वास्तविक उत्पन्न मानों के समय प्रतिशत के अनुरूप विश्वास स्तर। |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Monte Carlo सिमुलेशन में उपयोग किए जाने वाले प्रायिकता वितरण को सेट करता है। डिफ़ॉल्ट मान ProbabilityDistributionType.Normal है।

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeration में परिभाषित मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Monte Carlo सिमुलेशन में उपयोग किया गया प्रायिकता वितरण। |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


सबसे बेहतर प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत सेट करता है। डिफ़ॉल्ट मान 75 है, जिसका अर्थ है कि यदि अनुमानित निर्दिष्ट कार्य अवधि 4 दिन है तो आशावादी अवधि 3 दिन होगी।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | सबसे बेहतर प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत। |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


सबसे खराब प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत सेट करता है। डिफ़ॉल्ट मान 125 है, जिसका अर्थ है कि यदि अनुमानित निर्दिष्ट कार्य अवधि 4 दिन है तो निराशावादी अवधि 5 दिन होगी।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | सबसे खराब प्रोजेक्ट परिदृश्य में हो सकने वाली सबसे संभावित कार्य अवधि का प्रतिशत। |

