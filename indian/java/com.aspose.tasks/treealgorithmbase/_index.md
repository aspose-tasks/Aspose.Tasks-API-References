---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ITreeAlgorithmltTgt के कार्यान्वयन के लिए एक बेस क्लास।"
type: docs
weight: 327
url: /hi/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

ITreeAlgorithm&lt;T&gt; के कार्यान्वयन के लिए एक बेस क्लास।

T : तत्वों का प्रकार।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | एक पेड़ की नोड को प्रोसेस करता है। |
| [postAlg(T el, int level)](#postAlg-T-int-) | एक पेड़ की नोड को प्रोसेस करने के बाद बुलाया जाता है। |
| [preAlg(T el, int level)](#preAlg-T-int-) | एक पेड़ की नोड को प्रोसेस करने से पहले बुलाया जाता है। |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


एक पेड़ की नोड को प्रोसेस करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रसंस्करण के लिए नोड। |
| स्तर | int | ट्री नोड स्तर। |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


एक पेड़ की नोड को प्रोसेस करने के बाद बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रसंस्करण के लिए नोड। |
| स्तर | int | ट्री नोड स्तर। |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


एक पेड़ की नोड को प्रोसेस करने से पहले बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रसंस्करण के लिए नोड। |
| स्तर | int | ट्री नोड स्तर। |

