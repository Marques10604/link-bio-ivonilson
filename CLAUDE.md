# CLAUDE.md — Link Bio Ivonilson

## Início de sessão obrigatório
Isso é uma página HTML estática única (`index.html`, sem build step — abrir direto ou usar `local-server.js`). Antes de mexer em copy ou cor, leia `../../Marca e Conhecimento/brand.md` e `../../Marca e Conhecimento/voz-e-metodologia.md` — a paleta e o tom já foram corrigidos em 14/07/2026 pra bater com esses arquivos, não reintroduza laranja neon, glow, gradiente ou caixa alta.

## Pendências conhecidas (não perguntar de novo, checar o código)
- Link de agendamento (Google Calendar) e webhook do n8n já estão configurados no passo 6 do formulário e na função `submitForm` (14/07/2026). O webhook já é a URL de produção (`/webhook/`, ativado em 15/07/2026). O mesmo par também está preenchido em `../../Operações Inteligentes - Landing Page/components/diagnosis-form.tsx` — se o usuário mandar um valor novo, atualizar os dois arquivos juntos.
- Analytics (Google Tag) e Meta Pixel estão comentados no `<head>` até existirem IDs reais — não reative com IDs falsos.

## Regras de economia de tokens
- O arquivo tem ~650 linhas num só HTML — pra edições pontuais, leia só o trecho relevante (CSS de um seletor, ou a seção do formulário) em vez do arquivo inteiro
- Não há testes nem typecheck aqui — validar visualmente é a única forma de QA
