# Windmillcode Snippets Zero

# Overview
* have code you want to generate but its not big enough to write a script
but not small enough to copy and paste here are windmillcode snippets zero
to ease development in our day to day applications


# Docs

## SCSS

### Component styles
* used when setting up basis for component styles
* result

$1
```scss
:host {
  &.[COMPONENT_NAME]View {
  }
  .[COMPONENT_NAME]{
    &Main {
    &Pod{
    }
  }
  .Pod{
    &0{}
    }
  }
}
```

### Scss for
* used for css sequences where its better to use a for loop than repeat yourself x times
* result
```scss
@for $i from [START_VALUE_FOR_CSS_RULE] through [END_VALUE_FOR_CSS_RULE] {
  &#{$i} {

  }
}

```


### Import Global Styles
* Used to import global stylesheets into your component or project.
* Result

```scss
@import "src/assets/styles/global.scss";
```


### Numbering Conventions
* Utilized for creating a structured numbering convention in your styles.
* Result

```scss
&[YOUR_NUMBER] {
  &0 {

  }
}
```


### SCSS EM Values
* Generates SCSS for converting pixel values to em units. Always use em units to make responsiveness wayy easier
* Result:

```scss
calc(32/10.6 * 1em) = 32px
```


### SCSS CSS Color Value
* Creates SCSS for referencing CSS color variables using rgba notation. Used to help with color accessiblity and alighing to the UX color scheme even with opacity
* Result:

```scss
--primary-color: "32,64,43";
--secondary-color: "32,64,43";

rgba(var(--primary-color))

// #Examples
rgba(var(--primary-color),.5)

// (Dark mode enalbled)
// if the js script is setup you can now replace the color with a different color and see the update in the dom

```


markdown
Copy code
### SCSS CSS Color Variables
* Facilitates the creation of SCSS variables for CSS color values.
* Result:

```scss
--wml-primary-color:#{\$wml-primary-color};
--wml-orig-primary-color:#{\$wml-primary-color};
```

### @font-face Base64
* Generates an @font-face template for embedding fonts using Base64.
* Result:

```scss
@font-face {
  font-family: '$1';
  font-style: normal;
  font-weight: 900;
  font-display: block;
  src: url(data:font/woff2;base64,) format('woff2'),
       url(data:font/truetype;base64,) format('truetype'),
       url(data:application/vnd.ms-fontobject;base64,) format('embedded-opentype'),
       url(data:image/svg+xml;base64,) format('svg'),
       url(data:font/woff;base64,) format('woff');
}
```


markdown
Copy code
### @font-face URL
* Generates an @font-face template for linking to font files using URLs.
* Result:

```scss
@font-face {
  font-family: '$1';
  font-style: normal;
  font-weight: 900;
  font-display: block;
  src: url('../fonts/$1/$1.woff2') format('woff2'),
       url('../fonts/$1/$1.ttf') format('truetype'),
       url('../fonts/$1/$1.eot') format('embedded-opentype'),
       url('../fonts/$1/$1.svg') format('svg'),
       url('../fonts/$1/$1.woff') format('woff');
}
```



### WML Spacing
* References WML  spacing variables in SCSS.
  * note for best spacing use ()
```
$wml-spacing3,$wml-spacing5,$wml-spacing7
```
* Result:

```scss
padding: $wml-spacing3
```

