# ZippFrete_API

# ZippFrete API

🚚 **Cotação de Fretes Inteligente com Múltiplas Transportadoras**  
A **ZippFrete API** oferece cotações de frete em tempo real, integrando os principais serviços logísticos do mercado (Correios, Jadlog, FedEx e mais), com foco em performance, escalabilidade e monetização B2B. 

---

## 📌 Funcionalidades
- 🔐 Autenticação via JWT
- 📦 Cotação de frete multitransportadoras com base em CEP e dimensões
- 📊 Rate limiting por usuário (100 cotações/dia)
- 💾 Estrutura escalável com PostgreSQL (usuários, histórico de cotações)
- 🧩 Integração com APIs reais (Correios, Jadlog...)
- 📈 Monitoramento de uso para cobrança (freemium + planos pagos)

---

## 📂 Estrutura de Pastas (MVP)
```
ZippFrete_API/
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   ├── middleware/
│   ├── config/
│   └── index.js
├── .env
├── package.json
└── README.md
```

---

## 🚀 Como Rodar Localmente

### Pré-requisitos:
- Node.js 16+
- PostgreSQL
- Git

### Passos:
```bash
# Clone o repositório
$ git clone https://github.com/seu-usuario/ZippFrete_API.git

# Instale as dependências
$ cd ZippFrete_API
$ npm install

# Crie o arquivo .env
$ cp .env.example .env

# Inicie o servidor
$ npm start

# Acesse: http://localhost:3000/api/v1/
```

---

## 🛠️ Tecnologias Utilizadas
- **Backend**: Node.js + Express
- **Autenticação**: JWT
- **Banco de Dados**: PostgreSQL + Prisma ORM
- **Integrações**: Correios (SOAP), Jadlog (REST), FedEx (REST)
- **Deploy**: Render / Railway / Docker Ready
- **Documentação**: Swagger (OpenAPI)

---

## 📖 Documentação da API (em breve)
- `/api/v1/auth/login` – Autenticação e geração de token
- `/api/v1/cotacao/` – Enviar dados e obter múltiplas cotações
- Headers: `Authorization: Bearer {token}`
- Limite: 100 requisições/dia (plano gratuito)

---

## 💼 Roadmap Inicial
- [x] Estrutura básica Express + JWT
- [x] Middleware de rate limiting
- [ ] Integração Correios + Jadlog
- [ ] Interface Web para uso e cadastro
- [ ] Integração Stripe/Pix para monetização
- [ ] Deploy e monitoramento

---

## 📢 Suporte e Contato
Curtiu o projeto? Tem ideias ou precisa de suporte?  
📬 contato@zippfrete.com.br  
🔗 www.zippfrete.com.br  

---

## 🧩 Próximos Passos
- Criar identidade visual (logo e paleta)
- Desenvolver a interface inicial (painel de cotações e login)
- Escalar API com autenticação e monitoramento de requisições

---

> "A escolha inteligente para quem precisa de frete rápido, acessível e sob controle."  
**ZippFrete API — Seu frete, sua escolha, sua vantagem.**
