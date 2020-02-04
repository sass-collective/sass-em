# Sass Em

Generate em CSS value.

## Install

    npm install @sass-collective/sass-em --save

## Usage

### Global @import

#### Sass

    @import "@sass-collective/sass-em"

    body {
        font-size: sass-em(16);
    }

#### CSS 

    body {
        font-size: 1em;
    }

### Module System

#### Sass

    @use "@sass-collective/sass-em"

    // Function

    body {
        font-size: sass-em.em(16);
    }

    // Mixin

    body {
        @include sass-em.em(16);
    }

#### CSS

    body {
        font-size: 1em;
    }
