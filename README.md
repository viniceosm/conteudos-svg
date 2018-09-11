## Iniciando um SVG

```HTML
<svg width="100" height="100">
</svg>
```

## Formas SVG

- [Rectangle `<rect>`](#rectangle)
- [Circle `<circle>`](#circle)
- [Ellipse `<ellipse>`](#ellipse)
- [Line `<line>`](#line)
- Polyline `<polyline>`
- Polygon `<polygon>`
- [Path `<path>`](#path)

## Rectangle

|Tag atributo|Descrição 
|-|-
|`width`| Define largura.
|`height`| Define altura.
|`x`| Define coordenada no eixo x.
|`y`| Define coordenada no eixo y.
|`rx`| Define um raio no eixo x. Para deixar borda arredondada
|`ry`| Define um raio no eixo y. Para deixar borda arredondada

### Exemplo 1

```HTML
<svg width="400" height="110">
  <rect width="300" height="100" rx="20" ry="20" style="fill:rgb(0,0,255);stroke-width:3;stroke:rgb(0,0,0)" />
</svg>
```

### Exemplo 2

```HTML
<svg width="400" height="110">
  <rect width="300" height="100" x="50" y="20" style="fill:rgb(0,0,255);stroke-width:3;stroke:rgb(0,0,0)" />
</svg>
```

## Circle

|Tag atributo|Descrição 
|-|-
|`cx`| Define coordenada no eixo x.
|`cy`| Define coordenada no eixo y.
|`r`| Define o raio do elemento.

### Exemplo 1

```HTML
<svg width="400" height="110">
  <circle cx="50" cy="50" r="50" />
</svg>
```

## Ellipse

|Tag atributo|Descrição 
|-|-
|`cx`| Define coordenada no eixo x.
|`cy`| Define coordenada no eixo y.
|`rx`| Define um raio no eixo x. Para deixar borda arredondada
|`ry`| Define um raio no eixo y. Para deixar borda arredondada

### Exemplo 1

```HTML
<svg width="400" height="110">
  <ellipse cx="100" cy="50" rx="100" ry="50" />
</svg>
```

## Line
|Tag atributo|Descrição 
|-|-
|`x1`| Define a coordenada do eixo **x** do ponto **inicial** da linha
|`x2`| Define a coordenada do eixo **x** do ponto **final** da linha.
|`y1`| Define a coordenada do eixo **y** do ponto **inicial** da linha
|`y2`| Define a coordenada do eixo **y** do ponto **final** da linha.

### Exemplo 1

```HTML
<svg width="400" height="110">
  <line x1="0" y1="80" x2="100" y2="20" stroke="black" />
</svg>
```

## Path

- M = moveto
- L = lineto
- H = horizontal lineto
- V = vertical lineto
- C = curveto
- S = smooth curveto
- Q = quadratic Bézier curve
- T = smooth quadratic Bézier curveto
- A = elliptical Arc
- Z = closepath

Nota: Todos os comandos acima também podem ser expressos com letras mais baixas. Letras maiúsculas significa absolutamente posicionadas, as letras mais baixas significam relativamente posicionadas.

### Exemplo 1 (triângulo)

Primeiro vértice `150,0`, 2º para `75,200`, 3º para `225,200`, `Z` fecha a forma ligando o terceiro vértice com o primeiro.

```HTML
<svg height="210" width="400">
  <path d="M150 0 L75 200 L225 200 Z" />
</svg>
```
