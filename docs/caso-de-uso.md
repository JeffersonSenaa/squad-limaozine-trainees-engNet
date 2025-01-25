# Caso de uso

## Definição:
Um caso de uso é uma descrição detalhada de como os usuários (ou outros sistemas) interagem com um sistema para alcançar um objetivo específico. Ele é utilizado na análise e design de sistemas para documentar os requisitos funcionais de forma clara e compreensível.

## UC01: Fazer Login

### Breve Descrição
Permite que o usuário faça login no aplicativo utilizando e-mail e senha cadastrados.

### Atores
- Usuário

### Fluxo Principal
1. O sistema apresenta a tela de login.
2. O usuário insere o e-mail e a senha.
3. O sistema valida as credenciais fornecidas.
4. O sistema redireciona o usuário para a tela inicial.

### Fluxos Alternativos
1. **Recuperação de Senha**:
    - O usuário seleciona "Esqueci minha senha".
    - O sistema solicita o e-mail cadastrado.
    - O sistema envia um link para redefinição de senha ao e-mail fornecido.
    - O usuário redefine sua senha e retorna à tela de login.

### Fluxos de Exceção
1. **Credenciais Inválidas**:
    - Ocorre no passo 3 do fluxo principal, caso o e-mail ou senha estejam incorretos.
    - O sistema exibe uma mensagem de erro e retorna à tela de login.

---

## UC02: Cadastrar Usuário

### Breve Descrição
Permite que novos usuários se registrem no aplicativo fornecendo informações básicas, como e-mail e senha.

### Atores
- Usuário

### Fluxo Principal
1. O sistema apresenta a tela de cadastro.
2. O usuário insere e-mail, senha e outros dados obrigatórios.
3. O sistema valida as informações fornecidas.
4. O sistema confirma o cadastro com uma mensagem de sucesso.

### Fluxos Alternativos
1. **Campos Não Preenchidos**:
    - Ocorre no passo 2 do Fluxo Principal, caso algum campo obrigatório não seja preenchido.
    - O sistema exibe uma mensagem de erro e solicita o preenchimento dos campos.

### Fluxos de Exceção
1. **Formato Inválido de Dados**:
    - Ocorre no passo 3 do Fluxo Principal, caso os dados inseridos não atendam aos requisitos.
    - O sistema exibe uma mensagem indicando o formato correto e retorna à tela de cadastro.

---

## UC03: Conectar Conta Google ou Facebook

### Breve Descrição
Permite que os usuários acessem o aplicativo utilizando suas contas do Google ou Facebook.

### Atores
- Usuário
- Google API
- Facebook API

### Fluxo Principal
1. O sistema apresenta botões para login com Google e Facebook.
2. O usuário seleciona uma das opções.
3. O sistema redireciona para a autenticação na plataforma escolhida.
4. O sistema valida as credenciais e redireciona para a tela inicial.

### Fluxos Alternativos
1. **Usuário Já Autenticado**:
    - Ocorre no passo 2 do fluxo principal, caso o usuário já esteja autenticado.
    - O sistema redireciona diretamente para a tela inicial sem necessidade de nova autenticação.

### Fluxos de Exceção
1. **Erro na Conexão com API**:
    - Ocorre no passo 3 do fluxo principal, caso a conexão com a API falhe.
    - O sistema apresenta uma mensagem de erro e sugere tentar novamente mais tarde.

---

## UC04: Definirdo Tipo de Usuário

### Breve Descrição
Permite que o usuário defina o seu tipo durante o cadastro, personalizando o aplicativo para suas necessidades.

### Atores
- Usuário

### Fluxo Principal
1. O sistema apresenta as opções de tipo de usuário durante o cadastro.
2. O usuário seleciona uma opção.
3. O sistema ajusta as funcionalidades do aplicativo de acordo com o tipo selecionado.

