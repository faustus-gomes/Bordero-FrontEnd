<h1>Front End - planium</h1>

📋 Frontend - Sistema Planium

📖 Descrição

Frontend desenvolvido para integração com a API Planium, proporcionando uma interface web moderna e responsiva para visualização e gestão de dados do sistema.

🚀 Funcionalidades

🔐 Página de Login - Autenticação de usuários
📊 Dashboard com Grid - Visualização de dados em tabela responsiva
🔄 Controle de Estado - Botão inteligente que se adapta aos dados disponíveis
🎨 Design Responsivo - Interface compatível com diferentes dispositivos
⚡ Feedback Visual - Loading states e mensagens de erro/status
🛠 Tecnologias Utilizadas

HTML5 - Estrutura semântica
CSS3 - Estilização e design responsivo
Bootstrap 5.3.0 - Framework CSS para componentes UI
JavaScript (ES6+) - Interatividade e consumo de API
Fetch API - Comunicação com backend REST
📁 Estrutura de Arquivos
<pre>
frontend/
├── login.html              # Página de autenticação
├── dados_grid.html         # Dashboard com grid de dados
├── image/
│   └── header.png          # Logo da aplicação
└── README.md              # Documentação
</pre>

🔌 Integração com Backend

Endpoints Consumidos
<pre>
Método	Endpoint	Descrição
GET	/api/procedures/dados_grid	Busca dados para o grid
GET	/api/procedures/health	Health check da API
GET	/api/procedures/list	Lista de procedimentos
</pre>

Configuração CORS
<pre>
@CrossOrigin(origins = "http://localhost")
</pre>

🎯 Funcionalidades Específicas

Página de Login (login.html)

Formulário de autenticação com validação
Design limpo e profissional
Campos para email e senha
Opção "Lembrar-me"
Dashboard de Dados (dados_grid.html)

Grid Dinâmico: Renderiza dados da API automaticamente
Botão Inteligente: Habilita/desabilita baseado na disponibilidade de dados
Loading States: Feedback durante carregamento
Tratamento de Erros: Mensagens específicas para diferentes cenários
Design Responsivo: Adapta-se a diferentes tamanhos de tela
O backend deve estar configurado para aceitar requisições do frontend:
2. Recarregue o Apache
docker exec NOME_DO_CONTAINER service apache2 reload

