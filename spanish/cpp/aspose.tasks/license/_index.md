---
title: "Aspose::Tasks::License clase"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks for C++"
description: "Proporciona métodos para licenciar el componente."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/license/
---

## License class

Proporciona métodos para licenciar el componente.

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene <ms> el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> el archivo jar del componente:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Constructores

| Nombre | Descripción |
| --- | --- |
| [License](./license/) | Inicializa una nueva instancia de la clase License. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Licencia el componente. |

