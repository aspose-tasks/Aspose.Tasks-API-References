---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera फ़ाइलों XER या P6XML से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट प्रॉपर्टीज़ का प्रतिनिधित्व करता है।"
type: docs
weight: 205
url: /hi/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Primavera फ़ाइलों (XER या P6XML) से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट गुण दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | वर्तमान प्रोजेक्ट के बेसलाइन प्रोजेक्ट्स की एरे प्राप्त करता है। |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | क्रिटिकल एक्टिविटीज़ को परिभाषित करने की विधि प्राप्त करता है: सबसे लंबा पथ या टोटल फ़्लोट दृष्टिकोण। |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | यदि टोटल फ़्लोट विधि उपयोग की जाती है तो क्रिटिकल एक्टिविटीज़ को परिभाषित करने के लिए उपयोग किए जाने वाले थ्रेशहोल्ड मान को प्राप्त करता है। |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | वर्तमान बेसलाइन प्रोजेक्ट की आईडी प्राप्त करता है। |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि प्रोजेक्ट्स के बीच एक्टिविटी रिलेशनशिप को अनदेखा किया जाए या नहीं। |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि प्रोजेक्ट शेड्यूल करते समय एक्टिविटीज़ को क्रिटिकल के रूप में चिह्नित किया जाना चाहिए या नहीं। |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | एक विकल्प प्राप्त करता है जो निर्धारित करता है कि Primavera प्रोजेक्ट्स में रिलेशनशिप लैग को शेड्यूल करने के लिए कौन सा कैलेंडर उपयोग किया जाए। |
| [getShortName()](#getShortName--) | प्रोजेक्ट का संक्षिप्त नाम (Project ID) प्राप्त करता है। |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि एक्टिविटी समाप्ति तिथियों को अपेक्षित समाप्ति तिथियों के रूप में शेड्यूल किया जाना चाहिए या नहीं। |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


वर्तमान प्रोजेक्ट के बेसलाइन प्रोजेक्ट्स की एरे प्राप्त करता है। यह उन प्रोजेक्ट्स पर लागू होता है जो निर्यातित बेसलाइन वाली Primavera XML फ़ाइलों से पढ़े गए हैं।

**Returns:**
com.aspose.tasks.Project[] - वर्तमान प्रोजेक्ट के बेसलाइन प्रोजेक्ट्स की एरे।
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


क्रिटिकल एक्टिविटीज़ को परिभाषित करने की विधि प्राप्त करता है: सबसे लंबा पथ या टोटल फ़्लोट दृष्टिकोण।

**Returns:**
int - क्रिटिकल एक्टिविटीज़ को परिभाषित करने की विधि: सबसे लंबा पथ या टोटल फ़्लोट दृष्टिकोण।
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


यदि टोटल फ़्लोट विधि उपयोग की जाती है तो क्रिटिकल एक्टिविटीज़ को परिभाषित करने के लिए उपयोग किए जाने वाले थ्रेशहोल्ड मान को प्राप्त करता है।

**Returns:**
java.lang.Double - यदि टोटल फ़्लोट विधि उपयोग की जाती है तो क्रिटिकल एक्टिविटीज़ को परिभाषित करने के लिए उपयोग किया गया थ्रेशहोल्ड मान।
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


वर्तमान बेसलाइन प्रोजेक्ट की आईडी प्राप्त करता है। यह उन प्रोजेक्ट्स पर लागू होता है जो निर्यातित बेसलाइन वाली Primavera XML फ़ाइलों से पढ़े गए हैं।

**Returns:**
int - वर्तमान बेसलाइन प्रोजेक्ट की Id।
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि प्रोजेक्ट्स के बीच एक्टिविटी रिलेशनशिप को अनदेखा किया जाए या नहीं।

**Returns:**
boolean - एक फ़्लैग जो निर्धारित करता है कि प्रोजेक्ट्स के बीच गतिविधि संबंधों को अनदेखा किया जाए या नहीं।
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि प्रोजेक्ट शेड्यूल करते समय एक्टिविटीज़ को क्रिटिकल के रूप में चिह्नित किया जाना चाहिए या नहीं।

**Returns:**
boolean - एक फ़्लैग जो निर्धारित करता है कि प्रोजेक्ट शेड्यूल करते समय गतिविधियों को महत्वपूर्ण के रूप में चिह्नित किया जाना चाहिए या नहीं।
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


एक विकल्प प्राप्त करता है जो निर्धारित करता है कि Primavera प्रोजेक्ट्स में रिलेशनशिप लैग को शेड्यूल करने के लिए कौन सा कैलेंडर उपयोग किया जाए।

**Returns:**
int - एक विकल्प जो निर्धारित करता है कि Primavera प्रोजेक्ट्स में रिलेशनशिप लैग शेड्यूल करने के लिए कौन सा कैलेंडर उपयोग किया जाए।
### getShortName() {#getShortName--}
```
public final String getShortName()
```


प्रोजेक्ट का संक्षिप्त नाम (Project ID) प्राप्त करता है।

**Returns:**
java.lang.String - प्रोजेक्ट का संक्षिप्त नाम (Project ID).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि एक्टिविटी समाप्ति तिथियों को अपेक्षित समाप्ति तिथियों के रूप में शेड्यूल किया जाना चाहिए या नहीं।

**Returns:**
boolean - एक फ़्लैग जो निर्धारित करता है कि गतिविधि समाप्ति तिथियों को अपेक्षित समाप्ति तिथियों के रूप में शेड्यूल किया जाए या नहीं।
