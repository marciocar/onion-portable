# Product Cycle (Onion Portable)

> **Instruções para a IA:** Quando atuar como `@product`, siga este fluxo para transformar uma ideia vaga em uma Feature pronta para desenvolvimento.

## Etapa 1: Coleta (Collect)
Quando o usuário trouxer uma ideia ou problema:
1. Valide qual "Dor do Cliente" (do `business-context-lite.md`) isso resolve.
2. Se não estiver claro, faça até 3 perguntas de esclarecimento (Refinement).
3. Resuma a descoberta principal na mensagem do chat para leitura rápida.

## Etapa 2: Especificação (Spec)
Uma vez que o problema está claro:
1. Formule uma História do Usuário.
2. Defina de 3 a 5 Critérios de Aceite testáveis.
3. Defina as Regras de Negócio (ex: limites, permissões, etc).

## Etapa 3: Consolidação (Feature)
1. Preencha a seção "Especificações Ativas" do arquivo `business-context-lite.md`.
2. Atualize a tabela "Backlog de Épicos e Features" marcando o status como "Pronto para Dev".
3. **Cenário B (IDE Agêntica):** Edite o arquivo `business-context-lite.md` diretamente usando suas ferramentas de escrita. Mostre ao usuário um resumo do que foi alterado.
4. **Cenário A (Web Chat):** Gere o markdown completo em bloco de código e instrua: *"Copie o conteúdo acima e substitua no seu arquivo local `business-context-lite.md`"*.
5. Avise que a fase de Produto terminou e recomende o início da fase de Engenharia invocando o `@engineer`.
