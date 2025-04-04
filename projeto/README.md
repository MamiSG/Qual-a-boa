# Bot de Recomendações de Estabelecimentos

Um sistema de recomendação de bares e restaurantes baseado em arquitetura de camadas, que interage com usuários via WhatsApp através do Evolution Bot. O projeto é estruturado em APIs independentes que se comunicam entre si para oferecer recomendações personalizadas com base em preferências e localização do usuário.

## Arquitetura em Camadas

O sistema segue uma arquitetura de três camadas bem definidas:

### 1. Camada de Interface (Interface Layer)
**Componente**: Evolution Bot
- Gerencia a integração com a API do WhatsApp
- Recebe e encaminha mensagens entre o usuário e a aplicação
- Transforma a comunicação do usuário em webhooks para a camada de orquestração

### 2. Camada de Orquestração (Orchestration Layer)
**Componente**: `bot_api` (em desenvolvimento)
- Processa as interações do usuário recebidas via webhooks
- Gerencia o estado e fluxo das conversas com cada usuário
- Coordena requisições para a camada de dados conforme necessidade
- Formata as respostas antes de enviá-las de volta ao usuário

### 3. Camada de Dados (Data Layer)
**Componente**: `restaurantes_api`
- Gerencia o acesso aos dados dos estabelecimentos
- Implementa a lógica de filtragem e pesquisa de recomendações
- Fornece endpoints RESTful para consulta de estabelecimentos

## Estrutura do Projeto

```
projeto/
├── restaurantes_api/       # Camada de Dados
│   ├── controllers/        # Controladores de acesso aos dados
│   ├── models/             # Modelos de dados e lógica de negócio
│   ├── app.py              # Aplicação Flask e definição de endpoints
│   └── config.py           # Configurações da API e banco de dados
│
└── bot_api/                # Camada de Orquestração (planejada)
    ├── app.py              # Aplicação Flask e endpoints de webhook
    ├── conversation_manager.py  # Gerenciamento de estado das conversas
    ├── establishment_api_client.py  # Cliente para restaurantes_api
    ├── logger.py           # Sistema de logging para monitoramento
    └── config.py           # Configurações da API de bot
```

## Fluxo de Interação Entre Camadas

1. **Entrada de Dados**:
   - Usuário envia mensagem ou compartilha localização via WhatsApp
   - Evolution Bot (Camada de Interface) recebe e encaminha para a `bot_api`

2. **Processamento**:
   - `bot_api` (Camada de Orquestração) interpreta a mensagem e extrai intenções
   - Baseado no contexto da conversa, determina quais informações solicitar à Camada de Dados

3. **Consulta de Dados**:
   - `bot_api` formata e envia requisição para endpoints específicos da `restaurantes_api`
   - `restaurantes_api` (Camada de Dados) processa a solicitação, filtra estabelecimentos e retorna resultados

4. **Resposta ao Usuário**:
   - `bot_api` formata os resultados em mensagem amigável
   - Evolution Bot entrega a resposta ao usuário via WhatsApp

## Configuração e Execução

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/seu_usuario/bot-recomendacoes.git
   cd bot-recomendacoes
   ```

2. **Configure a camada de dados**:
   ```bash
   cd restaurantes_api
   pip install -r requirements.txt
   # Configure seu banco de dados em config.py
   python app.py
   ```

3. **Configure a camada de orquestração** (quando implementada):
   ```bash
   cd ../bot_api
   pip install -r requirements.txt
   # Configure as URLs da restaurantes_api em config.py
   python app.py
   ```

4. **Integração com Evolution Bot**:
   - Configure um webhook no Evolution Bot apontando para `http://seu-servidor/webhook`
   - Verifique a documentação do Evolution Bot para detalhes de autenticação

## Próximos Passos

- Implementar a Camada de Orquestração (`bot_api`) seguindo a estrutura planejada
- Desenvolver fluxos de conversa inteligentes para capturar preferências dos usuários
- Implementar sistema de cache para otimizar consultas frequentes
- Adicionar telemetria e monitoramento entre as camadas

## Requisitos Técnicos

- Python 3.8+
- Flask 2.0+
- MongoDB (para armazenamento de estabelecimentos)
- Acesso à plataforma Evolution Bot