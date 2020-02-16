![Sass Em](.repo/banner.png)

[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-em)](https://www.npmjs.com/package/@sass-collective/sass-em)

## Introduction

Generate em CSS value.

## Install

    npm install @sass-collective/sass-em --save

## Usage

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

### Legacy @import

#### Sass

    @import "@sass-collective/sass-em"

    // Function

    body {
        font-size: sass-em(16);
    }

    // Mixin

    body {
        @include sass-em(16);
    }

#### CSS 

    body {
        font-size: 1em;
    }
