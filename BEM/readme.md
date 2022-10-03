## BEM - Block Element Modifier

### Syntax

block - component like nav, form, ul(if you want use it as component)

__element - component item like li, div, img, a, element that doesn't exist outside component

--modifier - class which is a modification of some element

simple example

```yaml
div.block
  img.block__logo
  p.block__paragraph
  p.block__paragraph .block__paragraph--open
  div.block__wrapper-button
    button.block__btn block__button--submit
    button.block__btn block__button--cancel
```
