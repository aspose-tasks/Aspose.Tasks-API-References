---
title: "इवेंट"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक इवेंट।"
type: docs
weight: 374
url: /hi/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

एक इवेंट।

`TArgs`: इवेंट तर्क।

TArgs :
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | जब इवेंट उत्सर्जित होता है, तब यह मेथड बुलाया जाता है। |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


जब इवेंट उत्सर्जित होता है, तब यह मेथड बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रेषक | java.lang.Object | एक वस्तु जो इस घटना को आरंभ करती है। |
| args | TArgs | कस्टम तर्क। |

