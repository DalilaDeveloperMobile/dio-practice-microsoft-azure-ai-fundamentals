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
