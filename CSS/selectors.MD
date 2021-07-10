# CSS: Selector
CSS sectors identify specific HTML elements as targets for CSS style. This topic covers how CSS selectors target HTML elements. Selectors use a wide range of over 50 selections methods offered by the CSS languagege, including elements, classes, IDs, preudo-elements and pseudo-classes, and patterns.
<br>
<br>

## &#8284; Basic Selector
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

## &#8284; Attribute Selector
| Selector | Matched Element | Description | CSS Version |
| --- | --- | --- | --- |
| `[attr]` | &lt;div attr=""&gt; | With attribute `attr` .| 2 |
| `[attr="val"]` | &lt;div attr="val"&gt; | Where attribute `attr` has value `val` . | 2 |
| `[attr~="val"]` | &lt;div attr="val val2 val3"&gt; | Where `val` appears in the whitespace-separated list of `attr` . | 2 |
| `[attr^="val"]` | &lt;div attr="val val2"&gt; | Where `attr`'s value `begins` with `val` . | 2 |
| `[attr$="val"]` | &lt;div attr="sth aval"&gt; | Where the `attr`s value `ends` with `val` . | 2 |
| `[attr*="val"]` | &lt;div attr="somevalhere"&gt; | Where the `attr` contains `val` anywhere. | 2 |
| [attr &vert;="val"] | &lt;div attr="val-sth etc"&gt; | Where `attr`s value is exactly  `val`, or start with `val` and immediatelly followed by - (U+002D). | 2 |
<br>

## &#8284; Combinators
| Selectors |  Description | |
| --- | --- | --- |
| div span | Descendant Selector <br>All &lt;span&gt; that are decendants of a  &lt;div&gt;. |  |
| div > span | Child Selector <br> All  &lt;span&gt; that are a direct child of a  &lt;div&gt;|  |
| div ~ span | General Sibling Selector <br> All  &lt;span&gt;'s that are siblings after an &lt;a&gt;. |  |
| a + span | Adjacent Sibling Selector <br> All  &lt;span&gt;'s that are immediately after an  &lt;a&gt;. |  |
<br>

