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
