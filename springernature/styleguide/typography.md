# Typography

## Principles

**Create clear hierarchy**
Our typographic system uses font weight, scale and positioning to reflect the information hierarchy. 

Use semantic heading levels to create identifiable sections that are easy to scan.

**Design to be legible**
Our fonts, text colours and type spacing helps users to easily read text with minimal effort.  

## Typefaces
The Springer Nature brand uses the open-source Merriweather family. [Download the font files from the frontend toolkit on GitHub](https://github.com/springernature/frontend-toolkits/tree/main/context/brand-context/springernature/fonts).

### Merriweather sans
Merriweather Sans is the default typeface for Springer Nature. It’s designed to be readable at very small sizes and on low resolution screens.

Use it for body text, including:

- interactive elements, like buttons, forms and navigation links
- form elements, like text labels, hints and error messages
- instructional text and status messages
- secondary text such as metadata, author names and publication dates

![Type specimen of the Merriweather Sans font showing the alphabet and numbers.](https://user-images.githubusercontent.com/15365576/202757703-fcf98d2f-4eaf-4683-a4a7-7a7b94d0e247.png)


### Merriweather
Merriweather is a serif typeface that works harmoniously with Merriweather sans.

Use it for headings and long form content such as articles and book chapters. 

![Type specimen of the Merriweather font showing the alphabet and numbers.](https://user-images.githubusercontent.com/15365576/202757861-750fe579-9e92-4df6-a90a-0686a7b46662.png)

### Installation

Font files are provided in the [frontend toolkits](https://github.com/springernature/frontend-toolkits), in the brand-context package. Each brand includes a **/fonts** folder. You will need to create a CSS or Sass file to reference the fonts using `@font-face`. This should be the first stylesheet you import.

The Merriweather fonts, used by the Springer Nature brand, are variable fonts. The relevant weights, 300 and 700, are listed by each font’s font-weight property.

```
@font-face {
	font-family: 'Merriweather';
	src: url('../fonts/Merriweather-Variable.woff2') format('woff2 supports variations'),
	url('../fonts/Merriweather-Variable.woff2') format('woff2-variations');
	font-weight: 300 700;
	font-display: swap;
}



@font-face {
	font-family: 'Merriweather Sans';
	src: url('../fonts/MerriweatherSans-Variable.woff2') format('woff2 supports variations'),
	url('../fonts/MerriweatherSans-Variable.woff2') format('woff2-variations');
	font-weight: 300 700;
	font-display: swap;
}
```

The `font-display`: swap property ensures a system font is displayed until the web font is downloaded. The relevant brand-context stylesheets add suitable fallback fonts in the font-family declaration.

```
font-family: "Merriweather Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
```


## Applying typography

### Design tokens
We use [design tokens](https://github.com/springernature/frontend-toolkits/tree/main/context/design-tokens) instead of hard coded values to support an easily maintainable UI across our products.

For typography, we use literal tokens to define type size, weight, letter spacing and line height. 

Alias tokens define our typographic decisions, such as the styles for body text and headings. 

### Typographic scale
Our type scale reinforces visual hierarchy. We use tokens to define each type size, using rem units to ensure consistency throughout the UI. The base size is 1rem (16px).

![An example of every font size](https://user-images.githubusercontent.com/15365576/202760380-f5320815-dc6a-4ddf-9bde-6fd9bd0eff9b.png)


### Headings

Use the `heading-level` token to set the visual size and weight of the heading. This token does not affect the semantic heading level. [Always use semantic levels correctly](https://www.w3.org/WAI/tutorials/page-structure/headings/).  

We use the alias token `fluid` to scale headings for small screens. For example, `heading-level-1` will use the same style as `heading-level-2` on a smaller viewport.

![Panel](https://user-images.githubusercontent.com/15365576/202760823-4a2c6b33-86fb-4dda-b554-1ca30ad57c02.png)

### Line length

For sentences or paragraphs, do not exceed a line length of 90 characters to maintain a comfortable reading length for users. Text that stretches beyond this limit makes it harder to scan for information and more difficult for the eye to track progress.

![Panel](https://user-images.githubusercontent.com/15365576/202774007-d771099b-db26-4d94-9d26-052aa7191ba5.png)


### Spacing

### Line height
We use `line-height` tokens to set the spacing between lines of text in the same paragraph. 

Use `line-height` that is proportional to the font size. For example, when setting paragraph text that uses `font-size-400` (16px), use `$line-height-md`. Lines that are too close together will [negatively impact the readability of your content](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-visual-presentation.html). 
 
 ![Panel](https://user-images.githubusercontent.com/15365576/202774569-e2f08c01-5fbd-4692-a8b4-4c56672e0faf.png)

### Block spacing
Use block spacing to place margins before paragraph and heading elements. Always use the 8px grid for spacing elements to ensure consistency.
 
 ![Group](https://user-images.githubusercontent.com/15365576/202774847-feaaa065-21af-4623-9937-7bba236315a3.png)

## Tools for designers
- Use the Sketch styleguide to use the Elements typography styles in your designs
- If you’re designing in Sketch, we recommend using the stark plugin to the check colour contrast of text in your designs

 
