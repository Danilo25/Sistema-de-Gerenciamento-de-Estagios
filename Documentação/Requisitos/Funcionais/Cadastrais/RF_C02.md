# Cadastro de Informações da Empresa

## Descrição

**COMO** administrador da empresa  
**QUERO** registrar as informações da empresa no sistema  
**PARA** que o sistema consiga gerenciar as informações da empresa de forma organizada e eficiente.

---

## Prioridade

### Alta
O cadastro de empresas é necessário para disponibilizar vagas e conectar candidatos e empresas.

---

## Dados e Validações

### Dados Necessários

1. **Nome da Empresa**
   - **Tipo:** String  
   - **Validação:** Não pode ser vazio, deve ser único e conter apenas letras e espaços.

2. **CNPJ**
   - **Tipo:** String  
   - **Validação:** Deve ser um CNPJ válido e único no sistema.

3. **Endereço**
   - **Tipo:** String  
   - **Validação:** Não pode ser vazio, deve incluir rua, número e cidade.

4. **Número de Funcionários**
   - **Tipo:** Inteiro  
   - **Validação:** Deve ser um número inteiro positivo (mínimo de 1).

5. **E-mail de Contato**
   - **Tipo:** String  
   - **Validação:** Deve ser um endereço de e-mail válido e único no sistema.

6. **Telefone de Contato**
   - **Tipo:** String  
   - **Validação:** Deve ser um número de telefone válido, aceitando DDD e 9 dígitos (ex.: (XX) 9XXXX-XXXX).

---

## Validações Adicionais

- Todos os campos obrigatórios devem ser preenchidos corretamente antes de salvar.  
- Não é permitido cadastrar empresas com o mesmo CNPJ ou e-mail.  
- O CNPJ deve seguir o formato e a validação padrão brasileiro (14 dígitos com cálculo do dígito verificador).  
- O e-mail deve seguir o formato padrão (ex.: usuario@dominio.com).  
- O número de funcionários deve ser maior que zero.

---

## Critérios de Aceitação

1. **Cadastro bem-sucedido:**  
   - Quando todos os campos obrigatórios forem preenchidos corretamente, o sistema deve cadastrar as informações da empresa.  

2. **Validação de CNPJ único:**  
   - Caso o CNPJ já esteja cadastrado no sistema, deve ser exibida a mensagem de erro:  
     **"O CNPJ informado já está cadastrado no sistema."**

3. **Validação de e-mail único:**  
   - Caso o e-mail já esteja em uso, deve ser exibida a mensagem de erro:  
     **"O e-mail informado já está cadastrado no sistema."**

4. **Verificação de formato de CNPJ:**  
   - Caso o CNPJ não siga o formato válido, deve ser exibida a mensagem de erro:  
     **"O CNPJ informado é inválido. Por favor, insira um CNPJ válido."**

5. **Confirmação de cadastro:**  
   - Após o cadastro, o sistema deve exibir a mensagem de confirmação:  
     **"Informações da empresa cadastradas com sucesso."**

6. **Listagem de informações:**  
   - A empresa recém-cadastrada deve ser listada no painel de empresas disponíveis no sistema, com os dados corretamente preenchidos.

---

## Como Utilizar

1. Acesse o formulário de cadastro de informações da empresa no sistema.
2. Preencha os campos obrigatórios com os dados corretos.
3. Clique no botão de salvar para concluir o cadastro.
4. Caso ocorra algum erro, verifique a mensagem exibida e ajuste os dados informados.
5. Após o cadastro bem-sucedido, visualize as informações da empresa no painel de dados.

---