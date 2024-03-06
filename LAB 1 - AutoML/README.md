# automl-microsoft-azure
- Passo a passo de experimento de Aprendizagem Automatizado, de Regressão, usando a Azure Machine Learning.
- Feito desafio de projeto no Bootcamp Microsoft Azure AI Fundamentals Na [Dio.me](https://www.dio.me/) com [Documentação](https://aka.ms/ai900-auto-ml).
<br>

## Passo 1
- Criar uma conta no [https://azure.microsoft.com/pt-br/free].
- O cadastro é criado quando clicar nesse botão "Experimentar gratuitamente" (É preciso dizer um número de cartão de crédito).

![Captura de tela 2024-03-06 101816](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/008f138d-ab03-4c24-8b27-9fe9c5b3753e)
<br>

## Passo 2
- Entrar na plataforma do [Portal Azure](https://portal.azure.com).
- Pesquisar por "Azure Machine Learning" nesse campo de pesquisa selecionar Azure Machine Learning.

![Captura de tela 2024-03-06 102853](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/cc101740-9e2a-4d73-b063-6c5006025869)
<br>

## Passo 3
- Apertar em "Criar", para criar um Novo workspace.

![Captura de tela 2024-03-06 103407](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/97061017-ee2b-441c-90cd-9e9b8480184e)
<br>

## Passo 4
- Criar um novo "resource group", criar um "nome", a "região", e Apertar em "Examinar + criar".

![Captura de tela 2024-03-06 104345](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/81074373-4037-4f09-bf99-556818533ccc)

- Esperar até que a validação ser aprovada, e então Apertar em "criar".

![Captura de tela 2024-03-06 110313](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/a2e8c625-5c01-42c9-bd3e-d654f906d26c)
<br>

## Passo 5
- A implantação está em andamento e pode ser acompanhada na tela que será aberta automaticamente.

![Captura de tela 2024-03-06 110933](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/95803d17-99ba-4660-ba1a-cb25d951f842)
- Esta é a tela de finalização do deploy. Agora podemos Apertar em "ir para o recurso".

![Captura de tela 2024-03-06 111044](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/fe77635a-7c58-4092-a051-b33ac774deec)

- Na tela do recurso, apertar em "Iniciar estúdio".

![Captura de tela 2024-03-06 112247](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/82e5dfd4-2a8a-478c-a0b5-428455fbb9c1)
<br>

## Passo 6
- O diretório do workspace é então aberto.
- Posso visualizar todos os workspaces existentes, Apertando em "Todos os Espaços de Trabalho".

![Captura de tela 2024-03-06 112957](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/f184eba8-a9c7-47b9-8c97-b6f9bee2f7ac)

-  Aperte No workspace que você criou.

![Captura de tela 2024-03-06 113608](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6b772465-e21b-4583-845c-c66161883303)
<br>

## Passo 7
- O workspace escolhido é aberto. Aperte no ambiente "ML automatizado" e Apertar em criar um "Novo trabalho de ML automatizado".

![Captura de tela 2024-03-06 114224](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/684366ac-3dcf-493d-a6b0-76f12db620e9)

![Captura de tela 2024-03-06 115219](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/07106550-c60c-4c6f-a7be-33d9bb5b0f54)
<br>

## Passo 7
- Preencher os dados do job com as informações (fornecidas pela documentação da Microsoft).
- 7.1 -> Preenchimento das informações básicas. Quando Terminar de Preencher Aperte em Avançar.

![Captura de tela 2024-03-06 120152](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/bb05e9ba-9280-4dd0-baa6-d906598a7da1)

- 7.2 -> Escolha do tipo de tarefa (Regressão) e Aperte em criar.

![Captura de tela 2024-03-06 120658](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/f961da10-e3f0-4a9d-8a8d-1213f8f9c752)

- 7.3 -> Preencha as informações e Aperte em Avançar.
  
![Captura de tela 2024-03-06 121326](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/adbedbc3-943b-47b9-b675-de8e6abbc20b)

- 7.4 -> Escolha a fonte dos dados e Aperte em Avançar.

![Captura de tela 2024-03-06 121555](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/680456a5-5bde-4815-a869-29e66977128b)

- 7.5 -> Escreva a url e Aperte em Avançar. A url passa por uma verificação e validação.

![Captura de tela 2024-03-06 122022](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e497da57-8a72-484b-88a1-73b6453ef36a)

- 7.6 -> Os dados devem estar com as seguintes configurações e quando terminar de preencher apertar em Avançar.

![Captura de tela 2024-03-06 122507](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/6732f05e-b4fc-45bc-9bb0-4d6d5eb07b24)

- 7.7 -> Ele traz uma visualização do Esquema. Não é necessário alterar nenhuma informação e Aperte em Avançar.

![Captura de tela 2024-03-06 122919](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/1ae74e3c-73d0-48a1-9152-68b64b98cf64)

- 7.8 -> Por fim, ele traz todas informações para Examinar, e Aperte em "criar", para criar o Base de Dados.

![Captura de tela 2024-03-06 123253](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e78210c3-852e-4324-96ee-82fb8202c131)

- 7.9 -> Para avançar, selecione a Base de Dados, e Aperte em "Avançar".

![Captura de tela 2024-03-06 123625](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/b90b65d0-d981-4cfa-8578-db4d0a445391)

- 7.10 -> Configurações da tarefa.

![Captura de tela 2024-03-06 124557](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/8f3ee26a-620e-4477-b022-98b42af08c50)

![Captura de tela 2024-03-06 124701](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/aa3ed6e8-331e-4d02-a648-fb676fe08975)

![Captura de tela 2024-03-06 125016](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/07f18a6f-ae4b-481f-8239-270977920c2f)

- 7.11 -> Não é preciso escrever nenhuma informação diferente na tela Computação.

![Captura de tela 2024-03-06 130147](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/e08117f5-88dd-4eaa-9ddf-1e1117c6dc73)

- 7.12 -> As informações são trazidas e pode enviar o trabalho de treinamento.

![Captura de tela 2024-03-06 130439](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/72653e51-f5bc-4636-a8df-ff87732a7680)
<br>

## Passo 8
- O modelo inicia o treinamento até a finalização.

![Captura de tela 2024-03-06 130743](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/d9ea47c4-0b7d-4e91-a8d8-bf26f09a2079)
<br>

## Passo 9
- Validar métricas.
- 9.1 -> Acessar as informações do modelo conforme imagem abaixo.

![Captura de tela 2024-03-06 132035](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/a60a2cc3-89c1-4929-b597-920b3ac5573b)

- 9.2 -> Acessar o trabalho.

![Captura de tela 2024-03-06 132323](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/bcb59750-4037-496b-b3fa-d413cfaf207e)

- 9.3 -> Acessar as métricas.

![Captura de tela 2024-03-06 132617](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/c6ed7d82-97d5-47a5-95ed-4407103fe967)

- As métricas trazem dois gráficos, o predicted_true e o residuals, que trazem informações de valores previstos comparados com os reais.

![Captura de tela 2024-03-06 132832](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/fc39a053-e71d-4694-8bf5-ec4babac0e98)
<br>

## Passo 10
- Implantar e Teste do Modelo.
- 10.1 -> De volta à página do modelo, escolhemos a opção de Implantar Serviço Web.

![Captura de tela 2024-03-06 133349](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/93f21605-136a-4156-9df4-ce32ef043806)

- 10.2 -> Preencher com as informações fornecidas na documentação e Apertar em "Implantar".

![Captura de tela 2024-03-06 133938](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/99eab488-2e50-4134-afe6-8baac614c081)

- 10.3 -> Receberemos a notificação de que o Implantar está completo, e no menu esquerdo, vamos Apertar na aba Pontos de extremidade.

![Captura de tela 2024-03-06 134259](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/ad54433a-6927-46c6-bc35-45c889c9f98e)

- 10.4 -> Na tela de Pontos de extremidade, confirma o status "Succeeded" do Implantar, e Apertamos na aba "Testar"

![Captura de tela 2024-03-06 135510](https://github.com/DalilaDeveloperMobile/dio-practice-microsoft-azure-ai-fundamentals/assets/29806802/533a3ab1-b9a5-4c71-a298-4b4b9a887590)


