# Casos de Teste

## Informações Gerais

Projeto: QA API Postman - ServeRest  
Ambiente de Teste: Ambiente público de homologação (https://front.serverest.dev / https://serverest.dev)  
Ferramentas: Chrome / Postman

---

## CT001 - Cadastro de usuário administrador com sucesso

Suite de Teste: Usuários / Cadastro  
Pré-condições: Sistema disponível e email não cadastrado anteriormente.

Passo a passo:
1. Acessar tela de cadastro.
2. Informar nome válido.
3. Informar email novo.
4. Informar senha válida.
5. Marcar opção administrador.
6. Confirmar cadastro.

Resultado Esperado:  
Usuário cadastrado com sucesso.

Resultado Encontrado:
Cadastro realizado com sucesso.

Status: Aprovado

---

## CT002 - Login com credenciais válidas

Suite de Teste: Autenticação / Login  
Pré-condições: Usuário previamente cadastrado.

Passo a passo:
1. Acessar tela de login.
2. Informar email válido.
3. Informar senha correta.
4. Clicar em entrar.

Resultado Esperado: 
Usuário autenticado com sucesso e acesso liberado.

Resultado Encontrado: 
Login realizado normalmente.

Status: Aprovado

---

## CT003 - Login com dados inválidos

**Suite de Teste:** Autenticação / Login  
**Pré-condições:** Tela de login disponível.

**Passo a passo:**
1. Informar email inválido ou inexistente.
2. Informar senha incorreta.
3. Clicar em entrar.

**Resultado Esperado:**  
Sistema bloquear acesso e exibir mensagem de erro.

**Resultado Encontrado:**  
Sistema exige credenciais corretas para acesso.

**Status:** Aprovado

---

## CT004 - Permissão de administrador

Suite de Teste: Usuários / Permissões  
Pré-condições: Usuário cadastrado sem perfil administrador.

Passo a passo:
1. Realizar login com usuário comum.
2. Tentar acessar funções administrativas.

Resultado Esperado:  
Usuário sem permissão não deve acessar funções administrativas.

Resultado Encontrado:  
Acesso restrito corretamente.

Status: Aprovado

---

## CT005 - Listagem de produtos

Suite de Teste: Produtos / Catálogo  
Pré-condições: Sistema disponível.

Passo a passo:
1. Acessar área de produtos.

Resultado Esperado:  
Produtos exibidos para consulta.

Resultado Encontrado: 
Produtos listados normalmente.

Status: Aprovado

---

## CT006 - Adicionar produto ao carrinho

Suite de Teste: Carrinho / Compras  
Pré-condições: Produto disponível para compra.

Passo a passo:
1. Selecionar produto.
2. Adicionar ao carrinho.
3. Repetir ação com outros produtos.

Resultado Esperado:  
Produtos adicionados e acumulados no carrinho.

Resultado Encontrado:  
Carrinho funcionando corretamente.

Status: Aprovado

---

## CT007 - Visualização de detalhes do produto

Suite de Teste: Produtos / Detalhes  
Pré-condições: Produto disponível.

Passo a passo:
1. Selecionar produto listado.
2. Abrir página de detalhes.

Resultado Esperado:
Exibir informações do produto.

Resultado Encontrado: 
Detalhes exibidos corretamente.

Status: Aprovado

---

## CT008 - Pesquisa de produtos

Suite de Teste: Produtos / Busca  
Pré-condições: Produtos cadastrados no sistema.

Passo a passo:
1. Acessar barra de pesquisa.
2. Informar nome parcial ou total do produto.
3. Confirmar busca.

Resultado Esperado:  
Retornar produtos compatíveis com termo pesquisado.

Resultado Encontrado: 
Busca funcionando corretamente.

Status: Aprovado
