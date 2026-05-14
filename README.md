# Desafio Prático: Expandindo o Projeto Esporte Total

**Objetivo:** Criar páginas internas específicas para cada esporte, interligar a navegação e aplicar conceitos de acessibilidade com ARIA.

## Passo 1: Estrutura de Arquivos
1. Crie uma pasta chamada `paginas` na raiz do seu projeto.
2. Dentro da pasta `paginas`, crie três novos arquivos HTML:
   - `futebol.html`
   - `basquete.html`
   - `volei.html`

## Passo 2: Adaptação de Conteúdo
1. Copie a estrutura base da sua `index.html` e cole nos novos arquivos.
2. Altere a tag `<title>` de cada página para refletir o conteúdo (ex: `<title>Futebol - Esporte Total</title>`).
3. Modifique os títulos (`<h1>`, `<h2>`) e os textos dos parágrafos para falar especificamente sobre o esporte da respectiva página.

## Passo 3: Ajuste da Navegação (Hyperlinks)
Atualize os links (`href`) do cabeçalho em **todas as páginas** para que a navegação funcione perfeitamente entre a raiz e as subpastas.

**Atenção aos caminhos relativos:**
- Da `index.html` para as internas: `./paginas/nome-da-pagina.html`
- Das internas para a `index.html`: `../index.html`
- De uma interna para outra: `./nome-da-pagina.html`

## Passo 4: Imagens e Ícones
1. Substitua as imagens de destaque (Hero/Banners) para que correspondam ao esporte da página atual.
2. Adicione novas imagens ilustrativas ou ícones para enriquecer o layout e diferenciar visualmente cada seção.

## Passo 5: Acessibilidade (Foco em ARIA)
O uso do `aria-label` é **obrigatório** em todo o projeto. Aplique-o estrategicamente onde o contexto visual não for suficiente para leitores de tela:
- **Links genéricos:** Transforme links como "mais..." em botões acessíveis.
  *Ex: `<a href="#" aria-label="Leia mais sobre as regras do basquete">mais...</a>`*
- **Navegação:** Identifique seus menus.
  *Ex: `<nav aria-label="Navegação Principal">`*
- **Ícones decorativos:** Se utilizar ícones apenas para visual, esconda-os do leitor de tela usando `aria-hidden="true"`.

---
**Critério de Aceite:** O projeto será considerado concluído quando for possível navegar por todas as páginas através do menu superior sem encontrar links quebrados (Erro 404), e todos os botões de ação possuírem rótulos acessíveis.