---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfEncryptionDetails. Obtiene o establece la contraseña del propietario"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Obtiene o establece la contraseña del propietario.

```csharp
public string OwnerPassword { get; set; }
```

## Observaciones

Abrir el documento con la contraseña del propietario correcta (asumiendo que no sea la misma que la contraseña de usuario) permite acceso total (de propietario) al documento. Este acceso ilimitado incluye la capacidad de cambiar las contraseñas del documento y los permisos de acceso.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


