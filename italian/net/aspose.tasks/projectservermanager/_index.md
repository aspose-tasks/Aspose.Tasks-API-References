---
title: "Classe ProjectServerManager"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.ProjectServerManager classe. La classe che fornisce i metodi per leggere e per eseguire operazioni sui progetti nell'account Project Online specificato o nell'istanza onpremise di Project Server specificata. Sono supportate le versioni di Project Server 2016 e 2019."
type: docs
weight: 1500
url: /it/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

La classe che fornisce i metodi per leggere ed eseguire operazioni sui progetti nell'account Project Online specificato o nell'istanza on-premise di Project Server specificata (sono supportate le versioni 2016 e 2019 di Project Server).

```csharp
public sealed class ProjectServerManager
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Inizializza una nuova istanza della classe `ProjectServerManager`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Crea un nuovo progetto nell'istanza Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Crea un nuovo progetto nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Recupera il progetto con il guid specificato dall'account Project Online \ istanza di Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Recupera l'elenco dei progetti dal deposito 'Working' dell'account Project Online corrente \ istanza di Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Recupera i dati binari del progetto per scopi di risoluzione dei problemi. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. Il progetto esistente verrà sovrascritto. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. Il progetto esistente verrà sovrascritto. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server. |

## Esempi

Mostra come utilizzare il gestore di Project Server per creare un nuovo progetto con opzioni di salvataggio predefinite su Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


