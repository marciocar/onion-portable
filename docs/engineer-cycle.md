# Engineer Cycle (Onion Portable)

> **Instruções para a IA:** Quando atuar como `@engineer`, siga este fluxo para transformar uma Feature documentada em código funcional de alta qualidade.

## Etapa 1: Início (Start)
1. Leia o `business-context-lite.md` para entender a feature marcada como "Pronto para Dev".
2. Leia o `technical-context-lite.md` para entender a stack e arquitetura atuais.
3. Analise se a solução técnica proposta requer novas dependências, impacto em segurança ou banco de dados.

## Etapa 2: Planejamento (Plan)
1. **Nunca gere código final nesta etapa.**
2. Escreva uma seção "Plano para [Nome da Feature]" para ser adicionada no `technical-context-lite.md`.
3. O plano deve conter a lista de arquivos a serem criados/modificados e um checklist passo a passo lógico.
4. **Cenário B (IDE Agêntica):** Edite o `technical-context-lite.md` diretamente e pergunte: *"Você aprova este plano técnico?"*.
5. **Cenário A (Web Chat):** Entregue o markdown em bloco de código e pergunte: *"Você aprova este plano técnico?"*.

## Etapa 3: Execução (Work)
Uma vez aprovado:
1. **Cenário B (IDE Agêntica):** Gere e grave o código diretamente nos arquivos do projeto usando suas ferramentas de escrita.
2. **Cenário A (Web Chat):** Gere o código arquivo por arquivo em blocos de código, instruindo o usuário a criar/colar cada arquivo.
3. Se for uma mudança longa, divida em partes. Após cada bloco de código, atualize o usuário sobre qual item do checklist (do plano técnico) acabou de ser concluído.
4. Se você identificar um erro não previsto, pare a codificação e sugira uma mudança no plano técnico antes de prosseguir.

## Etapa 4: Conclusão (Finish)
1. Forneça instruções ao usuário sobre como testar as alterações recém-criadas.
2. **Cenário B:** Atualize diretamente o status da Feature no `business-context-lite.md` para "Feito".
3. **Cenário A:** Instrua o usuário a marcar a Feature como "Feito" no arquivo local.
