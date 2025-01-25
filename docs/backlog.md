# Backlog de Requisitos

## Definição
O backlog de requisitos é uma lista priorizada e organizada que contém todas as funcionalidades, melhorias, correções de bugs e mudanças desejadas para um projeto de software. Ele é desenvolvido a partir das necessidades e expectativas dos usuários finais, stakeholders e da equipe de desenvolvimento. É uma ferramenta essencial em metodologias ágeis, como Scrum e Kanban, mas também pode ser utilizada em outros processos de desenvolvimento de software.

No backlog, os itens são frequentemente chamados de user stories (histórias de usuário) ou requisitos, que descrevem o que o sistema deve fazer ou oferecer para atender às necessidades dos usuários. Cada item do backlog possui informações sobre a sua prioridade, complexidade e objetivos, permitindo que a equipe compreenda claramente o que deve ser desenvolvido.

## Backlog

Segue a tabela com os requisitos numerados e sua rastreabilidade:

| ID     | Número do Requisito | Descrição do Requisito                                                                                                                                       | Categoria               |
|--------|---------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|
| US:01  | REQ01              | Fazer login no aplicativo com email e senha para acessar as funcionalidades.                                                                                | Autenticação            |
| US:02  | REQ02              | Recuperar senha de acesso para realizar login.                                                                                                              | Autenticação            |
| US:03  | REQ03              | Trocar de conta e mudar dados da conta pessoal.                                                                                                             | Configuração de Conta   |
| US:04  | REQ04              | Realizar o cadastro no aplicativo, com campos obrigatórios validados (nome, email, senha) e redirecionamento para a tela inicial após o cadastro.            | Cadastro                |
| US:05  | REQ05              | Validar campos no cadastro para evitar campos em branco ou formato inválido.                                                                                | Cadastro                |
| US:06  | REQ06              | Receber mensagem de confirmação após concluir o cadastro.                                                                                                   | Feedback                |
| US:07  | REQ07              | Acessar o aplicativo com a conta Google para integrar contas.                                                                                               | Autenticação            |
| US:08  | REQ08              | Exibir botões para login com Google na tela inicial.                                                                                                        | Interface do Usuário    |
| US:09  | REQ09              | Acessar a conta utilizando o Facebook para login rápido.                                                                                                    | Autenticação            |
| US:10  | REQ10              | Definir o tipo de usuário (Estudante ou Turista) durante o cadastro para oferecer rotas personalizadas.                                                     | Personalização          |
| US:11  | REQ11              | Acessar o itinerário completo de um ônibus, com todas as paradas listadas em ordem.                                                                         | Informações de Rotas    |
| US:12  | REQ12              | Buscar itinerários por número da linha.                                                                                                                     | Busca                   |
| US:13  | REQ13              | Visualizar o horário estimado de espera por uma viagem.                                                                                                     | Informações de Rotas    |
| US:14  | REQ14              | Clicar no ônibus para ver detalhes da linha e próxima parada.                                                                                               | Interatividade          |
| US:15  | REQ15              | Visualizar no mapa onde o ônibus está em tempo real.                                                                                                        | Mapas e Geolocalização  |
| US:16  | REQ16              | Filtrar estações disponíveis por tipo de transporte (ônibus, metrô, etc.).                                                                                  | Filtro                  |
| US:17  | REQ17              | Receber notificações quando o ônibus estiver próximo da parada.                                                                                            | Notificações            |
| US:18  | REQ18              | Visualizar todas as estações próximas para escolher a mais conveniente.                                                                                     | Mapas e Geolocalização  |
| US:19  | REQ19              | Buscar rotas específicas em uma estação, listando as opções disponíveis.                                                                                    | Busca                   |
| US:20  | REQ20              | Filtrar estações por tipo de transporte e distância.                                                                                                        | Filtro                  |
| US:21  | REQ21              | Visualizar todas as rotas disponíveis em uma estação.                                                                                                       | Informações de Rotas    |
| US:22  | REQ22              | Obter rotas no mapa até uma estação selecionada.                                                                                                            | Mapas e Geolocalização  |
| US:23  | REQ23              | Usar mapa interativo para encontrar estações próximas.                                                                                                      | Interatividade          |
| US:24  | REQ24              | Visualizar rotas no mapa até uma estação selecionada.                                                                                                       | Mapas e Geolocalização  |
| US:25  | REQ25              | Saber o tempo estimado e o modo de locomoção sugerido (a pé, bicicleta, etc.) para chegar a uma estação.                                                    | Planejamento            |
| US:26  | REQ26              | Visualizar a rota até uma estação selecionada.                                                                                                              | Mapas e Geolocalização  |
| US:27  | REQ27              | Receber opções de rotas com diferentes modos de transporte e seus tempos estimados.                                                                         | Planejamento            |
| US:28  | REQ28              | Visualizar o tempo estimado para cada rota.                                                                                                                 | Informações de Rotas    |
| US:29  | REQ29              | Comparar o tempo estimado entre diferentes rotas.                                                                                                           | Planejamento            |
| US:30  | REQ30              | Visualizar no Moovit a disponibilidade de aplicativos de transporte em tempo real.                                                                          | Integração              |
| US:31  | REQ31              | Ver o preço estimado da corrida por aplicativos de transporte.                                                                                              | Integração              |
| US:32  | REQ32              | Visualizar no mapa a localização em tempo real dos ônibus.                                                                                                  | Mapas e Geolocalização  |
| US:33  | REQ33              | Receber previsão de chegada na próxima parada.                                                                                                             | Informações de Rotas    |
| US:34  | REQ34              | Visualizar a descrição completa de uma linha de ônibus ou metrô.                                                                                            | Informações de Rotas    |
| US:35  | REQ35              | Receber notificações sobre mudanças na operação de uma linha.                                                                                               | Notificações            |
| US:36  | REQ36              | Visualizar todas as estações de metrô próximas com informações relevantes para a viagem.                                                                    | Mapas e Geolocalização  |
| US:37  | REQ37              | Receber orientações para chegar à estação mais próxima.                                                                                                     | Planejamento            |
| US:38  | REQ38              | Visualizar rotas seguras para ciclistas.                                                                                                                    | Informações de Rotas    |
| US:39  | REQ39              | Receber opções de rotas a pé até o destino.                                                                                                                 | Planejamento            |
| US:40  | REQ40              | Visualizar rotas integradas de ônibus para trajetos mais rápidos e eficientes.                                                                              | Planejamento            |
| US:41  | REQ41              | Configurar preferências de integração entre rotas para evitar atrasos.                                                                                      | Personalização          |
| US:42  | REQ42              | Receber notificações de proximidade para saber o momento de descer.                                                                                         | Notificações            |
| US:43  | REQ43              | Ser avisado sobre mudanças no trajeto em tempo real.                                                                                                        | Notificações            |
| US:44  | REQ44              | Ser alertado sobre alterações na rota em tempo real.                                                                                                        | Notificações            |
| US:45  | REQ45              | Salvar rotas favoritas para acesso rápido.                                                                                                                  | Personalização          |
| US:46  | REQ46              | Acessar rapidamente as rotas mais utilizadas.                                                                                                              | Personalização          |
| US:47  | REQ47              | Programar trajetos considerando o horário exato de chegada.                                                                                                | Planejamento            |
| US:48  | REQ48              | Comparar rotas pelo tempo de deslocamento.                                                                                                                  | Planejamento            |
| US:49  | REQ49              | Visualizar o custo de cada rota para escolher a mais acessível.                                                                                             | Informações de Rotas    |
| US:50  | REQ50              | Programar trajetos considerando o horário de chegada.                                                                                                       | Planejamento            |
| US:51  | REQ51              | Visualizar o horário de saída estimado para evitar longas esperas.                                                                                          | Planejamento            |
| US:52  | REQ52              | Visualizar anúncios não invasivos.                                                                                                                          | Monetização             |
| US:53  | REQ53              | Poder pular anúncios.                                                                                                                                       | Monetização             |
| US:54  | REQ54              | Assinar plano premium para navegar sem anúncios e compartilhar a localização com contatos de segurança.                                                     | Monetização             |

