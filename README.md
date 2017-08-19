# Practical Property Sets

**[Practical Property Sets]** are a collection of meaningful property sets
designed to help you write cleaner, scalable, and easier to maintain CSS.

They are built upon the [CSS @apply Rule].

```sh
npm install --save-dev jonathantneal/practical-property-sets
```

## Usage

Practical Property Sets are used like extensions for rules. Their purposeful
names make them highly readable and reusable.

*Before*:
```css
.my-image {
  @apply --c-ratio-styles;
  @apply --c-ratio-cinema-styles;
}

/* becomes */

.my-image {
  display: block;
  position: relative;
}

.my-image::before {
  content: "";
  display: block;
  padding-top: 41.841%;
}

.my-image > :first-child {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
```

[Practical Property Sets]: https://github.com/jonathantneal/practical-property-sets
[CSS @apply Rule]: http://tabatkins.github.io/specs/css-apply-rule/
[Nicole Sullivan]: https://github.com/stubbornella
[Object Oriented CSS]: https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss/
