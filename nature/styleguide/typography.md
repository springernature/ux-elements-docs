# Typography

 <br />
 
## Font Families

 <br />
 
### Harding
We use our custom typeface, Harding as our primary font for headings and the main body text. Named after the late neurologist Anita Harding, it was designed specifically for science, with a large range of special characters for different subjects.

A key consideration in Harding’s overall design is performance on small digital screens. To boost readability in a limited space, it helps to enlarge the main portion of the lower-case letters, while making the ascenders and descenders (as in ‘h’ and ‘g’, respectively) smaller. Ultimately, this renders long, complex strings of words easier to parse, and allows for neat stacking of lengthy technical research-article titles over a number of lines.

Harding creates an overall impression of calm, rational intelligence with perhaps a dash of British formality and wit.

### Graphik
For services that sit under the Nature Portfolio such as Nano, we use Graphik as the primary font. Graphik is a clean and modern sans serif typeface that has a large family of varying weights.

### System fonts
We use system fonts or “native typography” for elements that are interactive, such as buttons, forms and navigation links. We also use it for secondary information such as meta data, author names, publication dates and article summaries.

Using system fonts ensure our websites can perform well on slow connection speeds, creating a more frictionless experience. Fonts native to the users’ OS, such as Apple’s SF Pro and Microsoft’s Segoe UI are also well optimised for legibility.

 <br />

## Usage

Use our font styles consistently by always making sure they reflect the information hierarchy on the page. If the hierarchy is clear, we ensure that our content is easily scannable for our audiences. Combining these font sizes and styles together with layouts designed for optimal reading experiences will foster familiarity for our users.

* In hero cards and headings, harding works best when character spacing and line height are tight
* Longer article text should use line height to maximise legibility
* Body text and paragraphs at base sizes should not exceed 800px in width
* We use fluid typography by applying properties for different screen sizes, "Max" and "Min" 

## Headings

## Write headings in sentence case

For example, “Latest reviews and analysis” not “Latest Reviews and Analysis”.

Sentence case is easier for people to read.

Headings should follow [our content guidelines](https://frontend-design-system.private.springernature.app/nature/content).

### Make headings meaningful

Use descriptive headings that convey the meaning of the section they refer to. This helps users scan and find the information they need, without having to read all of the content from top to bottom.
For example, “Publish with us” is clearer than “Information on submission”.

### Use heading levels to communicate page structure

Use semantic heading levels `<h1>` to `<h6>` to show the relationship of sections to subsections in the page structure.
Only include one `<h1>` per page, for the main heading.

Don’t skip heading levels. For example, don’t follow an `<h2>` with an `<h4>`. Doing this can be confusing, particularly for some assistive technology users.

Learn  more about how to use heading levels in the [W3 guide to headings](https://www.w3.org/WAI/tutorials/page-structure/headings/).

### Heading sizes

Here are the heading sizes we use for Nature Journals.

<table>
        <tr>
                <th>
                       Heading style 
                </th>
                <th>
                       Properties 
                </th>	
                <th>
                       Max 
                </th>
                <th>
                       Min
                </th>
        </tr>
        <tr>
                <td>
                       heading 1
                </td>
                <td>
                       font-size: <br />
                       font-weight: <br />
                       font-family: <br />
                       letter-spacing: <br />
                       line-height: <br />
                </td>
                <td>
                       32px <br />
                       bold <br />
                       harding <br />
                       -0.0625rem <br />
                       36px <br />
                </td>
                <td>
                       24px <br />
                       bold <br />
                       harding <br />
                       -0.01875rem <br />
                       26px <br />
                </td>
        </tr>	
        <tr>
                <td>
                       heading 2
                </td>
                <td>
                       font-size: <br />
                       font-weight: <br />
                       font-family: <br />
                       letter-spacing: <br />
                       line-height: <br />
                </td>
                <td>
                       24px <br />
                       bold <br />
                       harding <br />
                       -0.01875rem <br />
                       26px <br />
                </td>
                <td>
                       20px <br />
                       bold <br />
                       harding <br />
                       -0.01875 <br />
                       22px <br />
                </td>
        </tr>
        <tr>
                <td>
                       heading 3
                </td>
                <td>
                       font-size: <br />
                       font-weight: <br />
                       font-family: <br />
                       letter-spacing: <br />
                       line-height: <br />
                </td>
                <td>
                       20px <br />
                       bold <br />
                       harding <br />
                       -0.01875 <br />
                       22px <br />
                </td>
                <td>
                       20px <br />
                       bold <br />
                       harding <br />
                       -0.01875 <br />
                       22px <br />
                </td>
        </tr>	
</table>	

### Changing default heading sizes

Our typography styles determine the size of headings based on the heading level you apply. For example, an `<h1>` is the largest at 30px, followed by `<h2>` at `24px`, and so on.

If you need to use a different font size for a heading, you can use a utility class to override the default sizing. For example:

```
<h2 class="u-h3">Smaller h2 rendering</h2>
```

Do not change the semantic heading level purely to make the heading visually larger or smaller.