### Fluxos Alternativos
1. **Alteração do Tipo de Usuário Após Cadastro**:
    - O usuário acessa a funcionalidade de perfil para alterar o tipo de usuário configurado.
    - O sistema atualiza as funcionalidades de acordo com a nova seleção.

### Fluxos de Exceção
1. **Erro ao Salvar Tipo de Usuário**:
    - Ocorre no passo 3 do fluxo principal, caso haja falha ao salvar a seleção.
    - O sistema exibe uma mensagem de erro e retorna à tela de cadastro.

---

## UC05: Acessar ao Itinerário de Ônibus

### Breve Descrição
Permite que o usuário visualize o itinerário completo de uma linha de ônibus, incluindo horários e paradas.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de itinerários.
2. O sistema apresenta uma lista de linhas disponíveis.
3. O usuário seleciona uma linha.
4. O sistema apresenta o itinerário da linha escolhida.

### Fluxos Alternativos
1. **Filtragem de Linhas**:
    - O usuário aplica filtros, como horário ou direção, para visualizar apenas as linhas de interesse.
    - O sistema atualiza a lista de linhas disponíveis com base nos critérios aplicados.

### Fluxos de Exceção
1. **Linha Não Encontrada**:
    - Ocorre no passo 3 do fluxo principal, caso a linha selecionada não esteja cadastrada no sistema.
    - O sistema exibe uma mensagem de erro e retorna à lista de linhas.

---

## UC06: Ver a Localização dos Ônibus em Tempo Real

### Breve Descrição
Permite que o usuário visualize a localização em tempo real de um ônibus em uma linha selecionada.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de localização.
2. O sistema apresenta as linhas disponíveis para monitoramento.
3. O usuário seleciona uma linha.
4. O sistema exibe a localização em tempo real dos ônibus daquela linha.

### Fluxos Alternativos
1. **Configuração de Alertas**:
    - O usuário configura alertas para ser notificado quando o ônibus estiver próximo a uma parada específica.
    - O sistema ativa o monitoramento e envia notificações conforme configurado.

### Fluxos de Exceção
1. **Erro no Monitoramento**:
    - Ocorre no passo 4 do fluxo principal, caso o sistema não consiga recuperar os dados de localização.
    - O sistema exibe uma mensagem de erro e sugere tentar novamente mais tarde.


---

## UC07: Ver as Estações Disponíveis

### Breve Descrição
Permite que o usuário visualize as estações próximas para selecionar a mais conveniente para sua rota.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de estações.
2. O sistema exibe as estações disponíveis e suas localizações.
3. O usuário escolhe uma estação para mais detalhes.
4. O sistema exibe as informações da estação selecionada.

### Fluxos Alternativos
1. **Ordenação das Estações**:
    - O usuário altera a ordenação das estações exibidas.
    - O sistema atualiza a lista de estações com base nos critérios de ordenação selecionados.

### Fluxos de Exceção
1. **Erro ao Carregar Estações**:
    - Ocorre no passo 2 do fluxo principal, caso o sistema não consiga carregar as estações disponíveis.
    - O sistema exibe uma mensagem de erro e retorna à tela inicial.

---

## UC08: Visualizar Rotas até Estação

### Breve Descrição
Permite que o usuário visualize todas as rotas disponíveis em uma estação selecionada.

### Atores
- Usuário

### Fluxo Principal
1. O usuário seleciona uma estação.
2. O sistema exibe todas as rotas disponíveis naquela estação.
3. O usuário escolhe uma rota para mais detalhes.
4. O sistema exibe as informações da rota selecionada.

### Fluxos Alternativos
1. **Filtragem de Rotas**:
    - O usuário aplica filtros, como tipo de transporte ou destino final, para visualizar apenas rotas específicas.
    - O sistema atualiza a lista de rotas disponíveis com base nos critérios aplicados.

### Fluxos de Exceção
1. **Rota Não Encontrada**:
    - Ocorre no passo 3 do fluxo principal, caso a rota escolhida não esteja disponível.
    - O sistema exibe uma mensagem de erro e retorna à lista de rotas.
