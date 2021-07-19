# sphinx-design

A sphinx extension for designing beautiful, size responsive web components.

Created with inspiration from [Bootstrap](https://getbootstrap.com/) (v5), [Material Design](https://material.io) and [Material-UI](https://material-ui.com/) design frameworks.

## Cards

:::{card}
:width: 25
:margin: 0 2 auto auto
:text-align: center

align center
:::

:::{card}
:width: 50
:margin: 0 2 auto 0
:text-align: right

align right
:::

:::{card}
:width: 50
:margin: 0 2 0 auto
:text-align: left

align left
:::

paragraph

## Grids

::::{grid}
:columns: 1 2 2 3
:gutter: 1 3 3 3

:::{grid-item}

hallo

:::

:::{grid-item-card}
:img-top: https://via.placeholder.com/150
:img-bottom: https://via.placeholder.com/150

there df sdf  dsf  dsf  dfs   dsf  fds dsf

:::

:::{grid-item-card}
:text-align: center

a header
^^^
again [abc](https://google.com)
+++
a footer

:::

:::{grid-item-card} Card title
:columns: 12 6 6 6

bigger

+++

Footer

:::

:::{grid-item-card}
:columns: 12 6 6 6

bigger

more

+++

Footer

:::

::::

next paragraph 1

::::{grid}
:columns: 1 1 2 2
:gutter: 0 0 2 4
:text-align: justify

:::{grid-item}
{{ loremipsum }}
:::

:::{grid-item}
{{ loremipsum }}
:::

::::

### Nested grids

::::::{grid}
:columns: 1 1 2 2
:gutter: 1

:::::{grid-item}

::::{grid}
:columns: 1 1 1 1
:gutter: 1

:::{grid-item-card}

{{ loremipsum }}

:::

:::{grid-item-card}

B

:::

::::

:::::

:::::{grid-item}

::::{grid}
:columns: 1 1 1 1
:gutter: 1

:::{grid-item-card}

C

:::

:::{grid-item-card}

D

:::

:::{grid-item-card}

E

:::

::::

:::::

::::::

(badges)=

## Badges

- {bdg}`plain badge`
- {bdg-primary}`primary` {bdg-primary-line}`primary-line`
- {bdg-secondary}`secondary` {bdg-secondary-line}`secondary-line`
- {bdg-success}`success` {bdg-success-line}`success-line`
- {bdg-info}`info` {bdg-info-line}`info-line`
- {bdg-warning}`warning` {bdg-warning-line}`warning-line`
- {bdg-danger}`danger` {bdg-danger-line}`danger-line`
- {bdg-light}`light` {bdg-light-line}`light-line`
- {bdg-dark}`dark` {bdg-dark-line}`dark-line`

{bdg-link-primary}`name <https://example.com>`

{bdg-link-primary-line}`name <https://example.com>`

{bdg-ref-primary}`badges`

(buttons)=

### Buttons

```{button-link} https://example.com
```

```{button-ref} buttons
```

```{button-link} https://example.com
Button text
```

```{button-ref} buttons
Button text
```

```{button-link} https://example.com
:color: primary
```

```{button-link} https://example.com
:color: primary
:outline:
```

```{button-link} https://example.com
:color: secondary
:expand:
```

:::{card} Card with an expanded button
:hover:

```{button-link} https://example.com
:color: info
:click-parent:
```

:::

## Dropdown

:::{dropdown} Dropdown title
Dropdown content
:::

:::{dropdown}
Dropdown content
:::

::::{dropdown} Parent dropdown title (open by default)
:open:

:::{dropdown} Child dropdown title
:color: warning
:icon: alert

Dropdown content
:::
::::

### Dropdowns in a grid

:::::{grid}
:columns: 1 1 2 2
:gutter: 1

::::{grid-item}
:::{dropdown} Dropdown title
Dropdown content
:::
::::

::::{grid-item}
:::{dropdown} Dropdown title
Dropdown content
:::
::::

:::::

## Icons

Some {opticon-16}`report;sd-text-info` middle {opticon-24}`report` more text

{fas}`spinner;sd-bg-primary sd-bg-text-primary fa-2x`