## Requisitos Não Funcionais

| **ID**    | **Descrição do Requisito Não Funcional**                                                                                 | **Categoria**              |
|-----------|-------------------------------------------------------------------------------------------------------------------------|----------------------------|
| **RNF01** | O sistema deve ser capaz de suportar até 10.000 acessos simultâneos sem degradação significativa de desempenho.           | Desempenho                 |
| **RNF02** | O tempo de carregamento das telas deve ser inferior a 3 segundos em 90% dos casos, em uma conexão de internet de 5 Mbps. | Desempenho                 |
| **RNF03** | O sistema deve estar disponível 99,9% do tempo, com exceção de janelas de manutenção programadas.                        | Disponibilidade            |
| **RNF04** | Todos os dados do usuário devem ser armazenados e transmitidos usando criptografia AES-256.                              | Segurança                  |
| **RNF05** | O sistema deve ser compatível com os navegadores mais recentes (Chrome, Firefox, Safari, Edge) e suas duas últimas versões. | Compatibilidade            |
| **RNF06** | A interface do usuário deve ser responsiva, garantindo boa usabilidade em dispositivos móveis, tablets e desktops.      | Usabilidade                |
| **RNF07** | O sistema deve fornecer suporte a leitores de tela para garantir acessibilidade a usuários com deficiência visual.       | Acessibilidade             |
| **RNF08** | Legendas devem estar disponíveis para todos os conteúdos multimídia, como vídeos e tutoriais.                           | Acessibilidade             |
| **RNF09** | O aplicativo deve ser desenvolvido de forma modular para facilitar manutenção e futuras extensões de funcionalidade.     | Manutenibilidade           |
| **RNF10** | Logs de acesso e operação devem ser registrados e armazenados por no mínimo 180 dias.                                   | Monitoramento              |
| **RNF11** | O sistema deve suportar múltiplos idiomas, com possibilidade de fácil adição de novas traduções.                        | Internacionalização        |
| **RNF12** | A base de dados deve ser escalável horizontalmente para acomodar o crescimento do número de usuários.                   | Escalabilidade             |
| **RNF13** | O sistema deve estar em conformidade com a LGPD (Lei Geral de Proteção de Dados).                                       | Conformidade               |
| **RNF14** | O suporte técnico deve estar disponível em horário comercial com tempo de resposta de até 24 horas úteis.               | Suporte                    |
| **RNF15** | Deve haver documentação detalhada para desenvolvedores e usuários finais.                                               | Documentação               |
| **RNF16** | O sistema deve oferecer um tempo de recuperação de desastres (RTO) de até 4 horas.                                      | Recuperação de Desastres   |
| **RNF17** | O contraste de cores utilizado no sistema deve estar em conformidade com o padrão WCAG 2.1 (nível AA ou superior).          | Acessibilidade     |
| **RNF18** | Todos os elementos interativos (botões, links, menus) devem ser navegáveis exclusivamente pelo teclado.                     | Acessibilidade     |
| **RNF19** | O sistema deve fornecer notificações e mensagens de erro que sejam compreensíveis por leitores de tela.                     | Acessibilidade     |
| **RNF20** | Deve ser possível aumentar ou diminuir o tamanho do texto em pelo menos 200% sem perda de funcionalidade.                   | Acessibilidade     |
| **RNF21** | O sistema deve incluir descrições alternativas (atributo `alt`) para todas as imagens relevantes no aplicativo.              | Acessibilidade     |
| **RNF22** | O sistema deve oferecer suporte para navegação por voz em dispositivos compatíveis, como assistentes virtuais.              | Acessibilidade     |
| **RNF23** | Deve haver suporte para layouts de alto contraste configuráveis pelo usuário.                                               | Acessibilidade     |
| **RNF24** | O sistema deve permitir que o usuário escolha entre múltiplos modos de entrada, como teclado, mouse e dispositivos táteis.  | Acessibilidade     |
| **RNF25** | Deve ser fornecido um guia de acessibilidade em formato digital, com instruções detalhadas sobre como usar o sistema.       | Acessibilidade     |
