---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


# Instalação

### Primeiro, vamos instalar o componente!

Existem várias maneiras de começar a usar o Bulma Tooltip.

### NPM <sup>_recomendado_</sup>

```shell
npm install bulma-v1-tooltip
```

### CDN

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma-v1-tooltip/dist/bulma-v1-tooltip.min.css">
```

---

# Usando o componente

As dicas de ferramentas são exibidas em uma pequena caixa cinza na parte superior do elemento. Tudo o que você precisa fazer é adicionar o atributo `data-tooltip` com o texto que deseja exibir como valor.

## Estilos

### Padrão

> <span class="has-text-dark">Lorem ipsum dolor sit amet, <span data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores earum quod distinctio ducimus non dignissimos..</span>

```html
<p>
  Lorem ipsum dolor sit amet, <span data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores earum quod distinctio
  ducimus non dignissimos..
</p>
```

Tooltip pode ser usado em qualquer tipo de elemento HTML que suporte conjunto de dados.

<button class="button" data-tooltip="Tooltip content">Button</button>

```html
<button class="button" data-tooltip="Tooltip content">Button</button>
```

---

### Com seta

Para fins de design, você pode exibir uma seta no tooltip adicionando a classe `has-tooltip-arrow` no elemento

> <p class="has-text-dark">Lorem ipsum dolor sit amet, <span class="has-tooltip-arrow" data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores earum quod distinctio ducimus non dignissimos molestias amet corrupti voluptatum assumenda impedit beatae veritatis nemo veniam error, hic cumque.</p>

```html
<p>
  Lorem ipsum dolor sit amet, <span class="has-tooltip-arrow" data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores
  earum quod distinctio ducimus non dignissimos molestias amet corrupti voluptatum assumenda impedit beatae veritatis nemo veniam error, hic cumque.
</p>
```

---

### Posição

A posição do tooltip pode ser alterado adicionando uma das seguintes classes ao elemento HTML que contém a dica de ferramenta: `has-tooltip-right`, `has-tooltip-bottom`, `has-tooltip-left`.

> <p class="has-text-dark">Lorem ipsum dolor sit amet, <span class="has-tooltip-arrow" data-tooltip="Tooltip content on top">consectetur adipisicing elit</span>. Ipsa fugit <span class="has-tooltip-arrow has-tooltip-right" data-tooltip="Right tooltip content">dolores</span> earum quod distinctio ducimus non dignissimos <span class="has-tooltip-arrow has-tooltip-bottom" data-tooltip="Bottom tooltip content">molestias</span> amet corrupti voluptatum assumenda impedit beatae <span class="has-tooltip-arrow has-tooltip-left" data-tooltip="Left tooltip content">veritatis</span> nemo veniam error, hic cumque.</p>

```html
<p>
  Lorem ipsum dolor sit amet, <span class="has-tooltip-arrow" data-tooltip="Tooltip content on top">consectetur adipisicing elit</span>. Ipsa fugit
  <span class="has-tooltip-arrow has-tooltip-right" data-tooltip="Right tooltip content">dolores</span> earum quod distinctio ducimus non dignissimos
  <span class="has-tooltip-arrow has-tooltip-bottom" data-tooltip="Bottom tooltip content">molestias</span> amet corrupti voluptatum assumenda impedit
  beatae <span class="has-tooltip-arrow has-tooltip-left" data-tooltip="Left tooltip content">veritatis</span> nemo veniam error, hic cumque.
</p>
```

---

### Multilinha

Exiba o conteúdo longo no tooltip adicionando a classe `has-tooltip-multiline` ao elemento.

Você pode alterar o alinhamento do texto adicionando o modificador `has-tooltip-text-left`, `has-tooltip-text-centered` ou `has-tooltip-text-right`

> <p class="has-text-dark">Lorem ipsum dolor sit amet, <span class="has-tooltip-arrow has-tooltip-multiline has-tooltip-text-centered" data-tooltip="Ipsa fugit dolores earum quod distinctio ducimus non dignissimos molestias amet corrupti voluptatum assumenda impedit beatae veritatis nemo veniam error, hic cumque.">consectetur adipisicing elit</span>. </p>

```html
<p>
  Lorem ipsum dolor sit amet,
  <span
    class="has-tooltip-arrow has-tooltip-multiline has-tooltip-text-centered"
    data-tooltip="Ipsa fugit dolores earum quod distinctio ducimus non dignissimos molestias amet corrupti voluptatum assumenda impedit beatae veritatis nemo veniam error, hic cumque."
    >consectetur adipisicing elit</span>
