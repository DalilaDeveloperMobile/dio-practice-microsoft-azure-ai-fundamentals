# vision-studio-microsoft-azure
 Passo a passo de experimento usando:
-  Vision Studio/ Azure AI Vision para extrair texto de imagens sem a utilização de código.
-  Com tecnologia OCR (Optical Character Recognition).
#### Realizado como desafio de projeto no Bootcamp Microsoft Azure AI Fundamentals da [Dio.me](https://www.dio.me/).

> [!NOTE]
> Esse passo a passo é somente uma forma alternativa de realizar o procedimento. Sempre dê preferência a
> [Documentação Oficial - Reconhecimento](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html), [Documentação oficial - Analise de documentos](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html) e [Documentação oficial - Analise imagens](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html).

## Passo 1
- Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com , entrando com a conta da Microsoft associada à sua assinatura do Azure.

- Clique no botão ＋Criar um recurso e pesquise os serviços de IA do Azure . Selecione criar um plano de serviços de IA do Azure . Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:
  
- Assinatura : sua assinatura do Azure .
- Grupo de recursos : selecione ou crie um grupo de recursos com um nome exclusivo .
- Região : Leste dos EUA.
- Nome : Insira um nome exclusivo .
- Nível de preços : Padrão S0.
- Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo : Selecionado .
- Selecione Rever + criar e, em seguida , Criar e aguarde a conclusão da implantação.

## Passo 2
- Quando o serviço tiver terminado, acesse o [Vision Studio](https://portal.vision.cognitive.azure.com/?azure-portal=true) com a sua conta e aperte em “View all resources”.

![Captura de tela 2024-03-13 085124](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/7416fe96-77b7-4232-8c19-0ecf161e4871)

- Selecionamos o nosso recurso e apertamos em “Select as default resource” e apertamos em fechar nesse X.

![Captura de tela 2024-03-13 095100](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e742c464-e868-480a-bd2f-f76427d1faa9)
<br>

## Passo 3
### Reconhecimento de Face.

![Captura de tela 2024-03-13 104817](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/7875fce2-8e48-4a41-824a-fb16fb7930e9)

- Acesse o “Detect faces in an image”.

![Captura de tela 2024-03-13 105057](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/180bf2f1-43d3-4731-a78d-9f2b477cdf9d)

- Entre com sua conta e selecione: Try it out.
- Agora só selecionar uma das imagens padrões ou em seu computador e faça os testes.

![Captura de tela 2024-03-13 091621](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/23a4fa3a-31e6-40d7-9c22-20725404c86b)

![Captura de tela 2024-03-13 091719](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/c9aa487f-a4bc-48c2-9029-231203cfa090)

### Analise de documentos

- Acesse o Optical character recognition.

![Captura de tela 2024-03-13 091922](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/c8e7e78b-cc72-41fc-9cb7-3e7666cb0131)

- Entre com sua conta e selecione: Try it out.
- Selecione uma das imagens padrões ou em seu computador e faça os testes.

![Captura de tela 2024-03-13 105803](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/aca005c2-7be7-46fb-b647-b8dffdafc497)

### Analise de imagem

- Acesse o Add captions to images.

![Captura de tela 2024-03-13 092721](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/9df42edb-0a4d-44ea-977d-a7fdbee7bcb7)

- Entre com sua conta e selecione: Try it out.
- Selecione uma das imagens padrões ou em seu computador e faça os testes. No lado da imagem verá o texto dessa imagem.

![Captura de tela 2024-03-13 110541](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/b16223ee-2ffd-435b-8d55-f51b07d93933)

<h3 align="center"> Two <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> <img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30px"> Of Dalila...</h3>
<div align="center"  style="display: inline-block">
  <a href="https://www.linkedin.com/in/dalila-cust%C3%B3dio-046076181/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  <a href = "mailto:dalila.dalila70@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://instagram.com/dalila.dalila70" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a target="_blank" href="https://api.whatsapp.com/send?phone=5588997138541"><img  alt="Whatsapp" width="117px" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a> 
</div>
