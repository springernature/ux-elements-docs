# Spacing

## Approach
Our approach uses [gestalt principles](https://lawsofux.com/law-of-proximity/), which describe how humans process visual information. By using these principles, we can help users comprehend and interpret the user interface. 

For example, when UI elements are positioned closer together, users perceive them to share similar functionality.

We define our measurements as a set of spacing units, with 16px or 1rem as our base unit. Each spacing unit is stored as a design token and can be applied to components on the interface.

## Implementation
You can find tokens for each spacing unit inside the `literal` folder. They are then used by the `alias` tokens for `margin`, `padding`, and `gap`.

### Layout components
When adding spacing between components:

- use the [layout stack component](https://elements.springernature.com/springernature/components/global-layout-stack) for vertical space
- use the [layout cluster component](https://elements.springernature.com/springernature/components/global-layout-cluster) for grouped inline elements

For more information on our approach to layout, [go to the layout guide](https://elements.springernature.com/springernature/styleguide/layout).

### Logical properties
We use [logical properties](https://web.dev/learn/css/logical-properties/) and values to help our websites cater to right to left languages, such as Arabic. Unlike physical properties (left,right,top and bottom) logical properties will adapt the layout to the context of the language.

![A text link next to an icon is displayed in both English and Arabic. Text labels are used to show the start and end of the text. The English text goes left to right with the icon on the left. The Arabic text goes right to left, with the icon on the right](https://user-images.githubusercontent.com/15365576/224795402-d1a422b3-8fdf-4875-a220-0bffdc0d5aeb.png)

When setting `margin` space with logical properties, use the following:

| Logical property | Physical property |
| ---------------- | ----------------- | 
| margin-inline    | “left” and “right” on both sides |
| margin-inline-start   | “left” (the start of an element) |
| margin-inline-end    | “right” (the end of an element) |
| margin-block    | “top” and “bottom” |
| margin-block-start    | “top” |
| margin-block-end    | “bottom” |

Remember that logical properties also apply to `border` and `padding`.


## Spacing units
Spacing units use a base value of 16px and use multiples of 8 to make it easy to scale across designs and establish consistency. Do not use a spacing value outside of this system.

When designing in sketch, you can move objects by 8px increments by going to Sketch > Settings > Canvas in the top menu.

![A table showing a scale of spacing values, with 3 columns representing the pixel value, rem value and token name. 64px equates to 4rem and uses the 1600 token, 48px equates to 3rem and uses the 1200 token, 32px equates to 2rem and uses the 800 token, 24px equates to 1.5rem and uses the 600 token, 16px equates to 1rem and uses the 400 token, 8px equates to 0.5rem and uses the 200 token, 4px equates to 0.25rem and uses the 100 token](https://user-images.githubusercontent.com/15365576/224798603-d23878ad-4cf1-492e-ae2f-8209502a2dfc.png)

## Applying spacing

### Padding

Padding is the internal space between a UI element's boundaries and its content. 

If your component has a visible edge, such as a border or background colour, apply padding around the content. This will help make the content more readable.

Do not use padding for space between different components. Use margin instead.

![A card component containing a title, paragraph and two text links stacked vertically on a blue background. Next to this is an illustration of a female scientist. A purple highlight fills the space between the inner edge of the card and the text elements, showing how to apply a padding token of 400](https://user-images.githubusercontent.com/15365576/224799053-9e342cd1-46bb-4b40-9199-043f7e5fb447.png)

### Margins

Margins are the space around an element. For example, the space between the heading of the paragraph and the link.

![A card component containing a title, paragraph and two text links stacked vertically on a blue background. Next to this is an illustration of a female scientist. Orange blocks in between the text elements show how different values of spacing are applied using margin-block-end tokens of 200 and 600](https://user-images.githubusercontent.com/15365576/224802055-821a6f28-8014-49b9-8773-f744c28faa54.png)

### Gap

Gaps (also known as gutters) are the space between each column or row within a layout. 

Use a gap of `400` (16px) or more to provide a clear separation between components. This helps make information easier to understand. This is especially important if your component has no visible edge.

![A two column grid of cards, each containing a heading and some text. A green vertical block between the two columns represents how a gap token of 400 is being applied](https://user-images.githubusercontent.com/15365576/224803013-54974400-ac1b-492b-8790-e840db8e6c32.png)

### Grouping elements
Users will understand elements that are closer together as related and sharing functionality.

For example, group a text label and input field together by using less space, and separate them from other fields by using more space. 

Use larger spacing values like `600`(24px), `800`(32px) and `1200`(48px) to separate groups of elements or components from each other.

![A h1 heading and three text input fields that are stacked vertically underneath. Orange blocks represent the margin space in between each text input. The biggest space uses the margin-block-end-1200 token to separate the h1 heading from the first text input. The space between the text label and input field uses the margin-block-end-100 token. The space between each text input through the form uses the margin-block-end-600 token](https://user-images.githubusercontent.com/15365576/224803878-ed0bf5c9-6f51-4af5-acce-ad9cf85b9768.png)

### Vertical rhythm
Use spacing on long form content to create a vertical rhythm which helps make the text easier to read.

The contrast in spacing also helps establish a visual hierarchy and makes the content easier to scan. Use the following spacing values help achieve a vertical rhythm:

![A diagram showing an example of a long form article. Orange blocks represent the margin space between each text element. The biggest space uses the margin-block-start-1200 token to separate the h2 from the h1 heading. The space between the h2 and paragraph text underneath uses the margin-block-end-400 token. The space above each h3 heading uses the margin-block-end-800 token. The space between each h3 heading and paragraph text uses the margin-block-end-200 token.](https://user-images.githubusercontent.com/15365576/224804458-f51add0a-f47e-482c-8937-be633f61f18f.png)

### Information density
Information density is the amount of human-readable information within an area of the viewport. A user’s perception of space between information can impact their ability to understand the data or content, as well as the speed they do so.

For components with high information density, such as a table, use smaller units of spacing to help fit more content within a viewport. Make sure the content is still easy to read.

![A two column table with the first column containing location data and the second column containing the number of accesses. On the first row, a purple highlight fills the space between the inner edge of the cells and the content. The top and bottom space use the padding-inline-400 token. The left and right sides use the padding-inline-200 token](https://user-images.githubusercontent.com/15365576/224805349-8315b59d-55dc-4489-9374-0ce38d440db3.png)


## Resources
- [Gestalt psychology, Encyclopedia of Animal Cognition and Behavior ](https://link.springer.com/referenceworkentry/10.1007/978-3-319-55065-7_1257#Sec7231)
- [Space in Design Systems](https://medium.com/eightshapes-llc/space-in-design-systems-188bcbae0d62)

