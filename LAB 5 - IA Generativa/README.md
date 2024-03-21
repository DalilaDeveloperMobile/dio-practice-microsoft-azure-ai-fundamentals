# ia-generativa-microsoft-azure
Passo a passo de experimento usando:
 - Recursos de IA Generativa com Copilot e OpenAI.

 > [!NOTE]
> Essas informações são exclusivamente uma maneira de fazer essas atividades.
>  Mais o preferencial sempre será a Documentação Oficial: [Microsoft Copilot](https://aka.ms/ai900-bing-copilot), [Azure OpenAI](https://aka.ms/ai900-azure-openai), [Content Filters In Azure OpenAI](https://aka.ms/ai900-content-filters).

- Gerando Imagens Através de Textos com o [Microsoft Copilot](https://copilot.microsoft.com/).

![Captura de tela 2024-03-21 083758](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/067abf03-26ea-4231-b7a6-67dc6131f643)

### Imagens Geradas:
  - Input 1 & Output 1:
    
![Captura de tela 2024-03-21 090249](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/9228967b-f350-4cb4-8fee-80837e665f43)

  - Input 2 & Output 2:

![Captura de tela 2024-03-21 091349](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/253d0d27-5566-4aae-a342-01da45983593)

# Extrair Texto a Partir de Imagens.
- Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com , entrando com a conta da Microsoft associada à sua assinatura do Azure.
- Clique no botão ＋Criar um recurso e pesquise os serviços de IA do Azure. Selecione criar um plano de serviços de IA do Azure. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:
 - Assinatura: sua assinatura do Azure.
 - Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo.
 - Região: East US.
 - Nome: Insira um nome exclusivo.
 - Nível de preços: Standard S0.
 - Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo: Selecionado.
 - Selecione Rever + criar e, em seguida, Criar e aguarde a conclusão da implantação.

- Quando o serviço tiver terminado, acesse o [Vision Studio](https://portal.vision.cognitive.azure.com/?azure-portal=true) com a sua conta e aperte em “View all resources”.

![Captura de tela 2024-03-13 085124](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/7416fe96-77b7-4232-8c19-0ecf161e4871)

- Selecionamos o nosso recurso e apertamos em “Select as default resource” e apertamos em fechar nesse X.

![Captura de tela 2024-03-13 095100](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e742c464-e868-480a-bd2f-f76427d1faa9)
<br>
