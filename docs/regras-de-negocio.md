# Regras de Negócio — Sistema Urbanly

---

## RN001 — Avaliação apenas para usuários autenticados

O sistema deve permitir que **apenas usuários autenticados** realizem avaliações e comentários em estabelecimentos.

Caso um usuário não autenticado tente avaliar um estabelecimento, o sistema deve solicitar autenticação antes de permitir a ação.

---

## RN002 — Busca disponível para usuários não autenticados

O sistema deve permitir que **usuários não autenticados realizem buscas por estabelecimentos**, utilizando palavras-chave e filtros disponíveis.

Essa funcionalidade deve estar acessível sem necessidade de login.

---

## RN003 — Limitar uma avaliação por usuário em cada estabelecimento

Cada usuário poderá registrar **apenas uma avaliação por estabelecimento**.

Caso o usuário já tenha avaliado o estabelecimento, o sistema deve permitir:

- editar a avaliação existente
- atualizar nota ou comentário

O sistema não deve permitir múltiplas avaliações do mesmo usuário para o mesmo estabelecimento.

---

## RN004 — Associação obrigatória de palavras-chave aos estabelecimentos

Todo estabelecimento cadastrado deve possuir **pelo menos uma palavra-chave associada**.

As palavras-chave serão utilizadas para:

- indexação
- busca
- filtragem de resultados

O sistema não deve permitir o cadastro de estabelecimentos sem palavras-chave.

---

## RN005 — Exibir apenas estabelecimentos ativos

O sistema deve exibir nos resultados de busca **apenas estabelecimentos com status ativo**.

Estabelecimentos removidos ou desativados pelo administrador não devem ser apresentados aos usuários.

---

## RN006 — Garantir consistência das palavras-chave cadastradas

O sistema deve garantir que **palavras-chave associadas a um estabelecimento sejam únicas**, evitando duplicidade dentro do mesmo estabelecimento.

Isso garante consistência e melhor qualidade nos resultados de busca.

---

## RN007 — Informações resumidas para usuários não autenticados

Usuários não autenticados devem visualizar **apenas informações resumidas dos estabelecimentos** nos resultados de busca.

As informações exibidas devem incluir apenas:

- nome do estabelecimento
- categoria
- cidade
- avaliação média

Informações detalhadas devem ser ocultadas até que o usuário realize login.

---

## RN008 — Visualização completa apenas para usuários autenticados

Informações completas de um estabelecimento devem estar disponíveis **apenas para usuários autenticados**.

Essas informações incluem:

- descrição completa
- endereço detalhado
- fotos do estabelecimento
- avaliações de usuários
- comentários

Caso um visitante tente acessar essas informações, o sistema deve solicitar autenticação.
