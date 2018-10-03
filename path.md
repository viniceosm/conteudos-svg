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

Nota:
- Todos os comandos acima também podem ser expressos com letras mais baixas.
- Letras **maiúsculas** significa **absolutamente** posicionadas
- Letras **minúsculas** significam **relativamente** posicionadas.

### Exemplo 1 (triângulo)

Primeiro vértice `150,0`, 2º para `75,200`, 3º para `225,200`, `Z` fecha a forma ligando o terceiro vértice com o primeiro.

```HTML
<svg height="210" width="400">
  <path d="M150 0 L75 200 L225 200 Z" />
</svg>
```
