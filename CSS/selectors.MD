# CSS: Selector
CSS sectors identify specific HTML elements as targets for CSS style. This topic covers how CSS selectors target HTML elements. Selectors use a wide range of over 50 selections methods offered by the CSS languagege, including elements, classes, IDs, preudo-elements and pseudo-classes, and patterns.
<br>
<br>

## Basic Selector
| Selector | Description | Example |
| --- | --- | --- |
| `*` | Universal Selector <br>Select all elements in a document. |  |
| `div` |  |  |
| `.` | Class Sector |  |
| `#` | ID Selector |  |
| `:` | Pseudo Class Selector |  |
| :: | Pseudo Element Selector |  |
| :lang() | Language Selector <br>Element that matches :lang declaration. | ` <span lang="en"> ` |
| > | Child Selector |  |
<br>

## Attribute Selector
| Selector | Matched Element | Description | CSS Version |
| --- | --- | --- | --- |
| `[attr]` | &lt;div attr=""&gt; | With attribute `attr` .| 2 |
| `[attr="val"]` | &lt;div attr="val"&gt; | Where attribute `attr` has value `val` . | 2 |
| `[attr~="val"]` | &lt;div attr="val val2 val3"&gt; | Where `val` appears in the whitespace-separated list of `attr` . | 2 |
| `[attr^="val"]` | &lt;div attr="val val2"&gt; | Where `attr`'s value `begins` with `val` . | 2 |
| `[attr$="val"]` | &lt;div attr="val val2"&gt; | Where the `attr`s value `ends` with `val` . | 2 |
| `[attr*="val"]` | &lt;div attr="somevalhere"&gt; | Where the `attr` contains `val` anywhere. | 2 |
| `[attr|="val"]` | &lt;div attr="somevalhere"&gt; | Where the `attr` contains `val` anywhere. | 2 |