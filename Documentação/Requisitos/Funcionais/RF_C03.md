# Cadastro de Vaga pela Empresa

## Descrição

**COMO** administrador da empresa  
**QUERO** criar vagas de emprego no sistema com dados completos  
**PARA** que os candidatos possam visualizar e se candidatar às vagas disponíveis.

---

## Dados e Validações

### Dados Necessários

1. **Título da Vaga**
   - **Tipo:** String  
   - **Validação:** Não pode ser vazio, deve ter um título claro e descritivo.

2. **Descrição da Vaga**
   - **Tipo:** Texto  
   - **Validação:** Não pode ser vazio, deve descrever claramente as responsabilidades e requisitos da vaga.

3. **Área de Atuação**
   - **Tipo:** String  
   - **Validação:** Não pode ser vazio, deve representar a área de atuação (ex: TI, Marketing, Recursos Humanos).

4. **Requisitos**
   - **Tipo:** Texto  
   - **Validação:** Não pode ser vazio, deve listar as qualificações e habilidades necessárias para a vaga.

5. **Salário**
   - **Tipo:** Decimal  
   - **Validação:** Deve ser um valor positivo e maior que zero.

6. **Localização**
   - **Tipo:** String  
   - **Validação:** Não pode ser vazio, deve descrever o local de trabalho (cidade e estado, por exemplo).

7. **Tipo de Vaga**
   - **Tipo:** Enum (Tempo Integral, Meio Período, Estágio, Freelancer)  
   - **Validação:** Deve ser uma das opções válidas.

8. **Data Limite para Candidatura**
   - **Tipo:** Data  
   - **Validação:** Não pode ser uma data no passado e deve ser maior que a data atual.

---

## Validações Adicionais

- Todos os campos obrigatórios devem ser preenchidos corretamente antes de salvar.  
- O **salário** deve ser um valor numérico positivo.  
- A **data limite para candidatura** não pode ser no passado.  
- O **tipo de vaga** deve ser um dos valores pré-definidos (Tempo Integral, Meio Período, Estágio, Freelancer).  
- A **localização** deve ser preenchida com a cidade e estado, sem abreviações.

---

## Critérios de Aceitação

1. **Cadastro bem-sucedido:**  
   - Quando todos os campos obrigatórios forem preenchidos corretamente, a vaga deve ser cadastrada com sucesso no sistema.

2. **Validação de dados obrigatórios:**  
   - Caso algum campo obrigatório não seja preenchido, o sistema deve exibir a mensagem de erro:  
     **"Todos os campos obrigatórios devem ser preenchidos."**

3. **Validação de salário:**  
   - Caso o valor do salário seja menor ou igual a zero, o sistema deve exibir a mensagem de erro:  
     **"O salário informado deve ser um valor positivo."**

4. **Validação de data limite para candidatura:**  
   - Caso a data limite para candidatura seja no passado, o sistema deve exibir a mensagem de erro:  
     **"A data limite para candidatura não pode ser no passado."**

5. **Confirmação de cadastro:**  
   - Após o cadastro bem-sucedido, o sistema deve exibir a mensagem de confirmação:  
     **"Vaga cadastrada com sucesso."**

6. **Exibição de vagas:**  
   - A vaga recém-cadastrada deve aparecer na listagem de vagas disponíveis para os candidatos no sistema, com todos os dados preenchidos corretamente.

---

## Como Utilizar

1. Acesse o formulário de cadastro de vaga no sistema.
2. Preencha todos os campos obrigatórios com as informações detalhadas da vaga.
3. Clique no botão de salvar para concluir o cadastro.
4. Caso algum erro ocorra, verifique a mensagem de erro exibida e ajuste os dados informados.
5. Após o cadastro bem-sucedido, visualize a vaga na listagem de vagas disponíveis no painel de gestão da empresa.

---