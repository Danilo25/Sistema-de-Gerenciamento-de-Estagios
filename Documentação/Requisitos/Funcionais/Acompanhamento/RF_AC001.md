# Acompanhamento do Processo Seletivo

## Descrição

**COMO** estudante ou empresa  
**QUERO** acompanhar o status do processo seletivo das candidaturas  
**PARA** que eu tenha visibilidade das etapas e atualizações relacionadas ao processo de seleção.

---

## Prioridade  
### Alta  
Acompanhamento do processo seletivo é essencial para a transparência e experiência do usuário.  

---
## Dados e Validações

### Dados Necessários

1. **ID da Candidatura**  
   - **Tipo:** Inteiro  
   - **Validação:** Deve ser único e existir no sistema.  

2. **Status da Candidatura**  
   - **Tipo:** Enum (Ex.: "Inscrição Realizada", "Em Análise", "Entrevista Agendada", "Aprovado", "Reprovado")  
   - **Validação:** Deve corresponder a um dos status válidos definidos no sistema.  

3. **Data da Última Atualização**  
   - **Tipo:** Data e Hora  
   - **Validação:** Deve ser uma data válida e sempre posterior ou igual à data da criação da candidatura.  

4. **Descrição da Atualização (Opcional)**  
   - **Tipo:** String  
   - **Validação:** Pode ser preenchida para detalhar informações adicionais sobre o status.  

---

## Validações Adicionais

- O **status da candidatura** deve ser atualizado por um responsável autorizado (empresa ou estudante, dependendo da etapa).  
- O sistema deve garantir que nenhuma etapa seja pulada, respeitando a sequência lógica do processo seletivo.  
- A data da última atualização deve ser registrada automaticamente sempre que houver uma mudança no status.  

---

## Critérios de Aceitação

1. **Acompanhamento em tempo real:**  
   - O estudante e a empresa devem ser capazes de visualizar o status atual da candidatura na tela do sistema.  

2. **Atualização de status:**  
   - Empresas podem alterar o status da candidatura para refletir o progresso do processo seletivo.  
   - Estudantes podem visualizar as atualizações em tempo real.  

3. **Notificação de alteração:**  
   - Sempre que o status da candidatura for alterado, o estudante e a empresa devem ser notificados por meio do sistema (ex.: notificações internas, e-mail ou outro método definido).  

4. **Validação de sequência de etapas:**  
   - Caso uma empresa tente atualizar o status para uma etapa fora da sequência esperada, o sistema deve exibir a mensagem de erro:  
     **"A etapa selecionada não é válida para o progresso atual da candidatura."**  

5. **Histórico de atualizações:**  
   - O sistema deve manter um registro de todas as mudanças no status da candidatura, com as respectivas datas e descrições.  

6. **Confirmação de atualização:**  
   - Após cada atualização de status, o sistema deve exibir a mensagem de confirmação:  
     **"O status da candidatura foi atualizado com sucesso."**  

---

## Como Utilizar

1. O estudante ou a empresa acessa a página da candidatura no sistema.  
2. O estudante visualiza o status atual e o histórico de atualizações.  
3. A empresa pode alterar o status da candidatura para refletir o progresso do processo seletivo, preenchendo as informações necessárias.  
4. Após cada atualização, notificações são enviadas aos envolvidos (empresa e estudante).  
5. O estudante acompanha as mudanças de status até a conclusão do processo seletivo.  

---