</p>
```

---

### Cores

o tooltip oferece suporte ao modificador de cores adicionando uma das seguintes classes ao elemento HTML que contém o tooltip: `has-tooltip-info`, `has-tooltip-warning`, `has-tooltip-primary`, `has-tooltip-success`, `has-tooltip-danger`.

> <p class="has-text-dark">Lorem ipsum <span class="has-tooltip-arrow has-tooltip-info" data-tooltip="Info tooltip content">dolor</span> sit amet, <span class="has-tooltip-arrow has-tooltip-warning" data-tooltip="Warning tooltip content">consectetur adipisicing elit</span>. Ipsa fugit <span class="has-tooltip-arrow has-tooltip-right has-tooltip-success" data-tooltip="Success tooltip content">dolores</span> earum quod distinctio ducimus non dignissimos <span class="has-tooltip-arrow has-tooltip-bottom has-tooltip-primary" data-tooltip="Primary tooltip content">molestias</span> amet corrupti voluptatum assumenda impedit beatae <span class="has-tooltip-arrow has-tooltip-left has-tooltip-danger" data-tooltip="Danger tooltip content">veritatis</span> nemo veniam error, hic cumque.</p>

```html
<p>
  Lorem ipsum <span class="has-tooltip-arrow has-tooltip-info" data-tooltip="Info tooltip content">dolor</span> sit amet,
  <span class="has-tooltip-arrow has-tooltip-warning" data-tooltip="Warning tooltip content">consectetur adipisicing elit</span>. Ipsa fugit
  <span class="has-tooltip-arrow has-tooltip-right has-tooltip-success" data-tooltip="Success tooltip content">dolores</span> earum quod distinctio
  ducimus non dignissimos
  <span class="has-tooltip-arrow has-tooltip-bottom has-tooltip-primary" data-tooltip="Primary tooltip content">molestias</span> amet corrupti
  voluptatum assumenda impedit beatae
  <span class="has-tooltip-arrow has-tooltip-left has-tooltip-danger" data-tooltip="Danger tooltip content">veritatis</span> nemo veniam error, hic
  cumque.
</p>
```

---

### Sempre ativo

Você pode definir o tooltip para estar sempre visível adicionando a classe `has-tooltip-active` no elemento.<br/><br/>

> <p class="has-text-dark">Lorem ipsum dolor sit amet, <span class="has-tooltip-active" data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores earum quod distinctio ducimus non dignissimos.</p>

```html
<p>Lorem ipsum dolor sit amet, <span class="has-tooltip-active" data-tooltip="Tooltip content">consectetur adipisicing elit</span>. Ipsa fugit dolores earum quod distinctio ducimus non dignissimos.
</p>
```

---

### Responsividade

#### Posição

A posição do tooltipo pode ser baseada em breakponts responsivos adicionando uma das seguintes classes ao elemento HTML que contém o tooltip:

- `has-tooltip-#{$direction}-mobile`
- `has-tooltip-#{$direction}-tablet`
- `has-tooltip-#{$direction}-tablet-only`
- `has-tooltip-#{$direction}-touch`
- `has-tooltip-#{$direction}-desktop`
- `has-tooltip-#{$direction}-desktop-only`
- `has-tooltip-#{$direction}-until-widescreen`
- `has-tooltip-#{$direction}-widescreen`
- `has-tooltip-#{$direction}-widescreen-only`
- `has-tooltip-#{$direction}-until-fullhd`
- `has-tooltip-#{$direction}-fullhd`

Não se esqueça de substituir `#${direction}` por uma das direções disponíveis: `top`, `right`, `bottom`, `left`.

#### Alinhamento de texto

- `has-tooltip-text-#{$direction}-mobile`
- `has-tooltip-text-#{$direction}-tablet`
- `has-tooltip-text-#{$direction}-tablet-only`
- `has-tooltip-text-#{$direction}-touch`
- `has-tooltip-text-#{$direction}-desktop`
- `has-tooltip-text-#{$direction}-desktop-only`
- `has-tooltip-text-#{$direction}-until-widescreen`
- `has-tooltip-text-#{$direction}-widescreen`
- `has-tooltip-text-#{$direction}-widescreen-only`
- `has-tooltip-text-#{$direction}-until-fullhd`
- `has-tooltip-text-#{$direction}-fullhd`

Não se esqueça de substituir `#${direction}` por uma das direções disponíveis: `top`, `right`, `bottom`, `left`.

#### Visibilidade
<div style="overflow:auto">
<table class="table" style="width:800px">
		<thead>
			<tr>
				<th>Class</th>
				<th>Mobile</th>
				<th>Tablet</th>
				<th>Desktop</th>
				<th>Widescreen</th>
				<th>FullHD</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>has-tooltip-hidden-mobile</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-tablet-only</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-desktop-only</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-widescreen-only</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-touch</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-tablet</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-desktop</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-widescreen</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
			</tr>
			<tr>
				<td>has-tooltip-hidden-fullhd</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-success">visible</span>
				</td>
				<td>
					<span class="tag is-danger">hidden</span>
				</td>
			</tr>
		</tbody>
	</table>
</div>