## &#8284; Pseudo Classes
| Name |  Description |
| --- | --- | 
| `:active`| Applies to any element being activated (i.e. clicked) by the user.|
| `:any` | Allows you to build sets of related selectors by creating groups that the included items will match. This is an alternative to repeating an entire selector. |
| `:target` | Selects the current active `#news` element. <br> e.g. Clicked on a URL containing that anchor name. |
| `:checked` | Applies to `radio, checkbox, or option elements that are checked or toggled into an "on" state. |
| `:default` | Represents any user interface element  that is the default among a group of similar elements. |
| `:disabled` | Applies to any UI element which is in a disable state. |
| `:empty` | Applies to any element which has no children. |
| `:enabled` | Applies to any element which is in an enabled state. | 
| `:first` | Used in conjunction with the `@page` rule, this selects the first page in a printed document. |
| `:first-child` | Represnts any element that is the first child element of it's parent. | 
| `:forst-of-type` | Applies when an element is the first of the selected element type inside it's parent. This may or may  not be the first-child. |
| `:focus` | Applies to any element which has the user's focus. This can be given by the user's keyboard, mouse events, or other forms of input. | 
| `:focus-within` | Can be used to highlight a whole section wehen one element inside it is focused. It mathches any element that the `:focus` preudo-calss mathches or that has a descendant focused. |
| `:hover` | Applies to any element being hovered by the user's pointing device, but not activated. |
| `:indeterminate` | Applies radio or checkbox UI elements which are neither checked  nor unchecked, but are in an indeterminate state. This can be due to an element's attribute or DOM manipulation. |
| `:in-range`| The `:in-range` CSS pseudo-class matches when an element has it's value attribute inside the specified range limitations for this element. It allows the page to give a feedback that the value currently defined using the element is indside the range limits.  |
| `:invalid` | Applies to &lt;input&gt; elements whose values are invalid accroding to the type specified in the `type=` attribute. |
| `:lan` | Applies to any element who's wrapping &lt;body&gt; element has a properly designated `lang=` attribute. For the pseudo-calss to be valid, it must containt a a valid two or three letter language code. |
| `:last-child` | Represents any element that is the last child element of it's parent. |
| `:last-of-type` | Applies when an element is the last of the selected element type inside it's parent. This may or may not be the `last-child`. |
| `:left` | Used in conjunction with the `@page` rule, this selects all the left pages in a printed document. |
| `:link` | Applied to any link which haven't been visited by the user. |
| `:not()` | Applies to all elemnts which **do not** match the value passed to (`:not(p)` or `:not(.class-name)`) for example. It must have a value to be valid and it can onlu contain one selector. However, you can chain multiple `:not` selectors together. |
| `:nth-child` | Applies when an element is the n-th element of it's parent, ehre `n` can be an integer, a mathmatical expression (e.g `n+3`) or the keywords add or even. |
|`:nth-of-type` | Applies when an element is the n-th element if it's parent of the same element type, where `n` can be an integer, a mathmatical expression (e.g `n+3`) or the keywords odd or even. |
| `:only-child` | The `:only-child` CSS pseudo-class represents any element which is the only chid of it's parent. This is the same as `:first-child:last-child` or `:nth-child(1):nth-last-child(1)`, with a lower specificity.|
| `:optional` | The `:only-child` CSS pseduo-class represents anyy element that does not have the required attribute set on it. This allows forms to easily indicate optional fields and to style them accordingly. |
| `:out-of-range` | The `:out-of-range` CSS pseudo-class matches when an element has it's value attribute outside the specified range limitations for this element. It allows the page to give a feedback that the value currently defined using the  element is outside the range limits. A value can be outside of a range if it is either smaller or larger than maximum and minimum set values. | 
| `:placeholder-shown` | Experimental. Applies to any form element currently displaying placeholder text. |
| `:read-only` | Applies to any element which is not editable by the user. |
| `:read-write` | Applies to any element that is editable by a user, such as &lt;input&gt; elements. |
| `:right` | Used in conjunction with the `@page` rule, this selects all the right pages in a printed document. | 
| `:root` | Matches the root element of a tree representing the document. |
| `:scope` | CSS pseudo-class matches the elements that are a reference point for selectors to match against. |
| `:target` | Selects the current active #news element (clicked on a URL containing that anchor name) | 
| `:visited` | Applies to any links which have has been visited by the user. |
<br>

## &#8284; Child Pseudo Classes
---
| Pseudo-selector | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| `:first-child`  | &check; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash;| &dash; |
| `:nth-child(3)`  | &dash; | &dash; | &check; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; |
| `:nth-child(n+3)`  | &dash; | &dash; | &check; | &check; | &check; | &dash; | &check; | &check; | &check; | &check; |
| `:nth-child(3n)`  | &dash; | &dash; | &check; | &dash; | &dash; | &check; | &dash; | &dash; | &check; | &dash; |
| `:nth-child(3n+1)` | &check; |&dash;  | &dash; | &check; | &dash; | &dash; | &check; | &dash; | &dash; | &check; |
| `:nth-child(-n+3)` | &check; | &check; | &check; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; |
| `:nth-child(odd) ` | &check; | &dash; | &check; |  | &check; | &dash; | &check; | &dash; | &check; | &dash; |
| `:nth-child(even)` | &dash; | &check; | &dash; | &check; | &dash; | &check; | &dash; | &check; |  | &check; |
| `:last-child` | &dash; | &dash; |&dash;  | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; | &check; |
| `:nth-last-child(3) ` | &dash; | &dash; | &dash; | &dash; | &dash; | &dash; |&dash;  | &dash; | &check; | &dash; |
<br>

<br>
<br>
<br>
<br>
<br>
<br>

> <p style="text-align: center;">I'm still working on this project.</p>
> <p style="text-align: center;">For any change or update please contact me at abut1081@gmail.com .</p>