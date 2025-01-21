# Autenticação de Usuário

## Descrição

**COMO** usuário do sistema  
**QUERO** realizar a autenticação com login e senha ou por meio de uma rede social  
**PARA** que eu possa acessar funcionalidades personalizadas e seguras.

---

## Dados e Validações

### Dados Necessários

1. **E-mail**  
   - **Tipo:** String  
   - **Validação:** Deve ser um endereço de e-mail válido e previamente cadastrado no sistema.  

2. **Senha**  
   - **Tipo:** String  
   - **Validação:** Deve ter no mínimo 8 caracteres, contendo pelo menos uma letra maiúscula, uma letra minúscula, um número e um caractere especial.  

3. **Rede Social**  
   - **Tipo:** Enum (Ex.: "Google", "Facebook", "LinkedIn")  
   - **Validação:** A conta da rede social deve estar vinculada a um perfil válido no sistema.  

4. **Token de Autenticação (para login com rede social)**  
   - **Tipo:** String  
   - **Validação:** Deve ser válido e emitido pela rede social escolhida.  

---

## Validações Adicionais

- O e-mail e a senha fornecidos pelo usuário devem corresponder a um cadastro existente no sistema.  
- Para login por redes sociais, o token recebido deve ser validado com o provedor da rede social antes de conceder acesso ao usuário.  
- Após uma autenticação bem-sucedida, o sistema deve gerar um **token de sessão** exclusivo e seguro para o usuário.  
- Em caso de 5 tentativas consecutivas de login com falha, o sistema deve bloquear temporariamente a conta por um período de 15 minutos.  

---

## Critérios de Aceitação

1. **Login com e-mail e senha:**  
   - O sistema deve autenticar o usuário quando as credenciais fornecidas forem válidas.  
   - Caso as credenciais sejam inválidas, o sistema deve exibir a mensagem de erro:  
     **"E-mail ou senha incorretos. Por favor, tente novamente."**  

2. **Login com rede social:**  
   - O sistema deve permitir que o usuário faça login utilizando redes sociais (ex.: Google, Facebook ou LinkedIn), validando o token recebido com o provedor.  
   - Caso a autenticação com a rede social falhe, o sistema deve exibir a mensagem de erro:  
     **"Não foi possível autenticar com a rede social. Por favor, tente novamente."**  

3. **Esqueci minha senha:**  
   - O sistema deve oferecer a funcionalidade de recuperação de senha, enviando um e-mail com um link para redefinição.  

4. **Token de sessão:**  
   - Após o login bem-sucedido, o sistema deve gerar um token de sessão para identificar e autorizar o usuário nas funcionalidades personalizadas.  

5. **Bloqueio de conta temporário:**  
   - Após 5 tentativas consecutivas de login com falha, o sistema deve bloquear temporariamente a conta e exibir a mensagem de erro:  
     **"Muitas tentativas de login. A conta foi bloqueada temporariamente por 15 minutos."**  

6. **Logout seguro:**  
   - O sistema deve oferecer a funcionalidade de logout, invalidando o token de sessão e encerrando a conexão do usuário.  

---

## Como Utilizar

1. Na página de login, o usuário escolhe entre:  
   - Inserir e-mail e senha cadastrados.  
   - Selecionar uma rede social para autenticação.  

2. O sistema valida as credenciais fornecidas ou o token da rede social.  
3. Após a autenticação bem-sucedida, o sistema redireciona o usuário para o painel principal com funcionalidades personalizadas.  
4. Em caso de erro de autenticação, o sistema exibe a mensagem correspondente e permite que o usuário tente novamente.  
5. O usuário pode fazer logout a qualquer momento para encerrar sua sessão de forma segura.  

---