---

## UC09: Visualizar Mapa Interativo para Localização das Estações

### Breve Descrição
Permite que o usuário utilize um mapa interativo para localizar estações próximas.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa no aplicativo.
2. O usuario clica em estações.
3. O usuário seleciona uma estação no mapa.
4. O sistema exibe as informações detalhadas da estação selecionada.

### Fluxos Alternativos
1. **Mudança de Escala no Mapa**:
    - O usuário ajusta a escala do mapa para visualizar estações em uma área maior ou menor.
    - O sistema atualiza a exibição das estações conforme a nova escala definida.

### Fluxos de Exceção
1. **Internet desconectada**:
    - Ocorre no passo 2 do fluxo principal, caso a internet esteja desconectada.
    - O sistema exibe uma mensagem de erro.

---

## UC10: Visualizar Rota até a Estação

### Breve Descrição
Permite que o usuário visualize a rota para chegar a uma estação específica.

### Atores
- Usuário

### Fluxo Principal
1. O usuário seleciona uma estação desejada.
2. O sistema exibe as opções de rotas disponíveis para chegar até essa estação.
3. O usuário escolhe a rota mais adequada.
4. O sistema apresenta o percurso detalhado até a estação.

### Fluxos Alternativos
1. **Escolha por Meio de Transporte**:
    - O usuário filtra as rotas disponíveis por meio de transporte (ex.: a pé, bicicleta, carro).
    - O sistema atualiza as opções de rotas com base na escolha do usuário.

### Fluxos de Exceção
1. **Erro ao Carregar Rotas**:
    - Ocorre no passo 2 do fluxo principal, caso o sistema não consiga carregar as rotas disponíveis.
    - O sistema exibe uma mensagem de erro e sugere tentar novamente mais tarde.

---

## UC11: Visualizar Tempo Estimado da Viagem

### Breve Descrição
Permite que o usuário visualize o tempo estimado de viagem para cada rota disponível.

### Atores
- Usuário

### Fluxo Principal
1. O usuário seleciona uma rota.
2. O sistema calcula o tempo estimado de viagem com base nas condições atuais.
3. O sistema exibe o tempo estimado para o usuário.

### Fluxos Alternativos
1. **Comparação entre Rotas**:
    - O usuário seleciona várias rotas para comparar seus tempos estimados de viagem.
    - O sistema exibe um resumo comparativo das rotas selecionadas.

### Fluxos de Exceção
N/A

---

## UC12: Integrar com Aplicativos de Transporte

### Breve Descrição
Permite que o usuário integre o aplicativo com outros serviços de transporte, como Uber.

### Atores
- Usuário
- Serviços de transporte externos

### Fluxo Principal
1. O sistema apresenta opções de aplicativos de transporte disponíveis.
2. O usuário seleciona um aplicativo para integração.
3. O sistema redireciona o usuário para o aplicativo escolhido.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
1. **Erro na Conexão com Serviço Externo**:
    - Ocorre no passo 3 do fluxo principal, caso o sistema não consiga se conectar ao serviço externo.
    - O sistema direciona o usuário para baixar o aplicativo.

---

## UC13: Consultar Ônibus

### Breve Descrição
Permite que o usuário consulte informações detalhadas sobre uma linha de ônibus específica.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de consulta de ônibus.
2. O sistema solicita o número ou nome da linha desejada.
3. O usuário insere as informações solicitadas.
4. O sistema exibe os detalhes da linha, incluindo itinerário, horários e localização atual.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
N/A

---

## UC14: Descrever a Linha

### Breve Descrição
Permite que o usuário visualize a descrição completa de uma linha de ônibus ou metrô.

### Atores
- Usuário

### Fluxo Principal
1. O usuário seleciona uma linha para mais informações.
2. O sistema exibe a descrição completa da linha e detalhes do percurso.

