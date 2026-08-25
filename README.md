# Mapa-interativo
Criado para a uso unicamente da USP
https://odonto-usp.github.io/Mapa-interativo/?hl=pt-BR
## 🎨 Como Alterar ou Adicionar Novos Ícones (.png)

Siga o passo a passo abaixo para incluir novas marcações ou substituir os símbolos existentes no mapa:

### 1. Adicionar o arquivo de imagem
1. Coloque a nova imagem no formato `.png` dentro da **mesma pasta** onde está o `index.html` (na raiz do repositório).
2. Use imagens com **fundo transparente** (PNG sem fundo) e proporção quadrada (ex: 32x32 ou 64x64 pixels).

---

### 2. Atualizar o dicionário `CATEGORIAS` no `index.html`
Abra o arquivo `index.html`, localize a constante **`CATEGORIAS`** no início do `<script>` e adicione a nova opção com um número único:

```javascript
const CATEGORIAS = {
  "1": { nome: "Igreja", arquivo: "igreja.png" },
  "2": { nome: "Aluguel", arquivo: "aluguel.png" },
  "3": { nome: "Cabeleireiro", arquivo: "cabelereiro.png" },
  "4": { nome: "Faixa de Pedestre", arquivo: "faixa-de-pedestre.png" },
  "5": { nome: "Acidente Elétrico", arquivo: "acidente-eletrico.png" },
  "6": { nome: "Dengue", arquivo: "dengue.png" },
  "7": { nome: "Ponto de Ônibus", arquivo: "ponto-de-onibus.png" },
  // Adicione a nova categoria aqui:
  "8": { nome: "Nome da Categoria", arquivo: "nome-do-arquivo.png" }
};
