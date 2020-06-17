![Sass Em](.repo/banner.png)

[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)

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

body {
    // Single value
    font-size: sass-em.em(16, 16);
    
    // Multiple values
    padding: sass-em.em(20 30, 16);
}

// Mixin

body {
    // Single value
    @include sass-em.em(font-size, 16, 16);
    
    // Multiple values
    @include sass-em.em(padding, 20 30, 16);
}
```

### Legacy @import

```scss
@import "@sass-collective/sass-em";

// Function

body {
    font-size: sass-em(16, 16);
    padding: sass-em(20 30, 16);
}

// Mixin

body {
    @include sass-em(font-size, 16, 16);
    @include sass-em(padding, 20 30, 16);
}
```

### CSS

```css
body {
    font-size: 1em;
    padding: 1.25em 1.875em;
}
```
