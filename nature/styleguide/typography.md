# Typography
 
## Font
 
Use Harding for headings and the main body text. 

Use Graphik for services that sit under the Nature Portfolio such as Nano.

Use system fonts or “native typography” for:

- elements that are interactive, such as buttons, forms and navigation links
- secondary information such as metadata, author names, publication dates and article summaries

## Headings

### Write headings in sentence case

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
