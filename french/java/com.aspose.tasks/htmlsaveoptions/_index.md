---
title: "HtmlSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de projet en HTML."
type: docs
weight: 132
url: /fr/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de projet en HTML.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Initialise une nouvelle instance de la classe [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Obtient le callback qui est appelé pour créer la ressource où stocker le CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Obtient le préfixe de style CSS. |
| [getExportCss()](#getExportCss--) | Obtient la façon dont le CSS est exporté. |
| [getExportFonts()](#getExportFonts--) | Obtient la façon dont les polices sont exportées. |
| [getExportImages()](#getExportImages--) | Obtient la façon dont les images sont exportées. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Obtient les types de police. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Obtient le callback qui est appelé pour créer la ressource où stocker la police. |
| [getFontSettings()](#getFontSettings--) | Spécifie les paramètres de police utilisés lors du rendu de la vue du projet. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Obtient le callback qui est appelé pour créer la ressource où stocker la police. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Obtient une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Obtient une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtient un callback défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [getPages()](#getPages--) | Obtient une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Obtient une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Définit le callback qui est appelé pour créer la ressource où stocker le CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Définit le préfixe de style CSS. |
| [setExportCss(int value)](#setExportCss-int-) | Définit la façon dont le CSS est exporté. |
| [setExportFonts(int value)](#setExportFonts-int-) | Définit la façon dont les polices sont exportées. |
| [setExportImages(int value)](#setExportImages-int-) | Définit la façon dont les images sont exportées. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Définit les types de police. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Définit le rappel qui est appelé pour créer la ressource de stockage de la police. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Définit le rappel qui est appelé pour créer la ressource de stockage de la police. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Définit une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Définit une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Initialise une nouvelle instance de la classe [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Réservé à un usage interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Réservé à un usage interne.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Obtient le callback qui est appelé pour créer la ressource où stocker le CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Obtient le préfixe de style CSS.

**Returns:**
java.lang.String - préfixe de style CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Obtient la façon dont le CSS est exporté.

**Returns:**
int - la façon dont le CSS est exporté.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Obtient la façon dont les polices sont exportées.

**Returns:**
int - la façon dont les polices sont exportées.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Obtient la façon dont les images sont exportées.

**Returns:**
int - la façon dont les images sont exportées.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Obtient les types de police.

Valeur : les types de police.

**Returns:**
int - les types de police.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Obtient le callback qui est appelé pour créer la ressource où stocker la police.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Spécifie les paramètres de police utilisés lors du rendu de la vue du projet.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Obtient le callback qui est appelé pour créer la ressource où stocker la police.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Obtient une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML.

**Returns:**
boolean - une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Obtient une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML.

**Returns:**
boolean - une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtient un callback défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Obtient une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet.

--------------------

Toutes les pages du projet seront enregistrées si cette liste est vide.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Returns:**
boolean - une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Obtient une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.

--------------------

L'utilisation actuelle du pinceau dégradé n'est pas prise en charge lors du rendu en HTML.

**Returns:**
boolean - une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Définit le callback qui est appelé pour créer la ressource où stocker le CSS.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | le rappel qui est appelé pour créer la ressource de stockage du CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Définit le préfixe de style CSS.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | Préfixe de style CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Définit la façon dont le CSS est exporté.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la façon dont le CSS est exporté. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Définit la façon dont les polices sont exportées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la façon dont les polices sont exportées. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Définit la façon dont les images sont exportées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la façon dont les images sont exportées. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Définit les types de police.

Valeur : les types de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | les types de fontes. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Définit le rappel qui est appelé pour créer la ressource de stockage de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | le rappel qui est appelé pour créer la ressource de stockage de la police. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Définit le rappel qui est appelé pour créer la ressource de stockage de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | le rappel qui est appelé pour créer la ressource de stockage de la police. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Définit une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet.

--------------------

Toutes les pages du projet seront enregistrées si cette liste est vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;java.lang.Integer&gt; | une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Définit une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.

--------------------

L'utilisation actuelle du pinceau dégradé n'est pas prise en charge lors du rendu en HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |

