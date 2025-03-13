# PROJETO QUAL A BOA

## 1. Definição do Produto
Bot de WhatsApp para analisar o mercado de uma possível solução de problema envolvendo informação e divulgação de produtos comercializados em bares e eventos.

O Bot tem como objetivo identificar o público alvo e analisar a viabilidade para implementação de um possível App que facilita a estrutura de consumação de eventos e estabelecimentos, oferecendo informações sobre os produtos e cardápios, visando frequentadores de eventos, principalmente adolescentes e jovens adultos, que desejam se planejar melhor  no evento, e organizadores de eventos e festas, que farão a utilização do aplicativo para melhorar a experiência de consumo e divulgação em seus eventos. A plataforma com o intuito de melhorar a experiência do consumidor e otimizar a venda do evento.

O objetivo é proporcionar uma experiência mais fluida para os clientes, gerar maior visibilidade para os estabelecimentos e aumentar o faturamento dos mesmos.

## 2. Requisitos do Sistema
Requisitos Funcionais (RF)

    1. Consulta de Estabelecimentos: O bot deve permitir que os usuários consultem bares e eventos próximos com base na localização fornecida;

    2. Informação sobre Produtos e Preços: O bot deve exibir os cardápios, preços e promoções disponíveis nos estabelecimentos cadastrados;

    3. Interação via WhatsApp: O bot deve responder aos usuários por meio de mensagens no WhatsApp, utilizando a Evolution-API;

    4. Filtragem de Estabelecimentos: O usuário deve poder filtrar estabelecimentos por tipo (bar, balada, evento) ou por promoção específica;

    5. Resposta Rápida e Automatizada: O bot deve reconhecer comandos básicos e responder de maneira estruturada e clara;

    6. Cadastro de Estabelecimentos: Os estabelecimentos devem poder cadastrar e atualizar suas informações (nome, localização, cardápio, promoções);

    7. Registro de Interações: O sistema deve armazenar consultas feitas pelos usuários para análise posterior;

    8. Dashboard de Métricas: Deve ser possível visualizar o número de acessos, consultas frequentes e horários de pico (a ser implementado futuramente).

Requisitos Não Funcionais (RNF)

    Desempenho:

        1. O bot deve responder às mensagens dos usuários em um tempo máximo de 2 segundos para garantir uma experiência fluida;

        2. A API deve ser capaz de processar múltiplas requisições simultâneas sem comprometer a velocidade de resposta;

        3. O sistema deve ser otimizado para minimizar o consumo de recursos computacionais e garantir baixa latência.

    Escalabilidade:

        1. A arquitetura do sistema deve permitir a expansão para suportar um aumento gradual no número de usuários e estabelecimentos cadastrados sem necessidade de grandes modificações;

        2. O sistema deve suportar diferentes volumes de acessos, garantindo estabilidade mesmo em horários de pico.

    Segurança:

        1. Deve haver um mecanismo de autenticação para que apenas estabelecimentos autorizados possam cadastrar ou atualizar informações sobre cardápios e promoções;

        2. As informações armazenadas devem ser protegidas contra acessos não autorizados utilizando criptografia de dados sensíveis;

        3. O bot não deve solicitar nem armazenar informações pessoais sensíveis dos usuários, garantindo conformidade com leis de proteção de dados.

    Usabilidade:

        1. O bot deve fornecer respostas estruturadas, utilizando mensagens curtas e diretas para facilitar a compreensão dos usuários;

        2. A interação com o bot deve ser intuitiva, sem necessidade de comandos complexos, garantindo acessibilidade para usuários com diferentes níveis de familiaridade com tecnologia;

        3. O sistema deve evitar a repetição excessiva de mensagens e oferecer menus dinâmicos para melhorar a experiência do usuário.

    Manutenibilidade:

        1. O código do sistema deve ser desenvolvido seguindo boas práticas de modularização e documentação, garantindo que futuras alterações e correções possam ser feitas com facilidade;

        2. O sistema deve ser projetado para permitir atualizações sem impacto na experiência dos usuários;

        3. Devem ser implementados logs e monitoramento contínuo, permitindo a rápida identificação e correção de falhas.

## 3. Restrições e Condições
Para a criação do BOT no WhatsApp, é utilizada a ferramenta Evolution-API, uma API gratuita que faz a criação de Bots no Whatsapp. A linguagem utilizada para a criação da API responsável por controlar os cálculos e respostas do BOT será TypeScript, utilizando o framework NestJS.
Será também utilizado TypeScript com o framework ReactJS para a criação de um Dashboard de visualização de acessos e métricas. Utilizaremos a metodologia ágil Scrum e Kanban, utilizando o trello para esta gestão, junto ao Clockify para as métricas envolvendo tempo de desenvolvimento e reuniões. A princípio, a ferramenta de deploy utilizada será Vercel.

