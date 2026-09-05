---
title: "CancellationToken"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "संचालन को रद्द करने की सूचना को प्रसारित करता है।"
type: docs
weight: 46
url: /hi/java/com.aspose.tasks/cancellationtoken/
---

**Inheritance:**
java.lang.Object
```
public class CancellationToken
```

संचालन को रद्द करने की सूचना को प्रसारित करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [isCancellationRequested()](#isCancellationRequested--) | प्राप्त करता है कि इस टोकन के लिए रद्दीकरण का अनुरोध किया गया है या नहीं। |
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


प्राप्त करता है कि इस टोकन के लिए रद्दीकरण का अनुरोध किया गया है या नहीं।

**Returns:**
boolean - true, यदि अंतर्निहित `CancellationTokenSource` के लिए रद्दीकरण का अनुरोध किया गया हो; अन्यथा false।
