---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "बहु‑पृष्ठ दस्तावेज़ में प्रत्येक पृष्ठ को अलग स्ट्रीम में सहेजा जाने पर कॉल किया जाने वाला कॉलबैक दर्शाता है।"
type: docs
weight: 382
url: /hi/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

बहु‑पृष्ठ दस्तावेज़ में प्रत्येक पृष्ठ को अलग स्ट्रीम में सहेजा जाने पर कॉल किया जाने वाला कॉलबैक दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [onFinish()](#onFinish--) | वह विधि जो सभी पृष्ठ लिखे जाने पर कॉल की जाएगी। |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | एक पृष्ठ को स्ट्रीम में सहेजे जाने पर कॉल की जाने वाली विधि। |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


वह विधि जो सभी पृष्ठ लिखे जाने पर कॉल की जाएगी।

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


एक पृष्ठ को स्ट्रीम में सहेजे जाने पर कॉल की जाने वाली विधि।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | पृष्ठ सहेजने के तर्क। |

