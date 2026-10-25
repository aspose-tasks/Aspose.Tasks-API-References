---
title: "License.SetLicense"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método License. Licencia el componente."
type: docs
weight: 20
url: /es/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licencia el componente.

```csharp
public void SetLicense(string licenseName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| licenseName | Cadena | Puede ser un nombre de archivo completo o corto, o el nombre de un recurso incrustado. Use una cadena vacía para cambiar al modo de evaluación. |

## Observaciones

Intenta encontrar la licencia en las siguientes ubicaciones:

1. Ruta explícita.

2. La carpeta que contiene el ensamblado del componente Aspose.

3. La carpeta que contiene el ensamblado que llama el cliente.

4. La carpeta que contiene el ensamblado de entrada (inicio).

5. Un recurso incrustado en el ensamblado que llama el cliente.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Ruta explícita.

2. Un recurso incrustado en el ensamblado que llama el cliente.

2. La carpeta que contiene el archivo JAR del componente Aspose.

3. La carpeta que contiene el archivo JAR que llama el cliente.

## Ejemplos

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

el archivo jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Muestra cómo aplicar una licencia de Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Ver también

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

Licencia el componente.

```csharp
public void SetLicense(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Un flujo que contiene la licencia. |

## Observaciones

Use este método para cargar una licencia desde un flujo.

## Ejemplos

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Muestra cómo aplicar una licencia de Aspose.Tasks leída desde &lt;see cref=\"System.IO.FileStream\" /&gt;.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### Ver también

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