(falta orçamentos e prazos de entrega)
## 5. Necessidades dos Stakeholders
Clientes (Estabelecimentos, Bares e Organizadores de Eventos)

    Divulgação e Visibilidade:

        1. Precisam de um canal acessível e de baixo custo para promover seus estabelecimentos, produtos e promoções;

        2. Desejam alcançar mais clientes, especialmente jovens adultos que frequentam eventos e bares.

    Aumento de Vendas e Planejamento de Consumo:

        1. Buscam atrair mais clientes ao divulgar promoções e preços antecipadamente;

        2. Precisam de um meio eficiente para informar sobre horários de funcionamento, eventos e produtos disponíveis.

    Facilidade de Cadastro e Atualização de Informações:

        1. Devem ter um meio simples para cadastrar e atualizar seus cardápios e promoções, sem necessidade de conhecimento técnico avançado.

    Análise de Dados e Comportamento do Consumidor:

        1. Desejam entender melhor os hábitos dos consumidores para ajustar promoções e estratégias de venda;

        2. Precisam de métricas sobre o interesse dos usuários e os estabelecimentos mais pesquisados.

Usuários Finais (Frequentadores de Bares e Eventos)

    Acesso Rápido a Informações Relevantes:

        1. Querem saber onde ir com base em localização, preços e promoções disponíveis;

        2. Desejam informações rápidas e organizadas sem precisar baixar um aplicativo.

    Planejamento do Consumo:

        1. Precisam consultar os preços antes de sair para otimizar seus gastos;

        2. Buscam saber quais estabelecimentos têm as melhores promoções e custo-benefício.

    Interação Simples e Intuitiva:

        1. Preferem uma experiência fluida sem precisar digitar comandos complicados;

        1. Desejam um bot que responda de forma clara e direta, sem mensagens confusas ou demoradas.

Gerentes de Projeto e Equipe de Gestão

    Monitoramento de Desempenho e Adoção do Bot:

        1. Precisam de dados sobre a aceitação do bot, número de interações e engajamento dos usuários;

        2. Buscam métricas sobre os estabelecimentos mais consultados e os horários de pico de uso.

    Tomada de Decisão Baseada em Dados:

        1. Precisam de relatórios e dashboards para avaliar a viabilidade do projeto antes de expandi-lo para um aplicativo completo;

        2. Querem identificar possíveis melhorias no bot para aumentar sua utilidade.

    Gestão de Recursos e Tempo de Desenvolvimento:

        1. Precisam equilibrar as demandas do projeto com o orçamento e tempo disponível;

        2. Devem garantir que o desenvolvimento siga uma abordagem iterativa e dentro dos prazos estabelecidos.

Desenvolvedores (Equipe Técnica)

    Ferramentas e Infraestrutura Adequadas:

        1. Precisam de APIs confiáveis e bem documentadas para garantir o bom funcionamento do bot;

        2. Devem contar com um ambiente de desenvolvimento estável e escalável.

    Código Limpo e Manutenível:

        1. O sistema deve ser modular e bem estruturado para facilitar futuras atualizações;

        2. A documentação deve ser clara para permitir a colaboração entre os desenvolvedores.

    Facilidade de Deploy e Monitoramento:

        1. Precisam de um fluxo de deploy simples e eficiente (como Vercel) para agilizar as atualizações;

        2. Desejam ferramentas de logs e monitoramento para identificar possíveis falhas rapidamente.

## 6. Tendências Tecnológicas
O projeto do BOT "Qual a boa?" utilizará tecnologias modernas para garantir escalabilidade, eficiência e facilidade de manutenção. No backend, será utilizado TypeScript junto com NestJS, um framework modular baseado em arquitetura MVC e conceitos de microsserviços. Essa escolha permite suporte a GraphQL, WebSockets e APIs REST, facilitando integrações futuras. No frontend, será utilizado ReactJS com TypeScript para o desenvolvimento do dashboard de métricas, permitindo uma interface responsiva e interativa, além de integração com bibliotecas de visualização de dados como Recharts, D3.js e Chart.js.

Para infraestrutura e deploy, será utilizada a Vercel, uma plataforma de hospedagem serverless otimizada para aplicações React, Next.js e APIs em Node.js. Esse serviço permite deploy contínuo e escalável, sem necessidade de configurações avançadas. O banco de dados ainda será definido, podendo ser MongoDB (NoSQL) para armazenamento de interações do bot ou PostgreSQL (SQL) para dados estruturados de estabelecimentos e usuários. A automação do bot no WhatsApp será feita com a Evolution-API, uma API gratuita que possibilita a criação de bots sem necessidade de um número comercial. Caso o projeto cresça, existe a possibilidade de migração para o WhatsApp Business API.

