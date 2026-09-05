---
title: "IAlgorithm"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक एल्गोरिद्म का प्रतिनिधित्व करता है जिसे वस्तुओं की सूची T पर लागू किया जा सकता है।"
type: docs
weight: 375
url: /hi/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

`T` ऑब्जेक्ट्स की सूची पर लागू किए जा सकने वाले एल्गोरिदम का प्रतिनिधित्व करता है।

T : मेथड इंटरफ़ेस लागू करने के लिए ऑब्जेक्ट का प्रकार।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | सूची में एक वस्तु को प्रोसेस करता है। |
| [postAlg(T el, int index)](#postAlg-T-int-) | एक वस्तु के प्रसंस्करण के बाद कॉल किया जाता है। |
| [preAlg(T el, int index)](#preAlg-T-int-) | एक वस्तु के प्रसंस्करण से पहले कॉल किया जाता है। |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


सूची में एक वस्तु को प्रोसेस करता है। इसके बाद कॉल किया जाता है [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस की गई वस्तु। |
| सूचकांक | int | वस्तु का सूचकांक। |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


एक वस्तु के प्रसंस्करण के बाद कॉल किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस की गई वस्तु। |
| सूचकांक | int | वस्तु का सूचकांक। |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


एक वस्तु के प्रसंस्करण से पहले कॉल किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस की गई वस्तु। |
| सूचकांक | int | वस्तु का सूचकांक। |

