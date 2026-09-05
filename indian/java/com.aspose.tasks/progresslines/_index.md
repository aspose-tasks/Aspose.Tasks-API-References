---
title: "ProgressLines"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Gantt चार्ट दृश्य में प्रोग्रेस लाइन्स दर्शाता है।"
type: docs
weight: 219
url: /hi/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Gantt चार्ट दृश्य में प्रोग्रेस लाइन्स दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | प्रोग्रेस लाइन्स प्रदर्शित करने की तिथि प्राप्त करता है। |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | प्रोजेक्ट की प्रारम्भ तिथि से प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है। |
| [getDateFormat()](#getDateFormat--) | तारीख स्वरूप प्राप्त करता है ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | वर्तमान तिथि पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है। |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | आवर्ती अंतराल पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है। |
| [getDisplaySelected()](#getDisplaySelected--) | चयनित तिथियों पर प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है। |
| [getFont()](#getFont--) | प्रगति रेखा लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को प्राप्त करता है। |
| [getLineColor()](#getLineColor--) | वर्तमान प्रगति रेखा के लिए रेखा का रंग प्राप्त करता है। |
| [getLinePattern()](#getLinePattern--) | वर्तमान प्रगति रेखा का रेखा पैटर्न प्राप्त करता है। |
| [getOtherLineColor()](#getOtherLineColor--) | अन्य प्रगति रेखा का रंग प्राप्त करता है। |
| [getOtherLinePattern()](#getOtherLinePattern--) | अन्य प्रगति रेखा के लिए रेखा पैटर्न प्राप्त करता है। |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | अन्य प्रगति बिंदु का रंग प्राप्त करता है। |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | अन्य प्रगति रेखा के प्रगति बिंदु का आकार प्राप्त करता है। |
| [getProgressPointColor()](#getProgressPointColor--) | प्रगति बिंदु का रंग प्राप्त करता है। |
| [getProgressPointShape()](#getProgressPointShape--) | प्रगति बिंदु का आकार प्राप्त करता है। |
| [getRecurringInterval()](#getRecurringInterval--) | आवर्ती अंतराल प्राप्त करता है। |
| [getSelectedDates()](#getSelectedDates--) | प्रगति रेखाएँ प्रदर्शित करने के लिए चयनित तिथियों की सूची प्राप्त करता है। |
| [getShowDate()](#getShowDate--) | प्रत्येक प्रगति रेखा के लिए तिथि दिखाने का संकेत देने वाला मान प्राप्त करता है। |
| [isBaselinePlan()](#isBaselinePlan--) | बेसलाइन योजना या वास्तविक के लिए प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है। |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | बेसलाइन योजना या वास्तविक के लिए प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है। |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | प्रगति रेखाएँ प्रदर्शित करने की तिथि सेट करता है। |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | प्रोजेक्ट की प्रारम्भ तिथि से प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है। |
| [setDateFormat(int value)](#setDateFormat-int-) | तारीख स्वरूप सेट करता है ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | वर्तमान तिथि पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान सेट करता है। |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | आवर्ती अंतराल पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान सेट करता है। |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | चयनित तिथियों पर प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है। |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | प्रोग्रेस लाइन लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को सेट करता है। |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | वर्तमान प्रोग्रेस लाइन के लिए लाइन का रंग सेट करता है। |
| [setLinePattern(int value)](#setLinePattern-int-) | वर्तमान प्रोग्रेस लाइन का लाइन पैटर्न सेट करता है। |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | अन्य प्रोग्रेस लाइन का रंग सेट करता है। |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | अन्य प्रोग्रेस लाइन के लिए लाइन पैटर्न सेट करता है। |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | अन्य प्रोग्रेस पॉइंट का रंग सेट करता है। |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | अन्य प्रोग्रेस लाइन के प्रोग्रेस पॉइंट का आकार सेट करता है। |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | प्रोग्रेस पॉइंट का रंग सेट करता है। |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | प्रोग्रेस पॉइंट का आकार सेट करता है। |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | आवर्ती अंतराल सेट करता है। |
| [setShowDate(boolean value)](#setShowDate-boolean-) | प्रत्येक प्रोग्रेस लाइन के लिए तिथि दिखाने का संकेत देने वाला मान सेट करता है। |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


प्रोग्रेस लाइन्स प्रदर्शित करने की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - प्रोग्रेस लाइनों को प्रदर्शित करने की प्रारंभ तिथि।
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


प्रोजेक्ट की प्रारम्भ तिथि से प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - प्रोजेक्ट की प्रारंभ तिथि से प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान।
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


तारीख स्वरूप प्राप्त करता है ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - तिथि स्वरूप ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


वर्तमान तिथि पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - वर्तमान तिथि पर प्रोग्रेस लाइन प्रदर्शित करने का संकेत देने वाला मान।
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


आवर्ती अंतराल पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - आवर्ती अंतराल पर प्रोग्रेस लाइन प्रदर्शित करने का संकेत देने वाला मान।
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


चयनित तिथियों पर प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - चयनित तिथियों पर प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान।
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


प्रगति रेखा लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को प्राप्त करता है।

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


वर्तमान प्रगति रेखा के लिए रेखा का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - वर्तमान प्रोग्रेस लाइन के लिए लाइन का रंग।
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


वर्तमान प्रोग्रेस लाइन का लाइन पैटर्न प्राप्त करता है। `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - वर्तमान प्रोग्रेस लाइन का लाइन पैटर्न।
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


अन्य प्रगति रेखा का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - अन्य प्रोग्रेस लाइन का रंग।
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


अन्य प्रगति रेखा के लिए रेखा पैटर्न प्राप्त करता है।

**Returns:**
int - अन्य प्रोग्रेस लाइन के लिए लाइन पैटर्न।
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


अन्य प्रगति बिंदु का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - अन्य प्रोग्रेस पॉइंट का रंग।
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


अन्य प्रगति रेखा के प्रगति बिंदु का आकार प्राप्त करता है।

**Returns:**
int - अन्य प्रोग्रेस लाइन के प्रोग्रेस पॉइंट का आकार।
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


प्रगति बिंदु का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - प्रोग्रेस पॉइंट का रंग।
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


प्रोग्रेस पॉइंट का आकार प्राप्त करता है। [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - प्रोग्रेस पॉइंट का आकार।
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


आवर्ती अंतराल प्राप्त करता है। `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


प्रगति रेखाएँ प्रदर्शित करने के लिए चयनित तिथियों की सूची प्राप्त करता है।

**Returns:**
java.util.List&lt;java.util.Date&gt; - प्रोग्रेस लाइनों को प्रदर्शित करने के लिए चयनित तिथियों की सूची।
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


प्रत्येक प्रगति रेखा के लिए तिथि दिखाने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - प्रत्येक प्रोग्रेस लाइन के लिए तिथि दिखाने का संकेत देने वाला मान।
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


बेसलाइन योजना या वास्तविक के लिए प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - बेसलाइन योजना या वास्तविक के लिए प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान।
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


बेसलाइन योजना या वास्तविक के लिए प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | बेसलाइन योजना या वास्तविक के लिए प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान। |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


प्रगति रेखाएँ प्रदर्शित करने की तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | प्रोग्रेस लाइनों को प्रदर्शित करने की प्रारंभ तिथि। |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


प्रोजेक्ट की प्रारम्भ तिथि से प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | परियोजना की प्रारंभ तिथि से शुरू होकर प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान। |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


तारीख स्वरूप सेट करता है ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | तिथि प्रारूप ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


वर्तमान तिथि पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | वर्तमान तिथि पर प्रोग्रेस लाइन प्रदर्शित करने का संकेत देने वाला मान। |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


आवर्ती अंतराल पर प्रगति रेखा प्रदर्शित करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | आवर्ती अंतराल पर प्रोग्रेस लाइन प्रदर्शित करने का संकेत देने वाला मान। |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


चयनित तिथियों पर प्रगति रेखाएँ प्रदर्शित करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | चयनित तिथियों पर प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाला मान। |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


प्रोग्रेस लाइन लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | प्रोग्रेस लाइन लेबल के लिए प्रयुक्त फ़ॉन्ट। |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


वर्तमान प्रोग्रेस लाइन के लिए लाइन का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | वर्तमान प्रोग्रेस लाइन का रेखा रंग। |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


वर्तमान प्रोग्रेस लाइन की रेखा पैटर्न सेट करता है। `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वर्तमान प्रोग्रेस लाइन की रेखा पैटर्न। |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


अन्य प्रोग्रेस लाइन का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | अन्य प्रोग्रेस लाइन का रंग। |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


अन्य प्रोग्रेस लाइन के लिए लाइन पैटर्न सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | अन्य प्रोग्रेस लाइन के लिए रेखा पैटर्न। |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


अन्य प्रोग्रेस पॉइंट का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | अन्य प्रोग्रेस पॉइंट का रंग। |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


अन्य प्रोग्रेस लाइन के प्रोग्रेस पॉइंट का आकार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | अन्य प्रोग्रेस लाइन का प्रोग्रेस पॉइंट आकार। |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


प्रोग्रेस पॉइंट का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | प्रोग्रेस पॉइंट का रंग। |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


प्रोग्रेस पॉइंट आकार सेट करता है। [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | प्रोग्रेस पॉइंट आकार। |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


आवर्ती अंतराल सेट करता है। `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | पुनरावर्ती अंतराल। |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


प्रत्येक प्रोग्रेस लाइन के लिए तिथि दिखाने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि प्रत्येक प्रगति पंक्ति के लिए तिथि दिखानी है या नहीं। |

