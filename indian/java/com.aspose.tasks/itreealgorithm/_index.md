---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक एल्गोरिद्म को दर्शाता है जिसे ऑब्जेक्ट्स T के ट्री पर लागू किया जा सकता है।"
type: docs
weight: 384
url: /hi/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

`T` ऑब्जेक्ट्स के पेड़ पर लागू किया जा सकने वाला एल्गोरिद्म दर्शाता है।

T : मेथड इंटरफ़ेस लागू करने के लिए ऑब्जेक्ट का प्रकार।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | एक पेड़ की नोड को प्रोसेस करता है। |
| [postAlg(T el, int level)](#postAlg-T-int-) | एक पेड़ की नोड को प्रोसेस करने के बाद बुलाया जाता है। |
| [preAlg(T el, int level)](#preAlg-T-int-) | एक पेड़ की नोड को प्रोसेस करने से पहले बुलाया जाता है। |
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
public abstract void postAlg(T el, int level)
```


एक पेड़ की नोड को प्रोसेस करने के बाद बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रसंस्करण के लिए नोड। |
| स्तर | int | ट्री नोड स्तर। |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


एक पेड़ की नोड को प्रोसेस करने से पहले बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रसंस्करण के लिए नोड। |
| स्तर | int | ट्री नोड स्तर। |

