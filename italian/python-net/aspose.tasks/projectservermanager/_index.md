---
title: "ProjectServerManager"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 870
url: /it/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

La classe che fornisce i metodi per leggere e per eseguire operazioni sui progetti nell'account Project Online specificato o<br/>
            nell'istanza on-premise di Project Server specificata (sono supportate le versioni 2016 e 2019 di Project Server).

Il tipo ProjectServerManager espone i seguenti membri:
## Costruttori
| Nome | Descrizione |
| :- | :- |
| ProjectServerManager(credentials) | Inizializza una nuova istanza della classe [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/). |
## Methods
| Nome | Descrizione |
| :- | :- |
| update_project(project) | Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. Il progetto esistente sarà sovrascritto. |
| update_project(project, save_options) | Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. Il progetto esistente sarà sovrascritto. |
| create_new_project(project) | Crea un nuovo progetto nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. |
| create_new_project(project, save_options) | Crea un nuovo progetto nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. |
| get_project(project_guid) | Recupera il progetto con il GUID specificato dall'account Project Online \ istanza di Project Server. |
| get_project_raw_data(project_guid) | Recupera i dati binari del progetto per scopi di risoluzione dei problemi. |
| get_project_list() | Recupera l'elenco dei progetti dal deposito 'Working' dell'attuale account Project Online \ istanza di Project Server. |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

