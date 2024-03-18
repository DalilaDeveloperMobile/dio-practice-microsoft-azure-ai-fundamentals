# ai-search-microsoft-azure
Passo a passo de experimento usando:
  - Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados.

 #### Realizado como desafio de projeto no Bootcamp Microsoft Azure AI Fundamentals da [Dio.me](https://www.dio.me/).

 > [!NOTE]
> Essas informações são exclusivamente uma maneira de fazer essas atividades.
>  Mais o preferencial sempre será a Documentação Oficial: [AI Search](https://aka.ms/ai900-ai-search).

### Passo 1
- Entre no [Portal do Azure](https://portal.azure.com/?azure-portal=true).

#### Clique no botão + Create a resource, pesquise por Azure AI Search, e crie um recurso do Azure AI Search com as seguintes configurações:
- Subscription: Sua assinatura do Azure.
- Resource group: Selecione ou crie um grupo de recursos com um nome exclusivo.
- Service name: Um nome exclusivo.
- Location: Escolha qualquer região disponível. East US.
- Pricing tier: Básico. Selecione Basic.
- Selecione Review + create, e depois de ver a resposta Validation Success, selecione Create.
- Após a conclusão da implantação, selecione Go to resource. Na página de visão geral do Azure AI Search, você pode adicionar índices, importar dados e pesquisar índices criados.

### Passo 2
- Retorne à página inicial do portal do Azure. Clique no botão ＋Create a resource e pesquise por Azure AI services. Selecione criar um plano de Azure AI services. Você será levado a uma página para criar um recurso de Azure AI services. Configure-o com as seguintes configurações:
- Subscription: Sua assinatura do Azure.
- Resource group: O mesmo grupo de recursos que o seu recurso Azure AI Search.
- Region: O mesmo local que o seu recurso Azure AI Search. East US.
- Name: Um nome exclusivo.
- Pricing tier: Standard S0.
- Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo: Selecionado.
- Selecione Review + create. Depois de ver a resposta Validação aprovada, selecione Create.
- Aguarde a conclusão da implantação e visualize os detalhes da implantação.

### Passo 3
- Retorne à página inicial do portal do Azure e selecione o botão + Create a resource.
- Procure por storage account, e crie um recurso de Storage account com as seguintes configurações:
- Subscription: Sua assinatura do Azure.
- Resource group: O mesmo grupo de recursos que os recursos do Azure AI Search e dos serviços Azure AI.
- Storage account name: Um nome exclusivo.
- Location: Escolha qualquer local disponível. (US) East US.
- Performance: Standard
- Redundancy: Locally redundant storage (LRS).
- Clique em Revisar e em Criar. Aguarde a conclusão da implantação e vá para o recurso implantado.
- Na Azure Storage account que você criou, no painel de menu esquerdo, selecione Configuration (em Settings).
- Altere a configuração de Allow Blob anonymous access para Enabled e selecione Save.

### Passo 4
- No painel de menu esquerdo, selecione Containers.

![Captura de tela 2024-03-18 100428](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/5cea760d-7134-4fe0-b909-615ad6dd9ff1)

- Selecione + Container. Um painel do seu lado direito é aberto.
- Insira as seguintes configurações e clique em Create:
- Name: coffeereviews. Avaliações de café.
- Public access level: Container (anonymous read access for containers and blobs)
- Advanced: sem alterações.
- Aperte em Create.

### Passo 5
- Em uma nova guia do navegador, baixe as avaliações compactadas do café em https://aka.ms/mslearn-coffee-reviews, e extraia os arquivos para a pasta de coffee-reviews.
- No portal do Azure, selecione o coffee-reviews container. No container, selecione Upload.

![Captura de tela 2024-03-18 102156](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/762a99ff-9750-40df-836c-86cea104cccc)

- No painel Upload blob, selecione Selecionar um arquivo.
- Na janela do Explorer, selecione todos os arquivos na pasta de avaliações, selecione Abrir e, em seguida, selecione Upload.

![Captura de tela 2024-03-18 102558](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6413f799-934b-4916-b587-e39b14a4fc57)

- Depois que o upload for concluído, você poderá fechar o painel Upload blob. Seus documentos estão agora em seu coffee-reviews storage container.

### Passo 6
- No portal do Azure, navegue até o recurso Azure AI Search. Na página Visão geral, selecione Import data.

![Captura de tela 2024-03-18 103306](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/3421e372-58ba-4abb-b166-7414b7482baf)

- Na página Connect to your data, na lista Data Source, selecione Azure Blob Storage. Preencha os detalhes do armazenamento de dados com os seguintes valores:
- Data Source: Azure Blob Storage.
- Data source name: coffee-customer-data.
- Data to extract: Content and metadata
- Parsing mode: Default
- Connection string: *Selecione Escolha uma conexão existente. Selecione sua conta de armazenamento, selecione o contêiner de avaliações de café e clique em Selecionar.
- Managed identity authentication: None
- Container name: esta configuração é preenchida automaticamente depois que você escolhe uma conexão existente.
- Blob folder: Deixe isso em branco.
- Description: Reviews for Fourth Coffee shops.
- Selecione Next: Add cognitive skills (Optional).

### Passo 7
- Na Página "Add Cognitive skills (optional)", em "Attach AI Services", selecione seu recurso.
- Em "add enrichments" preencher conforme o texto seguido.
- Escreva o nome da Skillset para coffee-skillset.
- Marque a caixa de seleção: Enable OCR and merge all text into merged_content field.
- Certifique-se de que o Source data field esteja definido como merged_content.
- Altere o Enrichment granularity level para Pages (5000 character chunks).
- Não selecione: Enable incremental enrichment.
- Selecione os seguintes campos enriquecidos:
- Extract location names: locations.
- Extract key phrases: keyphrases.
- Detect sentiment: sentiment.
- Generate tags from images: imageTags.
- Generate captions from images: imageCaption.
- Em Save enrichments to a knowledge store, selecione: "Image projections".
- Selecione "choose an existing connection".
- Escolha o storage criado anteriormente.
- Clique em + Container para criar um novo contêiner chamado knowledge-store com o nível de privacidade definido como Private, e selecione Create.
- Selecione então o knowledge-store e clique em "select".

### Passo 8
- Selecione Azure blob projections: Document. Uma configuração para o nome do contêiner com as exibições preenchidas automaticamente do contêiner de armazenamento de conhecimento. Não altere o nome do contêiner.
- Selecione Next: Customize target index. Altere o nome do índice para coffee-index.
- Certifique-se de que a chave esteja definida como metadata_storage_path. Deixe o nome do Suggester name em branco e o Search mode preenchido automaticamente.
- Revise as configurações padrão dos campos de índice. Selecione filterable para todos os campos que estão selecionados por padrão.
- Selecione Next: Create an indexer.

### Passo 9
- Altere o nome do Indexer name para coffee-indexer.
- Deixe o Schedule definida como Once.
- Certifique-se de que a opção Base-64 Encode Keys esteja selecionada.
- Aperte em "submit".

### Passo 10
- Abrir o Azure AI Services| Ai Search, e Aperte em Search Explorer

![Captura de tela 2024-03-18 121011](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6d6e906d-87d0-44c8-91b6-e49708985c53)

- No Search Explorer, Filtrar por conta search=*&$count=true, e aperte em "search".

- Filtrar por localização search=locations:'Chicago' vai exibir as revisões com os sentimentos de pessoa dessa Localização.

- Filtrar por sentimentos negativos de pessoas search=sentiment:'negative'.

<hr>

<h3 align="center"> Four <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> Of Dalila...</h3>
<div align="center"  style="display: inline-block">
  <a href="https://www.linkedin.com/in/dalila-cust%C3%B3dio-046076181/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  <a href = "mailto:dalila.dalila70@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://instagram.com/dalila.dalila70" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a target="_blank" href="https://api.whatsapp.com/send?phone=5588997138541"><img  alt="Whatsapp" width="117px" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a> 
</div>