### Fluxos Alternativos
1. **Visualização de Ponto Específico**:
    - O usuário seleciona um ponto específico da linha para mais informações (ex.: horários de chegada).
    - O sistema apresenta os detalhes referentes ao ponto selecionado.

### Fluxos de Exceção
N/A

---

## UC15: Visualizar Estações de Metrô

### Breve Descrição
Permite que o usuário visualize todas as estações de metrô próximas e informações relevantes sobre elas.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de estações de metrô.
2. O sistema exibe uma lista das estações próximas e suas localizações.
3. O usuário seleciona uma estação para visualizar mais detalhes.
4. O sistema apresenta as informações detalhadas da estação selecionada.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
N/A

---

## UC16: Visualizar rotas de Bicicleta e Caminhada

### Breve Descrição
Permite que o usuário visualize rotas seguras para ciclistas ou trajetos a pé até o destino selecionado.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de rotas de bicicleta ou caminhada.
2. O sistema solicita o destino desejado.
3. O usuário insere o destino.
4. O sistema apresenta as rotas disponíveis com informações detalhadas.

### Fluxos Alternativos
1. **Seleção por Tipo de Rota**:
    - O usuário filtra as rotas por nível de tempo estimado.
    - O sistema atualiza as opções de rotas disponíveis com base nos critérios aplicados.

### Fluxos de Exceção
1. **Erro ao Carregar Rotas**:
    - Ocorre no passo 4 do fluxo principal, caso o sistema não consiga recuperar as rotas.
    - O sistema exibe uma mensagem de erro e retorna à tela inicial.

---

## UC17: Integrar entre Rotas de Ônibus

### Breve Descrição
Permite que o usuário planeje trajetos integrados entre diferentes rotas de ônibus, considerando o menor tempo de espera entre conexões.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de integração entre rotas.
2. O sistema solicita o ponto de origem e destino.
3. O usuário insere as informações solicitadas.
4. O sistema exibe as opções de trajetos integrados, ordenados pelo menor tempo de espera.
5. O usuário seleciona a opção desejada.
6. O sistema apresenta o trajeto detalhado.

### Fluxos Alternativos
1. **Alteração de Parâmetros de Busca**:
    - Ocorre no passo 4 do fluxo principal, caso o usuário deseje ajustar os parâmetros de origem, destino ou preferências.
    - O sistema atualiza as opções de trajetos com base nos novos parâmetros fornecidos.

### Fluxos de Exceção
N/A

---

## UC18: Avisar Proximidade

### Breve Descrição
Permite que o usuário receba notificações quando o ônibus estiver próximo ao ponto.

### Atores
- Usuário

### Fluxo Principal
1. O sistema monitora a localização do ônibus em tempo real.
2. Quando o ônibus estiver próximo ao ponto configurado, o aplicativo mostra ao usuário.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
1. **Erro no Monitoramento**:
    - Ocorre no passo 2 do fluxo principal, caso o sistema não consiga monitorar a localização do ônibus.
    - O sistema não mostra para o usuário a aproximidade.

---

## UC19: Notificar Alteração de Rota em Tempo Real

### Breve Descrição
Permite que o usuário seja avisado sobre mudanças no trajeto de sua rota em tempo real, para evitar atrasos inesperados.

### Atores
- Usuário

### Fluxo Principal
1. O sistema monitora a rota configurada pelo usuário.
2. O sistema detecta uma alteração no trajeto.
3. O sistema envia uma notificação ao usuário informando a mudança e sugerindo alternativas, se aplicável.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
1. **Erro na Detecção de Alterações**:
    - Ocorre no passo 2 do fluxo principal, caso o sistema não consiga identificar alterações na rota.
    - O sistema exibe uma mensagem genérica indicando que o monitoramento está indisponível.

---

## UC20: Mostrar Rotas Favoritas e Mais Utilizadas

### Breve Descrição
Permite que o usuário salve rotas favoritas para acessá-las rapidamente ou visualize as rotas mais utilizadas com base em seu histórico.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de rotas favoritas.
2. O sistema exibe as rotas salvas pelo usuário.
3. O usuário seleciona uma rota favorita para mais detalhes.

