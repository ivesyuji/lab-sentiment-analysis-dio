# Desvendando a Análise de Sentimentos com Language Studio no Azure AI

Este espaço foi criado para documentar minha jornada prática e o aprendizado adquirido no desafio de aprofundar o uso das ferramentas Azure Speech Studio e Language Studio. Aqui, você vai encontrar resumos, anotações e insights sobre como a Inteligência Artificial pode ser aplicada na análise de fala e linguagem natural.

O objetivo principal desse laboratório foi desenvolver habilidades práticas na criação de soluções baseadas em IA para voz e texto. Este README.md serve como um guia detalhado, registrando as etapas realizadas e as conclusões obtidas, funcionando como um material de apoio valioso para estudos futuros e implementações.


## **Passo 01: Criação do Recurso de Linguagem no Azure**

Para começar, precisamos provisionar o serviço de Language no Azure, que será a base para nossa análise de sentimentos.

1. Acesse o **Portal do Azure** em [https://portal.azure.com](https://portal.azure.com) e faça login com sua conta Microsoft.
2. No menu superior esquerdo (as três barras), navegue até **"IA + Machine Learning"** e selecione **"Language"**. Em seguida, clique em **"Criar"**.

![[Passo 01.png]]
    
3. Confirme sua intenção clicando em **"Continuar"**.

![[Captura de tela 2025-06-08 174134.png]]
    
4. Preencha as informações básicas para o seu novo recurso:

- **Assinatura:** Selecione sua assinatura Azure.
- **Grupo de Recursos:** Escolha um grupo de recursos existente ou crie um novo para organizar seus serviços.
- **Nome:** Forneça um nome **exclusivo** para seu recurso de linguagem (ex: `meu-language-service-dio`).
- **Nível de Preço:** Selecione **S (1K chamadas por minuto)**. Este nível oferece a capacidade necessária para a maioria dos testes.
- **Região de Pesquisa do Azure:** Escolha qualquer localização disponível próxima a você (ex: "Brazil South" ou "East US").
- **Nível de Preço da Pesquisa do Azure:** Selecione **F (Gratuito - 3 índices)**. Se esta opção não estiver disponível, escolha **Padrão S (50 índices)**.

![[Passo 03.png]]

5. Clique em **Revisar e Criar** e, em seguida, em **Criar** . Aguarde a implantação do serviço de idioma que dará suporte à sua base de conhecimento de resposta a perguntas personalizada.

## Passo 02 - Acessar o Language Studio

Com o recurso de linguagem provisionado, agora podemos acessar o Language Studio para realizar a análise.

1. Em uma nova guia do navegador, abra o **Azure AI Language Studio** em [https://language.azure.com](https://language.azure.com/?azure-portal=true) e faça login com a conta da Microsoft associada à sua assinatura do Azure.
    
2. Na tela inicial do Language Studio, na seção "Classificar texto", clique em **"Analisar sentimentos e minerar opiniões"**.

![[Pasted image 20250608175118.png]]
    
3. Você será direcionado para a interface de análise. Aqui, você pode colar seu texto, selecionar o idioma e executar a análise.
    
    - **Exemplo de Texto:** Utilizei um trecho de um review de mouse do Reddit (disponível em [https://www.reddit.com/r/MouseReview/comments/1gc65ab/hitscan_hyperlight_review/](https://www.reddit.com/r/MouseReview/comments/1gc65ab/hitscan_hyperlight_review/))

4. Após inserir o texto e selecionar o idioma, clique no botão **"Run"** para executar a análise.

![[Pasted image 20250608180008.png]]

## Resultados

![[Pasted image 20250608180302.png]]

![[Pasted image 20250608180353.png]]

![[Pasted image 20250608180409.png]]

![[Pasted image 20250608180428.png]]

![[Pasted image 20250608180449.png]]

![[Pasted image 20250608180459.png]]
![[Pasted image 20250608180549.png]]

![[Pasted image 20250608180533.png]]
## Conclusão

Este laboratório foi uma jornada prática imersiva no universo da Inteligência Artificial aplicada à análise de fala e linguagem natural com os serviços do Azure. Ao longo do processo, aprendi como funciona a criação de recursos no Azure e, ao mesmo tempo, pude explorar e compreender como a Inteligência Artificial interpreta e extrai insights significativos de dados de voz e texto.

Essa experiência me permitiu não só configurar e gerenciar serviços de IA na nuvem, mas também entender a profundidade da análise que pode ser feita. Desde a identificação de sentimentos até a organização de informações complexas, a prática demonstrou o poder do Azure AI em transformar dados brutos em conhecimento acionável.
