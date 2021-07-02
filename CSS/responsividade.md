# Responsividade

## CSS Units

Unidades de medidas do CSS

Layout Fixo/duro/enrijecido e sem adaptação

`px` - Pixels

Layou Fluído/Flexível e adaptável

`%` - Porcentagem
`auto` - Automática
`vh` - Viewport Height
`vw` - Viewport Width

Textos fixos

`1px` = 0.75pt
`16px` = 12pt

Texto fluidos

`em` - multiplicado pelo tamanho em `px` especificado no elemento pai do elemento cujo o qual o tamanho em `em` foi aplicado
`rem` - multiplciado pelo tamanho em `px` especificado no elemento `root` (html)

### OBS: Lembrar de aplicar tag meta no html: ``` <meta name="viewport" content="width=devide-width, initial-scale=1.0"> ```

## CSS Media Queries

```css
    @media (max-wdth: 320px) {
        #form h3 {
            font-size: 2rem.
        }
    }
```

## HTML Media Attributes

## Imagens

`<picture>`

JPG, PNG, SVG