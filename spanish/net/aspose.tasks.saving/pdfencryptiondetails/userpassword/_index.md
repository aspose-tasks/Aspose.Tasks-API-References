---
title: "PdfEncryptionDetails.UserPassword"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfEncryptionDetails. Obtiene o establece la contraseña de usuario"
type: docs
weight: 50
url: /es/net/aspose.tasks.saving/pdfencryptiondetails/userpassword/
---
## PdfEncryptionDetails.UserPassword property

Obtiene o establece la contraseña del usuario.

```csharp
public string UserPassword { get; set; }
```

## Observaciones

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tenga contraseña de usuario) permite realizar operaciones adicionales según los permisos de acceso de usuario especificados en el diccionario de cifrado del documento.

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