A gestão do projeto seguirá metodologias ágeis, combinando Scrum e Kanban (Scrumban). As tarefas serão organizadas em sprints curtas, garantindo entregas contínuas e priorização dinâmica, utilizando Trello para o gerenciamento das atividades. O Clockify será utilizado para rastrear o tempo de desenvolvimento, permitindo uma análise mais precisa do esforço investido em cada etapa do projeto. Além disso, será implementada uma estratégia de DevOps e CI/CD utilizando Vercel e GitHub Actions, garantindo automação nos testes e deploys para maior estabilidade.

O bot será desenvolvido para fornecer respostas diretas e objetivas sobre os estabelecimentos próximos e suas promoções. O foco será na eficiência e rapidez nas respostas, garantindo uma experiência simples e intuitiva para os usuários.

A escolha dessas tecnologias visa garantir um desenvolvimento moderno, flexível e escalável, permitindo a implementação rápida da primeira versão do bot e abrindo caminho para futuras melhorias e expansões. Caso novas demandas surjam, a estrutura do projeto já estará preparada para adaptações e crescimento.

## 7. Riscos do Projeto
Riscos Técnicos

    1. Disponibilidade da Evolution-API: Sendo uma ferramenta gratuita, pode haver limitações na estabilidade ou mudanças nos termos de uso, impactando o funcionamento do bot;

    2. Escalabilidade da Arquitetura: Caso o volume de usuários cresça rapidamente, pode ser necessário migrar para soluções pagas e mais robustas, como WhatsApp Business API e servidores dedicados;

    3. Falhas no Deploy e CI/CD: Problemas na Vercel ou conflitos de versão no código podem causar interrupções no funcionamento do bot e do dashboard;

    4. Escolha do Banco de Dados: Se a modelagem inicial não for bem definida, pode impactar o desempenho e exigir migração para outra solução, gerando retrabalho;

    5. Compatibilidade com WhatsApp: O WhatsApp frequentemente atualiza suas políticas e APIs, o que pode exigir ajustes no código para manter o bot funcionando corretamente.

Riscos Operacionais

    1. Aderência do Público: Existe o risco de o bot não ser amplamente adotado pelos usuários, reduzindo sua utilidade para os estabelecimentos;

    2. Interação Limitada do Bot: Como o bot não terá inteligência artificial, ele dependerá de comandos bem estruturados. Isso pode gerar frustração nos usuários caso as respostas não sejam suficientemente abrangentes;

    3. Dependência de Dados dos Estabelecimentos: A qualidade das informações divulgadas (preços e promoções) dependerá da atualização por parte dos estabelecimentos, o que pode comprometer a confiabilidade do serviço;

    4. Manutenção Contínua: Mesmo após o lançamento, será necessário monitoramento e ajustes constantes para manter a qualidade e disponibilidade do bot.

Riscos de Negócios

    1. Monetização do Serviço: O modelo de negócios precisa ser validado. Se os estabelecimentos não enxergarem valor na divulgação pelo bot, pode ser difícil gerar receita com o serviço;

    2. Concorrência com Outras Plataformas: Aplicativos já existentes, como Google Maps, iFood e redes sociais, também fornecem informações sobre bares e eventos, o que pode reduzir o diferencial competitivo do bot;

    3. Restrições Legais e Regulamentações: Dependendo da forma de monetização e coleta de dados, pode ser necessário seguir diretrizes de LGPD (Lei Geral de Proteção de Dados) para garantir a privacidade dos usuários;

    4. Sustentabilidade do Projeto: Se não houver tração suficiente ou um modelo de negócios sustentável, pode ser difícil justificar investimentos futuros para expansão do bot.

## 8. Tomada de Decisões

A tecnologia do backend será TypeScript com NestJS, devido à sua modularidade e segurança no desenvolvimento de APIs. O frontend será feito com ReactJS e TypeScript, garantindo um dashboard dinâmico e escalável. O banco de dados ainda será definido entre MongoDB (para maior flexibilidade) ou PostgreSQL (para estruturação rígida de dados). A Evolution-API foi escolhida para automação no WhatsApp, e o deploy será feito na Vercel devido à facilidade de integração com o ambiente de desenvolvimento.

Os dados serão estruturados para consultas rápidas, armazenando informações de estabelecimentos, usuários e histórico de interações. Para busca por proximidade, será usado um cálculo de distância geográfica. A ordenação das promoções seguirá prioridade de descontos e relevância para o usuário.

O sistema será composto pelo bot do WhatsApp, responsável pela interação com os usuários, uma API backend, que processa as requisições, um banco de dados, que armazena as informações, e um dashboard em React, que permitirá a visualização de métricas.

Para a tomada de decisões, foi feita uma análise comparativa de tecnologias, priorizando escalabilidade e custo-benefício. A estratégia de lançamento inclui testes com um público reduzido para avaliar a aceitação antes da expansão. Além disso, foram considerados riscos técnicos, operacionais e de negócios para minimizar impactos futuros.

## 9. Organização da Arquitetura MVC

## 10. Avaliação das Decisões