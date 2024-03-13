# vision-studio-microsoft-azure
 Passo a passo de experimento usando:
-  Vision Studio/ Azure AI Vision para extrair texto de imagens sem a utilização de código.
-  Com tecnologia OCR (Optical Character Recognition).
#### Realizado como desafio de projeto no Bootcamp Microsoft Azure AI Fundamentals da [Dio.me](https://www.dio.me/).

> [!NOTE]
> Esse passo a passo é somente uma forma alternativa de realizar o procedimento. Sempre dê preferência a
> [Documentação Oficial - Reconhecimento](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html), [Documentação oficial - Analise de documentos](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html) e [Documentação oficial - Analise imagens](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html).

## Passo 1
- Acessar [portal.azure.com](https://portal.azure.com/) e clicar em "Criar um recurso".
  
![Captura de tela 2024-03-08 124339](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6b52d7d3-3867-4dd1-8dc6-84741690c4f7)
<br>

## Passo 2
- Buscar por "Ai azure services" e clicar em "create"

![Captura de tela 2024-03-13 083543](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/b79ed1ed-d445-45b7-b443-ed35e0d1a138)
![Captura de tela 2024-03-13 083643](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/8419ddb1-21f6-449f-abb5-f96e61ca7cc6)
<br>

## Passo 3
- Preencher as informações mostradas abaixo. O resource group pode ser novo ou existente. Escolhi um que eu havia criado anteriormente. Depois disso, basta clicar em "review + create", e depois "create", e aguardar a finalização do deploy.
  
![Captura de tela 2024-03-13 084000](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/7fdbb19a-b93b-46b3-ae5d-59a234fe659d)

- Esta é a tela depois da finalização do deploy

![Captura de tela 2024-03-13 084125](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/5c75d8c0-2f4c-49e1-87b6-0361c1766e7b)
<br>

## Passo 4
- Assim que o serviço estiver sido criado, acessamos o [Vision Studio](https://portal.vision.cognitive.azure.com/?azure-portal=true) com as nossas credenciais e clicamos em “View all resources”.

![Captura de tela 2024-03-13 085124](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/b9d58af6-4b57-4e10-9b55-6d48c5402e58)

- Selecionamos o nosso recurso e clicarmos em “Select as default resource” e apertamos em fechar nesse X.

![Captura de tela 2024-03-13 085440](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/64e69df8-947b-451b-bb12-d7608577d8d8)


