---
title: "ImageSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de projet en images."
type: docs
weight: 134
url: /fr/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de projet en images.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Initialise une nouvelle instance de la classe [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) qui peut être utilisée pour enregistrer les images rendues aux formats TIFF, PNG, BMP ou JPEG. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Spécifie les paramètres de police utilisés lors du rendu de la vue du projet. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Obtient la résolution horizontale en dpi. |
| [getJpegQuality()](#getJpegQuality--) | Obtient une qualité JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtient un callback défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [getPages()](#getPages--) | Obtient une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés. |
| [getPixelFormat()](#getPixelFormat--) | Obtient le format des données couleur pour chaque pixel de l'image. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [getTiffCompression()](#getTiffCompression--) | Obtient le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | Obtient la résolution verticale en dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Définit la résolution horizontale en dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Définit une qualité JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Définit une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Définit le format des données couleur pour chaque pixel de l'image. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Définit le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Définit la résolution verticale en dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Initialise une nouvelle instance de la classe [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) qui peut être utilisée pour enregistrer les images rendues aux formats TIFF, PNG, BMP ou JPEG.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | Peut être TIFF, PNG, BMP ou JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Spécifie les paramètres de police utilisés lors du rendu de la vue du projet.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Obtient la résolution horizontale en dpi.

**Returns:**
float - la résolution horizontale en dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Obtient une qualité JPEG. La plage de valeurs autorisée est 0..100.

**Returns:**
int - une qualité JPEG.
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


Obtient une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés.

--------------------

Toutes les pages seront enregistrées si cette liste est vide.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Obtient le format des données couleur pour chaque pixel de l'image.

**Returns:**
int - le format des données couleur pour chaque pixel de l'image.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Returns:**
boolean - une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Obtient le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF.

--------------------

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Obtient la résolution verticale en dpi.

**Returns:**
float - la résolution verticale en dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Définit la résolution horizontale en dpi.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | la résolution horizontale en ppp. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Définit une qualité JPEG. La plage de valeurs autorisée est 0..100.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une qualité JPEG. |

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


Définit une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés.

--------------------

Toutes les pages seront enregistrées si cette liste est vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;java.lang.Integer&gt; | une liste de numéros de page à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Définit le format des données couleur pour chaque pixel de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le format des données de couleur pour chaque pixel de l'image. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Définit le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF.

--------------------

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Définit la résolution verticale en dpi.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | la résolution verticale en ppp. |

