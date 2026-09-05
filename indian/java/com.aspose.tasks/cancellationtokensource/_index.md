---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "CancellationToken को संकेत देता है कि इसे रद्द किया जाना चाहिए।"
type: docs
weight: 47
url: /hi/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

`CancellationToken` को संकेत देता है कि इसे रद्द किया जाना चाहिए।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [cancel()](#cancel--) | रद्दीकरण के अनुरोध को संप्रेषित करता है। |
| [getToken()](#getToken--) | इस `CancellationTokenSource` से जुड़ा नया `CancellationToken` बनाता है। |
| [isCancellationRequested()](#isCancellationRequested--) | जाँचता है कि इस CancellationTokenSource के लिए रद्दीकरण का अनुरोध किया गया है या नहीं। |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


रद्दीकरण के अनुरोध को संप्रेषित करता है।

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


इस `CancellationTokenSource` से जुड़ा नया `CancellationToken` बनाता है।

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


जाँचता है कि इस CancellationTokenSource के लिए रद्दीकरण का अनुरोध किया गया है या नहीं।

**Returns:**
boolean - true, यदि रद्दीकरण का अनुरोध किया गया है; अन्यथा false।
