---
title: "PdfSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages du projet en PDF."
type: docs
weight: 191
url: /fr/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages du projet en PDF.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialise une nouvelle instance de la classe [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) qui peut être utilisée pour enregistrer un document au format [SaveFileFormat](../../com.aspose.tasks/savefileformat). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Obtient le niveau de conformité souhaité pour le document PDF généré. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Obtient les détails du chiffrement. |
| [getFontSettings()](#getFontSettings--) | Spécifie les paramètres de police utilisés lors du rendu de la vue du projet. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtient un callback défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [getPages()](#getPages--) | Obtient la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Obtient une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés. |
| [getTextCompression()](#getTextCompression--) | Obtient le type de compression à utiliser pour tous les flux de contenu sauf les images. |
| [setCompliance(int value)](#setCompliance-int-) | Définit le niveau de conformité souhaité pour le document PDF généré. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Définit les détails du chiffrement. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Définit la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Définit une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés. |
| [setTextCompression(int value)](#setTextCompression-int-) | Définit le type de compression à utiliser pour tous les flux de contenu sauf les images. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialise une nouvelle instance de la classe [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) qui peut être utilisée pour enregistrer un document au format [SaveFileFormat](../../com.aspose.tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Obtient le niveau de conformité souhaité pour le document PDF généré. La valeur par défaut est [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Returns:**
int - un niveau de conformité souhaité pour le document PDF généré.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Obtient les détails du chiffrement. Si non défini, aucun chiffrement ne sera effectué.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Spécifie les paramètres de police utilisés lors du rendu de la vue du projet.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtient un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. S'applique lorsque l'option `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) est utilisée.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Obtient la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés.

--------------------

Toutes les pages seront enregistrées si cette liste est vide.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtient une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Returns:**
boolean - une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Obtient une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés.

**Returns:**
boolean - une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Obtient un type de compression à utiliser pour tous les flux de contenu sauf les images. La valeur par défaut est [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - un type de compression à utiliser pour tous les flux de contenu sauf les images.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Définit le niveau de conformité souhaité pour le document PDF généré. La valeur par défaut est [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un niveau de conformité souhaité pour le document PDF généré. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Définit les détails du chiffrement. Si non défini, aucun chiffrement ne sera effectué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | des détails du chiffrement. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. S'applique lorsque l'option `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) est utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Définit la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés.

--------------------

Toutes les pages seront enregistrées si cette liste est vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;java.lang.Integer&gt; | la liste des numéros de pages à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Définit une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Définit un type de compression à utiliser pour tous les flux de contenu sauf les images. La valeur par défaut est [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un type de compression à utiliser pour tous les flux de contenu sauf les images. |

