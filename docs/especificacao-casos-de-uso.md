# Especificação dos Casos de Uso — Urbanly

## UC01 — Criar conta

**Ator principal:** Visitante  

**Descrição:**  
Permite que um usuário visitante crie uma nova conta na plataforma para acessar funcionalidades restritas.

**Pré-condições**
- O usuário não possui conta cadastrada.

**Fluxo principal**
1. O visitante acessa a tela de cadastro.
2. O sistema solicita dados do usuário (nome, email, senha).
3. O visitante preenche os dados solicitados.
4. O sistema valida as informações.
5. O sistema cria a conta.
6. O sistema confirma o cadastro.

**Fluxos alternativos**

**4A – Email já cadastrado**
1. O sistema identifica que o email já está registrado.
2. O sistema informa o erro ao usuário.

**Pós-condições**
- A conta do usuário é criada no sistema.

---

# UC02 — Autenticar

**Ator principal:** Usuário

**Descrição:**  
Permite que um usuário realize login na plataforma.

**Pré-condições**
- O usuário possui uma conta cadastrada.

**Fluxo principal**

1. O usuário acessa a tela de login.
2. O usuário informa email e senha.
3. O sistema valida as credenciais.
4. O sistema autentica o usuário.
5. O usuário acessa as funcionalidades do sistema.

**Fluxos alternativos**

**3A – Credenciais inválidas**

1. O sistema detecta erro nas credenciais.
2. O sistema informa o erro ao usuário.

**Pós-condições**
- O usuário está autenticado no sistema.

---

# UC03 — Buscar estabelecimentos por palavra-chave

**Ator principal:** Visitante / Usuário

**Descrição:**  
Permite buscar estabelecimentos usando uma palavra-chave.

**Pré-condições**
- O sistema está disponível.

**Fluxo principal**

1. O usuário acessa a busca.
2. O usuário digita uma palavra-chave.
3. O sistema processa a busca.
4. O sistema retorna os estabelecimentos correspondentes.

**Pós-condições**
- O sistema exibe resultados da busca.

---

# UC04 — Buscar estabelecimentos por palavra-chave, localização e interesses

**Ator principal:** Usuário

**Descrição:**  
Permite realizar uma busca avançada com filtros.

**Pré-condições**
- O usuário está autenticado.

**Fluxo principal**

1. O usuário acessa a busca avançada.
2. O usuário informa:
   - palavra-chave
   - localização
   - interesses
3. O sistema processa os filtros.
4. O sistema retorna os resultados filtrados.

**Pós-condições**
- Resultados personalizados são exibidos.

---

# UC05 — Visualizar detalhes de estabelecimento

**Ator principal:** Visitante / Usuário

**Descrição:**  
Permite visualizar informações completas sobre um estabelecimento.

**Pré-condições**
- O estabelecimento existe no sistema.

**Fluxo principal**

1. O usuário seleciona um estabelecimento.
2. O sistema recupera as informações do estabelecimento.
3. O sistema exibe:
   - descrição
   - localização
   - avaliações
   - fotos
   - categoria

**Pós-condições**
- Informações detalhadas são exibidas.

---

# UC06 — Avaliar estabelecimento com comentário

**Ator principal:** Usuário

**Descrição:**  
Permite que usuários avaliem estabelecimentos e escrevam comentários.

**Pré-condições**
- O usuário está autenticado.
- O estabelecimento existe.

**Fluxo principal**

1. O usuário acessa a página do estabelecimento.
2. O usuário seleciona a opção de avaliação.
3. O usuário atribui uma nota.
4. O usuário escreve um comentário.
5. O sistema salva a avaliação.

**Pós-condições**
- A avaliação é registrada no sistema.

---

# UC07 — Favoritar estabelecimento

**Ator principal:** Usuário

**Descrição:**  
Permite salvar estabelecimentos na lista de favoritos.

**Pré-condições**
- Usuário autenticado.

**Fluxo principal**

1. O usuário visualiza um estabelecimento.
2. O usuário seleciona a opção "favoritar".
3. O sistema registra o estabelecimento nos favoritos.

**Pós-condições**
- O estabelecimento aparece na lista de favoritos do usuário.

---

# UC08 — Cadastrar estabelecimentos

**Ator principal:** Administrador

**Descrição:**  
Permite que administradores adicionem novos estabelecimentos ao sistema.

**Pré-condições**
- Administrador autenticado.

**Fluxo principal**

1. O administrador acessa a tela de cadastro.
2. O administrador informa os dados do estabelecimento.
3. O sistema valida as informações.
4. O sistema salva o estabelecimento.

**Pós-condições**
- O estabelecimento é registrado no sistema.

---

# UC09 — Editar detalhes dos estabelecimentos

**Ator principal:** Administrador

**Descrição:**  
Permite alterar informações de um estabelecimento existente.

**Pré-condições**
- Administrador autenticado.
- Estabelecimento existente.

**Fluxo principal**

1. O administrador seleciona um estabelecimento.
2. O administrador edita as informações.
3. O sistema valida os dados.
4. O sistema salva as alterações.

**Pós-condições**
- Informações atualizadas no sistema.

---

# UC10 — Moderar comentários sobre estabelecimentos

**Ator principal:** Administrador

**Descrição:**  
Permite que administradores moderem comentários feitos pelos usuários.

**Pré-condições**
- Administrador autenticado.

**Fluxo principal**

1. O administrador acessa a área de comentários.
2. O sistema lista os comentários.
3. O administrador seleciona um comentário.
4. O administrador pode:
   - aprovar
   - remover
   - ocultar o comentário.

**Pós-condições**
- O comentário é moderado.