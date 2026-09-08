---
title: "Enumeración PdfPermissions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.PdfPermissions. Especifica los permisos a usar para acceder a un documento PDF."
type: docs
weight: 2120
url: /es/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Especifica los permisos a usar para acceder a un documento PDF.

```csharp
public enum PdfPermissions
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Especifica los permisos a usar para acceder a un documento PDF. |
| Printing | `4` | Especifica los permisos a usar para acceder a un documento PDF. |
| ModifyContents | `8` | Especifica los permisos a usar para acceder a un documento PDF. |
| ContentCopy | `16` | Especifica los permisos a usar para acceder a un documento PDF. |
| ModifyAnnotations | `32` | Especifica los permisos a usar para acceder a un documento PDF. |
| FillIn | `256` | Especifica los permisos a usar para acceder a un documento PDF. |
| ContentCopyForAccessibility | `512` | Especifica los permisos a usar para acceder a un documento PDF. |
| DocumentAssembly | `1024` | Especifica los permisos a usar para acceder a un documento PDF. |
| HighResolutionPrinting | `2052` | Especifica los permisos a usar para acceder a un documento PDF. |
| AllowAll | `65535` | Especifica los permisos a usar para acceder a un documento PDF. |

## Ejemplos

Muestra cómo especificar los detalles de cifrado PDF al guardar un proyecto como archivo PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// especifica los detalles de cifrado
var encryptionDetails = new PdfEncryptionDetails(
    // especificar la contraseña del usuario
    "userPassword", 
    // especificar la contraseña del propietario
    "ownerPassword", 
    // especificar el algoritmo de cifrado
    PdfEncryptionAlgorithm.RC4_128);

// especificar los permisos
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// mostrar las contraseñas del usuario y del propietario
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// mostrar modo de cifrado: RC4_40 o RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// guardar el proyecto con los detalles de cifrado especificados
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


