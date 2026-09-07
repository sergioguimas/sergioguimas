# Sérgio Guimarães

Construo sistemas web, SaaS multi-tenant e automação de processos.
Entendo o processo antes de escolher a stack.

[sgdev.cloud](https://sgdev.cloud) · [LinkedIn](https://linkedin.com/in/sergio-guimar%C3%A3es-ads)

O portfólio expõe os mesmos dados que alimentam os cases por API pública — [`/api/projects`](https://sgdev.cloud/api/projects) e [`/api/stacks`](https://sgdev.cloud/api/stacks).

## Produtos

### [Eliza](https://github.com/sergioguimas/eliza)

`em produção · acesso restrito` — Next.js · TypeScript · Supabase · PostgreSQL

Agenda, prontuário, financeiro e permissões de equipe para clínicas e profissionais que ainda controlam atendimento em papel ou planilha.

Multi-tenant com isolamento por RLS no Postgres, quatro papéis por organização e confirmação de consulta automatizada por WhatsApp. Publicado sob licença MIT por escolha: dá para ler a implementação inteira antes de confiar nela.

### [Pandora](https://github.com/sergioguimas/pandora)

`em desenvolvimento` — Next.js · TypeScript · Supabase/pgvector · Gemini e OpenAI

Hub onde cada agente de IA tem base de conhecimento própria, memória de conversa e resposta em streaming — para quem precisa de assistentes especializados, não de mais um chat genérico.

A rodada de conversa é um gerador assíncrono com dependências injetáveis; a rota SSE é só o adaptador de transporte. A suíte principal roda em segundos, sem banco, sem HTTP e sem chamar o modelo; uma segunda suíte valida as políticas de isolamento contra um Postgres real. Código aberto para leitura.

### [Geti Fidelidade](https://github.com/sergioguimas/geti-fidelidade)

`em produção · acesso restrito` — Next.js · TypeScript · Supabase · PostgreSQL

Programa de pontos para lojistas: acúmulo por compra, resgate, expiração e indicadores comerciais, com vários programas na mesma base.

O motor consome pontos em FIFO e expira por lote. Saldo errado aqui não é bug de tela, é quebra de confiança com o cliente final — então ordenação e bordas de expiração são o núcleo do problema, não CRUD em volta de uma tabela.

### [Axios Calc](https://github.com/sergioguimas/axios-calc)

`uso interno` — Next.js · TypeScript · Prisma · SQLite · Docker

Custo real de impressão 3D em resina e filamento: material, energia, acabamento e frete abertos por item, com histórico de orçamentos para comparar decisão de preço ao longo do tempo.

Cada conta enxerga apenas as próprias resinas, impressoras e presets. Sai do Supabase de propósito — Prisma sobre SQLite, empacotado em Docker, porque este precisa rodar isolado.

## O que já está rodando

Trabalho que raramente vira repositório público:

- **Automação fiscal para escritório contábil** — Playwright preenchendo declaração de ITF em portal do governo a partir de planilhas, com conferência antes do envio e execução multi-empresa.
- **Exportação mensal de XML de notas** — login, coleta multi-empresa e recuperação dos arquivos por e-mail, em lote agendado.
- **Portal de documentos contábeis** — acesso de escritórios às pastas de Drive das empresas clientes, com níveis de contador e administrador. Flask e Google Drive API.
- **[Vitrine de catálogo para comércio local](https://o-cravo-e-a-rosa.vercel.app)** — mobile-first, com contato direto por WhatsApp e Instagram.

## Stack

**Frontend** — Next.js · React · TypeScript · Tailwind
**Backend e dados** — Supabase · PostgreSQL · Prisma · Node.js
**Automação** — Playwright · Python · n8n · PowerShell
**Infraestrutura** — Docker · VPS Linux · Traefik/Nginx · GitHub Actions
**IA** — Gemini · pgvector e RAG · orquestração de agentes

A stack muda quando o contexto pede. A clareza do problema vem primeiro.

## Colaborações

**[SolaBridge](https://github.com/joaoartur-mk0/SolaBridge)** — sistema contábil com escrituração de partidas dobradas, integração Open Finance e emissão de NFS-e. Frontend em React e TypeScript comigo; backend Laravel com [@joaoartur-mk0](https://github.com/joaoartur-mk0).

---

Análise e Desenvolvimento de Sistemas — IFNMG, em andamento.

Aberto a projeto e parceria: [sgdev.cloud](https://sgdev.cloud) · [LinkedIn](https://linkedin.com/in/sergio-guimar%C3%A3es-ads)
