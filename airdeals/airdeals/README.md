# AirDeals 🛫

Plataforma de monitoramento de passagens aéreas com IA.

## Deploy no Vercel (3 passos)

### 1. Suba para o GitHub
Crie um repositório e envie esta pasta inteira.

### 2. Importe no Vercel
- Acesse vercel.com/new
- Importe seu repositório
- Clique em Deploy

### 3. Configure a chave da IA (obrigatório para Aria funcionar)
- No Vercel: Settings → Environment Variables
- Adicione: `ANTHROPIC_API_KEY` = sua chave (obtenha em console.anthropic.com)
- Clique em Redeploy

## Estrutura
```
airdeals/
├── api/
│   └── chat.js        # Proxy serverless para a API da Anthropic
├── public/
│   └── index.html     # Aplicação completa
├── vercel.json        # Configuração de rotas
└── README.md
```

## Tecnologias
- React 18 (via CDN, sem build)
- Tailwind CSS (via CDN)
- Vercel Edge Functions (proxy da IA)
- Claude Haiku (Anthropic AI)
