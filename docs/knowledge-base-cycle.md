# Knowledge Base Cycle (Onion Portable)

> **Instruções para a IA:** Quando atuar como `@meta` ou quando o usuário solicitar a criação/estudo de um novo conceito, siga este fluxo para estruturar uma Knowledge Base (KB).

## Etapa 1: Pesquisa e Extração
Quando o usuário pedir para criar uma Knowledge Base sobre um tema (ex: "Crie uma KB sobre a API do Stripe"):
1. Pergunte se o usuário tem links, documentações ou se você deve usar seu conhecimento interno.
2. Identifique os conceitos centrais, limitações e melhores práticas associadas ao tema.

## Etapa 2: Estruturação
1. **Nunca gere um texto solto.** Toda KB deve seguir a estrutura:
   - **Visão Geral:** O que é e para que serve.
   - **Conceitos Chave:** Lista de conceitos fundamentais.
   - **Exemplos Práticos:** Trechos de código ou fluxos de uso.
   - **Armadilhas (Gotchas):** O que evitar.

## Etapa 3: Consolidação (KB Gerada)
1. Crie o documento completo da Knowledge Base.
2. **Cenário B (IDE Agêntica):** Salve o arquivo diretamente em `docs/knowledge-base/[nome-do-tema].md` usando suas ferramentas de escrita. Informe ao usuário o caminho do arquivo criado.
3. **Cenário A (Web Chat):** Gere o bloco markdown completo e instrua: *"Copie o bloco acima e salve em um novo arquivo dentro da sua pasta `docs/knowledge-base/[nome-do-tema].md`"*.
4. Avise o usuário que, nas próximas conversas, se ele fizer o upload deste arquivo (Cenário A) ou a IA ler do projeto (Cenário B), o padrão será implementado corretamente.
