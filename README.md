# PROJETO QUAL A BOA

## 1. Definição do Produto
Bot de WhatsApp para analisar o mercado de uma possível solução de problema envolvendo informação e divulgação de produtos comercializados em bares e eventos.

O Bot tem como objetivo identificar o público alvo e analisar a viabilidade para implementação de um possível App que facilita a estrutura de consumação de eventos e estabelecimentos, oferecendo informações sobre os produtos e cardápios, visando frequentadores de eventos, principalmente adolescentes e jovens adultos, que desejam se planejar melhor  no evento, e organizadores de eventos e festas, que farão a utilização do aplicativo para melhorar a experiência de consumo e divulgação em seus eventos. A plataforma com o intuito de melhorar a experiência do consumidor e otimizar a venda do evento.

O objetivo é proporcionar uma experiência mais fluida para os clientes, gerar maior visibilidade para os estabelecimentos e aumentar o faturamento dos mesmos.

## 2. Definição do Produto

## 3. Requisitos do Sistema
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

## 4. Restrições e Condições
Para a criação do BOT no WhatsApp, é utilizada a ferramenta Evolution-API, uma API gratuita que faz a criação de Bots no Whatsapp. A linguagem utilizada para a criação da API responsável por controlar os cálculos e respostas do BOT será TypeScript, utilizando o framework NestJS.
Será também utilizado TypeScript com o framework ReactJS para a criação de um Dashboard de visualização de acessos e métricas. Utilizaremos a metodologia ágil Scrum e Kanban, utilizando o trello para esta gestão, junto ao Clockify para as métricas envolvendo tempo de desenvolvimento e reuniões. A princípio, a ferramenta de deploy utilizada será Vercel.

(falta orçamento)
## 5. Necessidades dos Stakeholders

## 6. Tendências Tecnológicas

## 7. Riscos do Projeto

## 8. Tomada de Decisões

## 9. Organização da Arquitetura MVC

## 10. Avaliação das Decisões