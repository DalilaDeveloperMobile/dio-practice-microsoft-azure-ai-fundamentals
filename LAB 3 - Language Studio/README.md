# language-studio-microsoft-azure

Passo a passo de experimento usando:
  - Análise de Sentimentos com Language Studio no Azure AI.
    
 #### Realizado como desafio de projeto no Bootcamp Microsoft Azure AI Fundamentals da [Dio.me](https://www.dio.me/).

> [!NOTE]
> Essas informações são exclusivamente uma maneira de fazer essas atividades.
>  Mais o preferencial sempre será a Documentação Oficial: [Estúdio de Fala](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html),
 [Language Studio](https://aka.ms/ai900-text-analysis).

## Estúdio de Fala
- Em outra guia do navegador, abra o [Portal Estúdio de Fala](https://speech.microsoft.com/portal) entrando com a conta da Microsoft do Azure.
  
### Comentário: O sistema pega um arquivo de áudio e vai transcrever em texto ou um texto e vai transformar em áudio.

## Configuração:
#### Selecione Configurações e depois Crie um recurso. Configure-o com as seguintes configurações:
- Nome do novo recurso : Insira um nome exclusivo.
- Assinatura : sua assinatura do Azure.
- Região : Selecione uma região suportada: Leste dos EUA.
- Nível de preços : selecione Padrão S0.
- Grupo de recursos : selecione ou crie um grupo de recursos com um nome exclusivo.
- Selecione Criar recurso.
- Aguarde até que o recurso seja criado.
- selecione Usar recurso.
- Aperte em X para navegar para a página Introdução à Fala.

## Conversão de fala em texto: 
### Passo 1
- Acessar a parte da tela onde tem conversão de fala em texto.
- Apertar Conversão de fala em texto em tempo real.

### Passo 2
- Escolher um idioma.
  
![Captura de tela 2024-03-15 101027](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/f9cf00a6-94ac-4811-b4d8-f891b4c1dfb6)
  
- Em Escolher arquivos de áudio, selecione Procurar arquivos e navegue até a pasta onde você salvou o arquivo. km_20240128_1080p_30f_20240128_114750 e depois Abrir.
  
![Captura de tela 2024-03-15 101045](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/2ffca9a7-6d34-4388-925b-806ac491daad)

## Análise de Sentimentos:
### Passo 1
- Em outra guia do navegador, abra o portal do Azure em [Portal Azure](https://portal.azure.com), entrando com a conta da Microsoft associada à sua assinatura do Azure.

### Passo 2
- Clique no botão ＋ Create a resource.
- Procure por Language service.
- Selecione criar Language service.
- Você será levado a uma página para Select additional features.
- Mantenha a seleção padrão e clique em Continue to create your resource.

### Passo 3
#### Na página Create Language, configure-o com as seguintes configurações:
- Subscription: sua assinatura do Azure.
- Resource group: selecione ou crie um grupo de recursos com um nome exclusivo.
- Region: East US.
- Name: Insira um nome exclusivo..
- Pricing tier: Free F0.
- Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo: Selecionado.
- Selecione Review + create e depois Create e aguarde a conclusão da implantação.

### Passo 4
- Em outra guia do navegador, abra o [Portal Language Studio](https://language.cognitive.azure.com) e entre com a conta da Microsoft do Azure.

### Passo 5
#### Quando solicitado com Select an Azure resource, faça as seguintes configurações:
- Azure directory: Diretório Padrão, o diretório que você está usando. Ex: Canal da Cloud.
- Azure subscription: Selecione a assinatura que você está usando.
- Resource type: Language
- Resource name: Selecione o recurso de serviço de idioma que você acabou de criar.
- Em seguida, selecione: Done.

### Passo 6
- Na página inicial Language Studio. Selecione a guia Classify text.
- Em seguida, selecione o bloco Analyze sentiment and mine opinions.
- Em Selecionar idioma do texto, pode ser Inglês ou Português de sua preferência.
- Escreva a Sentença ou Selecione o seu recurso Azure.
- Marque o CheckBox e Aperte em Run.

## Resultado:
### Sentimento do Documento:

![Captura de tela 2024-03-15 113314](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/2bb65bf4-cd85-4117-97f7-75fc1bd6fe57)

### Sentence 1
- EN: I bought a size S and it fit perfectly

![S1](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/cecddc80-2e0d-4d9d-8c85-f49336e0ff10)

### Sentence 2
- EN: I found the zipper a little bit difficult to get up & down due to the side rushing.

![S2](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/5eb8cc6f-4316-4d4b-83cb-e8a1672686f1)

### Sentence 3
- EN: The color and material are beautiful in person.

![S3](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e461cb73-f48d-41bc-bb35-a6ec47f8cf0a)

### Sentence 4
- EN: Amazingly comfortable!

![S4](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/b4e1d7a8-ed1b-4e4e-9679-6da73a11d30c)

### Original text
- EN: I bought a size S and it fit perfectly. I found the zipper a little bit difficult to get up & down due to the side rushing. The color and material are beautiful in person. Amazingly comfortable!

![OT](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6efd5aff-f1cf-4168-8680-9c133c52f3fa)

<hr>

<h3 align="center"> Three <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> Of Dalila...</h3>
<div align="center"  style="display: inline-block">
  <a href="https://www.linkedin.com/in/dalila-cust%C3%B3dio-046076181/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  <a href = "mailto:dalila.dalila70@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://instagram.com/dalila.dalila70" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a target="_blank" href="https://api.whatsapp.com/send?phone=5588997138541"><img  alt="Whatsapp" width="117px" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a> 
</div>