### Fluxos Alternativos
1. **Adicionar Nova Rota Favorita**:
    - O usuário opta por adicionar uma nova rota favorita durante a navegação.
    - O sistema salva a rota no perfil do usuário e a exibe na lista de favoritas.
2. **Visualizar Rotas Mais Utilizadas**:
    - O sistema exibe uma lista das rotas mais frequentes do usuário com base no histórico de uso.

### Fluxos de Exceção
1. **Erro ao Carregar Rotas Favoritas**:
    - Ocorre no passo 2 do fluxo principal, caso o sistema não consiga recuperar as rotas salvas.
    - O sistema exibe uma mensagem de erro.

---


## UC21: Mostrar Opções de Rotas com Tempo e Custo

### Breve Descrição
Permite que o usuário visualize e compare as opções de rotas disponíveis com base no tempo estimado de viagem e custo de transporte.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de comparação de rotas.
2. O sistema solicita o ponto de origem e destino.
3. O usuário insere as informações solicitadas.
4. O sistema exibe as rotas disponíveis com o tempo estimado.
5. O usuário seleciona a rota desejada para mais detalhes.

### Fluxos Alternativos
1. **Alteração de Critérios de Comparação**:
    - O sistema recalcula e exibe as rotas com base nos novos critérios fornecidos.

### Fluxos de Exceção


N/A

---

## UC22: Ver Horário de Saída ou Chegada

### Breve Descrição
Permite que o usuário programe seu trajeto considerando o horário exato de saída ou chegada para evitar atrasos.

### Atores
- Usuário

### Fluxo Principal
1. O usuário acessa a funcionalidade de horários.
2. O sistema solicita o ponto de origem, destino e horário desejado (saída ou chegada).
3. O usuário insere as informações solicitadas.
4. O sistema apresenta as rotas disponíveis compatíveis com o horário especificado.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
1. **Erro ao Processar Horário**:
    - Ocorre no passo 4 do fluxo principal, caso o sistema não consiga processar as informações de horários.
    - O sistema exibe uma mensagem de erro e retorna à tela inicial.

---

## UC23: Utilizar versão gratuíta

### Breve Descrição
Permite que o usuário utilize a versão gratuita do aplicativo com anúncios exibidos.

### Atores
- Usuário

### Fluxo Principal
1. O usuário utiliza a versão gratuita do aplicativo.
2. O sistema exibe anúncios de forma intercalada durante o uso.

### Fluxos Alternativos
1. **Pular Anúncio**:
    - O sistema oferece a opção de pular anúncios em alguns casos, caso aplicável.

### Fluxos de Exceção
N/A

---

## UC24: Utilizar versão paga

### Breve Descrição
Permite que o usuário acesse a versão premium do aplicativo, realizando o pagamento online para desbloquear funcionalidades adicionais.

### Atores
- Usuário
- Sistema de Pagamento Online

### Fluxo Principal
1. O usuário acessa a funcionalidade de assinatura premium.
2. O sistema exibe as opções de planos disponíveis.
3. O usuário seleciona um plano e insere as informações de pagamento.
4. O sistema processa o pagamento e confirma a assinatura.
5. O usuário passa a ter acesso aos benefícios premium.

### Fluxos Alternativos
N/A

### Fluxos de Exceção
1. **Erro no Processamento do Pagamento**:
    - Ocorre no passo 4 do fluxo principal, caso o sistema de pagamento não consiga processar a transação.
    - O sistema exibe uma mensagem de erro e retorna à tela de planos.

---



## Histórico de Versões

| Versão | Data       | Alterações Principais  | Autor                                                                                     |
| ------ |------------|------------------------|-------------------------------------------------------------------------------------------|
| 1.0    | 25/01/2025 | Criação do caso de uso | [Ana Luíza](https://github.com/analufernanndess) |
