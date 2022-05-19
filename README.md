# Media queries for standard devices

Sass files with mixins for getting any @media query for mobile view.

An idea had arisen from article [Media queries for standards devices](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

### Mobile models

```txt
iPhone: 4, 4S, 5, 5S, 5C, 5SE, 6, 6S, 7, 8, 6+, 7+, 8+ and high (default)
Galaxy: S3, S4, S5, Note3 and high (default)
Pixel: XL and other (default)
Nexus: 4, 5, and other (default)
```

### Tablet models

```txt
iPad: 1, 2, 3, 4, Air, Mini, Pro 9.7'', Pro 10.5'', Pro 12.9'' and other (default)
Galaxy Tab: 2, S, and other (default)
Nexus: 7, 9, and other (default)
Kindle Fire: HD 7'', HD 8.9'' and other (default)
```

### Using

```sass
.container {
  @include iphone('5S') {
    /* styles for iphone 5s width */
  }
}
.container {
  @include galaxy_t(null, 'portrait') {
    /* styles for galaxy tab all models, exeption 2, and for only portrait orientation */
  }
}
```
