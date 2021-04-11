![Sass Em](.github/banner.png)

[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)

> **DEPRECATED:** this package has been moved to new reference in Sass Collective [monorepo](https://github.com/sass-collective/sass-collective/tree/master/packages/em) `@sass-collective/em`, use this package because the current repository is no more maintained.

## Introduction

Sass function & mixin to generate em value.

## Install

    npm install @sass-collective/sass-em --save

## Usage

### Function

```scss
em($values, $context);
```

### Mixin

```scss
em($property, $values, $context);
```

### Module System

```scss
@use "@sass-collective/sass-em";

// Function

html,
body {
    // Single value
    font-size: sass-em.em(16, 16);
    
    // Multiple values
    margin: sass-em.em(20 30, 16);
}

// Mixin

html,
body {
    // Single value
    @include sass-em.em(font-size, 16, 16);
    
    // Multiple values
    @include sass-em.em(margin, 20 30, 16);
}
```

### Legacy @import

```scss
@import "@sass-collective/sass-em";

// Function

html,
body {
    font-size: sass-em(16, 16);
    margin: sass-em(20 30, 16);
}

// Mixin

html,
body {
    @include sass-em(font-size, 16, 16);
    @include sass-em(margin, 20 30, 16);
}
```

### CSS

```css
html,
body {
    font-size: 1em;
    margin: 1.25em 1.875em;
}
```
