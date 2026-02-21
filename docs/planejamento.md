# Urbanly -- Planejamento do MVP

## 1. Definição do Escopo do MVP

### Objetivo do MVP

Validar se: 
- Usuários utilizam busca por palavra-chave para descobrir
locais.
- Estabelecimentos enxergam valor em aparecer com base em
características.
- Recomendações baseadas em localização geram retenção.

------------------------------------------------------------------------

## Funcionalidades do MVP

### Usuário

Incluído: 
- Cadastro/Login (Google ou e-mail)
- Permissão de localização
- Busca por palavra-chave
- Filtro por distância
- Visualização de detalhes do local
- Avaliação (nota 1-5)
- Salvar como favorito

Não incluído: 
- Gamificação
- Chat
- Badges
- IA avançada
- Parcerias com mobilidade
- Monetização
- Feed social

------------------------------------------------------------------------

### Estabelecimentos

Incluído: 
- Cadastro manual via painel admin interno
  - Nome
  - Categoria
  - Descrição
  - Palavras-chave
  - Endereço
  - Fotos
  - Horário

Não incluído: 
- Painel para estabelecimento
- Plano pago
- Estatísticas

------------------------------------------------------------------------

## Arquitetura do MVP

### Stack recomendada

Frontend: 
- React ou Next.js (PWA)
- Tailwind

Backend: 
- Supabase (Auth + Postgres + Storage)
- Edge Functions (se necessário)

Infra: 
- Vercel
- Supabase Cloud

Motivo: 
- Baixo custo
- Entrega rápida
- Escalável

------------------------------------------------------------------------

## 2. Finalidade do MVP

Responder às seguintes perguntas:

1.  As pessoas buscam locais por palavra-chave?
2.  Utilizam localização como filtro?
3.  Avaliações melhoram a busca?
4.  Conseguimos retenção mínima de 30% em D7?

### Métricas de Sucesso

-   (adicionar)

------------------------------------------------------------------------

## 3. Cronograma

Tempo estimado: 8 semanas

### Semana 1 -- Planejamento

-   Definição de requisitos
-   Modelagem de banco
-   Wireframes
-   Definição da stack

### Semanas 2-3 -- Backend

-   Modelagem Postgres
-   Autenticação
-   CRUD de locais
-   Busca por palavra-chave
-   Filtro por localização

### Semanas 4-6 -- Frontend

-   Login
-   Tela principal (busca)
-   Tela de detalhes
-   Avaliações
-   Favoritos

### Semana 7 -- Testes e Deploy

-   Testes funcionais
-   Ajustes UX
-   Deploy

### Semana 8 -- Lançamento Beta

-   Lançamento fechado
-   Coleta de feedback
-   Ajustes rápidos

------------------------------------------------------------------------

## 4. Viabilidade

### Custo Técnico Inicial

-   Supabase Free
-   Vercel Free
-   Domínio

### Custo Operacional

-   Marketing inicial
-   Conteúdo interno

### Viabilidade Técnica

Alta viabilidade. - Sem necessidade de IA complexa - Postgres com
Full-Text Search resolve a busca

------------------------------------------------------------------------

## 5. Principais Riscos

1.  Poucos estabelecimentos cadastrados
    -   Solução: Seed inicial manual
2.  Usuário não entende proposta
    -   Landing clara + tutorial
3.  Concorrência com Google Maps/TripAdvisor
    -   Diferencial: descoberta por "vibe"

------------------------------------------------------------------------

## Escopo Final do MVP

Um aplicativo PWA que permite buscar locais urbanos por palavra-chave
com base na localização do usuário, visualizar detalhes, avaliar e
salvar favoritos.

Sem gamificação. Sem monetização. Sem painel comercial. Foco total em
validação de comportamento.
