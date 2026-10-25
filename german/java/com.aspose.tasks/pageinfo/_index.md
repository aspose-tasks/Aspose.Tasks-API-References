---
title: "PageInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Seiteneinrichtungsdaten dar, die im MPP-Dateiformat vorhanden und zum Drucken verwendet werden."
type: docs
weight: 176
url: /de/java/com.aspose.tasks/pageinfo/
---

**Inheritance:**
java.lang.Object
```
public class PageInfo
```

Stellt Seiteneinrichtungsdaten dar, die im MPP-Dateiformat vorhanden und zum Drucken verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PageInfo()](#PageInfo--) | Initialisiert eine neue Instanz der Klasse [PageInfo](../../com.aspose.tasks/pageinfo). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFooter()](#getFooter--) | Gibt eine Instanz der Klasse [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) zurück, die Fußzeilendaten darstellt. |
| [getHeader()](#getHeader--) | Gibt die Instanz der Klasse [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) zurück, die Kopfzeilendaten darstellt. |
| [getLegend()](#getLegend--) | Ruft eine Instanz der [PageLegend](../../com.aspose/tasks/pagelegend)-Klasse ab, die die Rendering-Optionen der Seitenlegende festlegt. |
| [getMargins()](#getMargins--) | Ruft eine Instanz der [PageMargins](../../com.aspose/tasks/pagemargins)-Klasse ab, die die Seitenränder festlegt. |
| [getName()](#getName--) | Ruft den Namen der Ansicht ab, für die Setup-Daten verwendet werden. |
| [getPageSettings()](#getPageSettings--) | Ruft eine Instanz der `PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--))-Klasse ab, die die Druckeinstellungen der Seite festlegt. |
| [getPageViewSettings()](#getPageViewSettings--) | Ruft eine Instanz der `PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--))-Klasse ab, die die Druckeinstellungen der Seitenansicht festlegt. |
| [setFooter(HeaderFooterInfo value)](#setFooter-com.aspose.tasks.HeaderFooterInfo-) | Setzt eine Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Fußzeilendaten darstellt. |
| [setHeader(HeaderFooterInfo value)](#setHeader-com.aspose.tasks.HeaderFooterInfo-) | Setzt die Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Kopfdaten darstellt. |
| [setLegend(PageLegend value)](#setLegend-com.aspose.tasks.PageLegend-) | Setzt eine Instanz der [PageLegend](../../com.aspose/tasks/pagelegend)-Klasse, die die Rendering-Optionen der Seitenlegende festlegt. |
### PageInfo() {#PageInfo--}
```
public PageInfo()
```


Initialisiert eine neue Instanz der [PageInfo](../../com.aspose/tasks/pageinfo)-Klasse. Stellt Seiteneinrichtungsdaten dar, die im MPP-Dateiformat vorhanden und für den Druck verwendet werden.

### getFooter() {#getFooter--}
```
public final HeaderFooterInfo getFooter()
```


Gibt eine Instanz der Klasse [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) zurück, die Fußzeilendaten darstellt.

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - an instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a footer data.
### getHeader() {#getHeader--}
```
public final HeaderFooterInfo getHeader()
```


Gibt die Instanz der Klasse [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) zurück, die Kopfzeilendaten darstellt.

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - the instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a header data.
### getLegend() {#getLegend--}
```
public final PageLegend getLegend()
```


Ruft eine Instanz der [PageLegend](../../com.aspose/tasks/pagelegend)-Klasse ab, die die Rendering-Optionen der Seitenlegende festlegt.

--------------------

Derzeit gilt dies nur für Gantt-Diagramm-Ansichten.

**Returns:**
[PageLegend](../../com.aspose.tasks/pagelegend) - an instance of the [PageLegend](../../com.aspose.tasks/pagelegend) class which specifies rendering options of page legend.
### getMargins() {#getMargins--}
```
public final PageMargins getMargins()
```


Ruft eine Instanz der [PageMargins](../../com.aspose/tasks/pagemargins)-Klasse ab, die die Seitenränder festlegt.

**Returns:**
[PageMargins](../../com.aspose.tasks/pagemargins) - an instance of the [PageMargins](../../com.aspose.tasks/pagemargins) class which specifies page margins.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Namen der Ansicht ab, für die Setup-Daten verwendet werden.

**Returns:**
java.lang.String – der Name der Ansicht, für die Setup-Daten verwendet werden.
### getPageSettings() {#getPageSettings--}
```
public final PageSettings getPageSettings()
```


Ruft eine Instanz der `PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--))-Klasse ab, die die Druckeinstellungen der Seite festlegt.

**Returns:**
[PageSettings](../../com.aspose.tasks/pagesettings) - an instance of the `PageSettings`([getPageSettings()](../../com.aspose.tasks/pageinfo\#getPageSettings--)) class which specifies page printing settings.
### getPageViewSettings() {#getPageViewSettings--}
```
public final PageViewSettings getPageViewSettings()
```


Ruft eine Instanz der `PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--))-Klasse ab, die die Druckeinstellungen der Seitenansicht festlegt.

**Returns:**
[PageViewSettings](../../com.aspose.tasks/pageviewsettings) - an instance of the `PageViewSettings`([getPageViewSettings()](../../com.aspose.tasks/pageinfo\#getPageViewSettings--)) class which specifies page view printing settings.
### setFooter(HeaderFooterInfo value) {#setFooter-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setFooter(HeaderFooterInfo value)
```


Setzt eine Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Fußzeilendaten darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | eine Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Fußzeilendaten darstellt. |

### setHeader(HeaderFooterInfo value) {#setHeader-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setHeader(HeaderFooterInfo value)
```


Setzt die Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Kopfdaten darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | die Instanz der [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)-Klasse, die Kopfdaten darstellt. |

### setLegend(PageLegend value) {#setLegend-com.aspose.tasks.PageLegend-}
```
public final void setLegend(PageLegend value)
```


Setzt eine Instanz der [PageLegend](../../com.aspose/tasks/pagelegend)-Klasse, die die Rendering-Optionen der Seitenlegende festlegt.

--------------------

Derzeit gilt dies nur für Gantt-Diagramm-Ansichten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PageLegend](../../com.aspose.tasks/pagelegend) | eine Instanz der [PageLegend](../../com.aspose/tasks/pagelegend)-Klasse, die die Rendering-Optionen der Seitenlegende festlegt. |

