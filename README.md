# A first-level heading
## A second-level heading
### A third-level heading
#### A forth-level heading
##### A fifth-level heading
###### a sixth-level heading


**STYLING TEXTS:**

You can indicate emphasis with bold, italic, strikethrough, subscript, or superscript text in comment fields and .md files.

Style	Syntax	Keyboard shortcut	Example	Output

Bold	** ** or __ __	Command+B (Mac) or Ctrl+B (Windows/Linux)	
**This is bold text**	
This is bold text

Italic	* * or _ _     	Command+I (Mac) or Ctrl+I (Windows/Linux)	
_This text is italicized_	
This text is italicized

Strikethrough	~~ ~~	None	
~~This was mistaken text~~	
This was mistaken text

Bold and nested italic	** ** and _ _	None	
**This text is _extremely_ important**	
This text is extremely important

All bold and italic	*** ***	None	
***All this text is important***	
All this text is important

Subscript	<sub> </sub>	None	
This is a <sub>subscript</sub> text	
This is a subscript text

Superscript	<sup> </sup>	None	
This is a <sup>superscript</sup> text	
This is a superscript text


Text that is not a quote

> Text that is a quote


**QUOTING CODE:**

You can call out code or a command within a sentence with single backticks. 
The text within the backticks will not be formatted. 
You can also press the Command+E (Mac) or Ctrl+E (Windows/Linux) keyboard shortcut to insert the backticks for a code block within a line of Markdown.


Use `git status` to list all new or modified files that haven't yet been committed.


To format code or text into its own distinct block, use triple backticks.

Some basic Git commands are:
```
git status
git add
git commit
```


In issues, pull requests, and discussions, you can call out colors within a sentence by using backticks. 
A supported color model within backticks will display a visualization of the color.

The background color is `#ffffff` for light mode and `#000000` for dark mode.


**LINKS:**

You can create an inline link by wrapping link text in brackets [ ], and then wrapping the URL in parentheses ( ). 
You can also use the keyboard shortcut Command+K to create a link. 
When you have text selected, you can paste a URL from your clipboard to automatically create a link from the selection.

You can also create a Markdown hyperlink by highlighting the text and using the keyboard shortcut Command+V. 
If you'd like to replace the text with the link, use the keyboard shortcut Command+Shift+V.

This site was built using [GitHub Pages](https://pages.github.com/).


**RELATIVE LINKS:**

You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. 
For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

[Contribution guidelines for this project](docs/CONTRIBUTING.md)
GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. The path of the link will be relative to the current file. Links starting with / will be relative to the repository root. 
You can use all relative link operands, such as ./ and ../.

Relative links are easier for users who clone your repository. 
Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.



**IMAGES:**

You can display an image by adding ! and wrapping the alt text in [ ]. 
Alt text is a short text equivalent of the information in the image. 
Then, wrap the link for the image in parentheses ().

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)


Context	Relative Link
In a .md file on the same branch	/assets/images/electrocat.png
In a .md file on another branch	/../main/assets/images/electrocat.png
In issues, pull requests and comments of the repository	../blob/main/assets/images/electrocat.png?raw=true
In a .md file in another repository	/../../../../github/docs/blob/main/assets/images/electrocat.png
In issues, pull requests and comments of another repository	../../../github/docs/blob/main/assets/images/electrocat.png?raw=true


**SPECIFIYING THE THEME A PICTURE IS SHOWN TO:**

You can specify the theme an image is displayed for in Markdown by using the HTML <picture> element in combination with the prefers-color-scheme media feature. 
We distinguish between light and dark color modes, so there are two options available. 
You can use these options to display images optimized for dark or light backgrounds. This is particularly helpful for transparent PNG images.

For example, the following code displays a sun image for light themes and a moon for dark themes:

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>


**LISTS:**

You can make an unordered list by preceding one or more lines of text with -, *, or +.

- George Washington
* John Adams
+ Thomas Jefferson


  To order your list, precede each line with a number.

1. James Madison
1. James Monroe
1. John Quincy Adams


**NESTED LISTS:**

You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Visual Studio Code, you can align your list visually. 
Type space characters in front of your nested list item until the list marker character (- or *) lies directly below the first character of the text in the item above it.

1. First list item
   - First nested list item
     - Second nested list item
    

To create a nested list in the comment editor on GitHub, which doesn't use a monospaced font, you can look at the list item immediately above the nested list and count the number of characters that appear before the content of the item. Then type that number of space characters in front of the nested list item.

In this example, you could add a nested list item under the list item 100. First list item by indenting the nested list item a minimum of five spaces, since there are five characters (100 .) before First list item.

100. First list item
     - First nested list item
    

