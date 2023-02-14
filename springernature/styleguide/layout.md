# Layout

## Approach

Design layouts so that they can adapt to any viewport or screen size. Think about the content you need to display and how you would structure it in a single column first.

Our audience uses a very large range of devices and screen sizes. They may be using multiple windows on a screen and can size those windows however they choose.

This means we should not rely on fixed numbers of columns and specific breakpoints. 

## Implementation

Elements provides a small set of components for common layout tasks. These are in the global directory and have the prefix `global-layout`.

Use our layout  components with the layout utility classes provided in the `brand-context` folder. This means less code and a less prescriptive approach that better adapts to various screen sizes. 

For example, `global-layout-grid` creates a basic grid layout of rows and columns. Each cell in the grid has the same width. The number of columns is determined by:

- the overall width of the grid, derived from the width of its container
- the basis for each cell

The basis is the ideal width of the cells. Set this using `--grid--basis`.  

The width shown on the screen will likely be smaller or larger than the `--grid--basis value`, as columns wrap and stretch to use the available space. The larger the `--grid--basis value`, the fewer columns that are possible.

Where multiple columns can fit in the available space, a grid emerges. Where they cannot, a simple single column layout takes its place.

## Page anatomy

All pages must have 3 regions:

- Header (including top level navigation)
- Main content area (including a page title)
- Footer (including a set of standard links for all our websites)

![Diagram highlighting the 3 main regions of a web page, the header, main content area and footer. These are show using rectangles to indicate the areas of the page. Text labels are used to show which area is which.](https://user-images.githubusercontent.com/120400118/218751209-8be7e21f-d4be-4b9a-b6ab-fdb5e2c63cf4.png)

## Common layouts

### Single column

This is the most basic layout. Use it for task or information focused content such as:

- log in pages
- error pages, for example a 404 error page
- step by step processes

![Diagram of a single column web page layout. A green dotted line indicates the overall page container. Rectangles represent where content may sit on the page.](https://user-images.githubusercontent.com/120400118/218752189-e4f5e925-4564-47d8-a0ff-94e41a16e808.png)


For single column layouts, use the utility `u-container` to set a maximum width. This is one of many class-based style utilities found in the `brand-context`.

The maximum width for the Springer Nature brand is 1080px. For the Springer and Nature brands it is 1248px. 

If the line length of text is too long inside its containing space, use the `ch` unit to set a more comfortable line length. [Go to the typography guidelines on line length](https://elements.springernature.com/springernature/styleguide/typography#line-length).

Use the [layout stack component](https://elements.springernature.com/springernature/components/global-layout-stack) to add vertical space between elements. For example, you can use it to add space between cards stacked on top of each other and also between the elements inside the card. 

![Diagram of a web page with various content elements represented by green rectangles. Orange blocks in between the elements show how the layout stack component will add vertical space between things.](https://user-images.githubusercontent.com/120400118/218753529-a2aca5f9-4115-4e5a-9087-baece71d9219.png)

Use the [layout cluster component](https://elements.springernature.com/springernature/components/global-layout-cluster) to add space between grouped inline elements such as buttons. Grouping elements closer together will help users to perceive them as related.

![Diagram of a web page with various content elements represented by green rectangles. Orange blocks show how the layout cluster component will add horizontal space between things in a group.](https://user-images.githubusercontent.com/120400118/218754382-07a465a4-26df-4e80-ad86-262257316094.png)

### Layout with sidebar

This is a 2 column layout where 1 column is smaller and sits on the side of a larger column, which takes up more horizontal space on a wide viewport. 

![Diagram of a web page with a sidebar layout. Green rectangles with dotted lines show the sidebar region taking up a third of the page on the left, and the main content area taking up the other two thirds on the left.](https://user-images.githubusercontent.com/120400118/218755255-ded2f959-b2f0-4898-823a-0af8c9d0e6a1.png)

Use this layout when you want to show some main content alongside supporting content or functionality, for example:

- navigational elements
- filters and sorting elements
- promoting related content or information that is relevant at that point

Use the [layout with sidebar component](https://elements.springernature.com/springernature/components/global-layout-with-sidebar) to enable a responsive layout without the use of media queries. 

The sidebar column can appear either before or after the main column. When the main column is less than or equal to 50% of the page container’s width, it will stack onto a new line and take up all the space.

![Diagram showing how the sidebar is responsive when using this component. Green blocks represent the main content, while orange blocks represent the sidebar. With the sidebar on the left, it moves to the top of a single column when the main content is less than or equal to half the width of the page container. When the same thing happens with the sidebar on the right, it stacks on the bottom.](https://user-images.githubusercontent.com/120400118/218755953-2211d4da-9955-4586-8bc3-7fea7abb36db.png)

### Grid layout

The grid layout enables multiple columns of the same width on wide viewports. Each column will stack according to the available space.

![Diagram showing a grid layout. Four cards are aligned next to each other, each taking up and equal amount of space.](https://user-images.githubusercontent.com/120400118/218756964-8d616bf5-fc08-4515-804e-40a340bca71b.png)

Use this layout when showcasing a variety of content teasers or onward journeys such as on homepages or landing pages. 

For example, cards that place an emphasis on imagery can act as a bridge to related content and services.

For scenarios where there is a long list of content, such as article lists, use a single column instead.

Use the [layout grid component](https://elements.springernature.com/springernature/components/global-layout-grid) to create responsive multi column layouts.

## Combining layouts

Use the components in combination to achieve the right layout for your users.

![Diagram showing the different layout components in use on the same page. Rectangles represent a sidebar layout with a green sidebar block on the left. Within the main content area, there is a single column layout with various content elements stacked on top of each other. This is represented by purple blocks. Underneath this, still within the main content area of the sidebar layout, is an orange area showing four cards in a grid layout.](https://user-images.githubusercontent.com/120400118/218757996-c43edfe9-3bb1-4320-b414-b52c03e33000.png)

## Resources

Apply the basic page template to your designs using the [Sketch style guide](https://www.sketch.com/s/fa9c2fc9-a179-43f0-b21e-9562c9c17c0c).

Our layout components are based on [Every Layout](https://every-layout.dev/).

## Help improve this page
If you’ve got a question, idea or suggestion about how to improve this component or guidance, post in the [#ask-elements](https://springernature.slack.com/archives/CNBTFLBLP) Slack channel .
