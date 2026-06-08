# Sync & Reverse Engineering Cycle (Onion Portable)

> **Instruções para a IA:** Quando atuar como `@docs` ou quando o usuário solicitar para "fazer engenharia reversa", "sincronizar o projeto" ou "documentar código legado", siga este fluxo.

## Etapa 1: Ingestão de Código (Reverse Engineering)

### Cenário B (IDE Agêntica) — Preferencial
1. Use suas ferramentas (`list_dir`, `view_file`, `grep_search`) para varrer a estrutura do projeto.
2. Leia os arquivos de configuração (`package.json`, `requirements.txt`, `Cargo.toml`, `*.config.*`, etc.) para identificar a stack.
3. Percorra os diretórios de código-fonte para mapear a arquitetura, entidades e fluxos lógicos.

### Cenário A (Web Chat) — Fallback
1. Instrua o usuário: *"Por favor, cole aqui o conteúdo dos seus principais arquivos de código, ou faça o upload de um .zip/arquivos soltos caso a plataforma suporte."*
2. Analise os arquivos fornecidos.

### Em ambos os cenários, foque em identificar:
- Qual é a stack tecnológica?
- Quais são as principais entidades e fluxos lógicos (arquitetura)?
- Quais problemas de negócio esse código parece resolver?

## Etapa 2: Sincronização do Contexto Técnico (Tech Sync)
1. Com base na análise do código, gere uma nova versão do `technical-context-lite.md`.
2. Preencha detalhadamente as seções "Stack Tecnológica" e "Arquitetura Lógica".
3. **Cenário B:** Edite o arquivo `technical-context-lite.md` diretamente e mostre um resumo das mudanças ao usuário.
4. **Cenário A:** Entregue o markdown ao usuário e peça para ele salvar no seu arquivo local.

## Etapa 3: Inferência do Contexto de Negócio (Business Sync)
1. Tente inferir as features que o código implementa.
2. Gere uma nova versão do `business-context-lite.md` preenchendo a tabela "Backlog de Épicos e Features" com as funcionalidades já implementadas (Status: "Feito").
3. **Cenário B:** Edite o arquivo `business-context-lite.md` diretamente e mostre um resumo das mudanças ao usuário.
4. **Cenário A:** Entregue o markdown ao usuário e peça para ele salvar no seu arquivo local.

## Etapa 4: Validação
1. Após entregar os documentos sincronizados, pergunte ao usuário: *"Estes documentos refletem bem o estado atual do projeto? Há algo que eu deva corrigir?"*
