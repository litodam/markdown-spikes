# Authoring Guidance for Markdown #
 
This guide describe the typical styles used in DPE content.  
If you're not already familiar with Markdown, you should spend 15 minutes and go over the excellent Markdown Syntax Guide at Daring Fireball.

## Document section headings ##
Topic titles like Overview and Exercises use a first and second level heading.  
In Markdown heading 1 can be written in the following ways (being the first one the suggested syntax):

	# Overview #
	OR:
	# Overview
	OR:
	Overview
	========
		
Output:
# Overview #

Heading 2 also has different forms (being the first one the suggested syntax):

	## Instructions ##
	OR:
	## Instructions
	OR:
	Instructions
	-----------

Output:
## Instructions ##

Other sections like Tasks or other subsections uses lower level headings.
Examples:

	### This is an h3 title ###
	#### This is an h4 topic ####

Output:
### This is an h3 title ###
#### This is an h4 topic ####


## Bold ##
In Markdown bold text can be specified in the following ways (being the first one the suggested syntax):
Example:

	**bold text**
	OR:
	__bold text__
	
	
Output:

**bold text**


## Italics ##
In Markdown, text in italics can be specified in the following ways (being the first one the suggested syntax):
Example:

	_italics text_
	OR:
	*italics text*
	
	
Output:

_italics text_
	

## Strikethrough ##
In Markdown, strikethrough text is not supported out of the box but there are several engines that support an extension using the following syntax:
Example:

	~~strikethrough text~~
	
	
Output:

~~strikethrough text~~


## Ordered Lists ##
Use ordered list for the detailed instructions to accomplish tasks. 

To simplify the authoring experience it is recommended to use "1." for every item in the list. The engine will take care of the proper numbering. 
Example:

	1. Open Visual Studio
	1. Go to File -> New Project
		1. Select C# language
		1. Choose WPF Project template
		1. Enter HelloWorld as project name
	1. Click Ok

Output:

1. Open Visual Studio
1. Go to File -> New Project
	1. Select C# language
	1. Choose WPF Project template
	1. Enter HelloWorld as project name
1. Click Ok

## Unordered lists ##
Unordered lists are used to enumerate things. In Markdown item lists can be written in the following ways (being the first one the suggested syntax):
Example:

	- Item 1
	- Item 2
	OR:
	+ Item 1
	+ Item 2
	OR:
	* Item 1
	* Item 2
	
Output:

- Item 1
- Item 2
- Item 3

## Code Snippets ##
In standard markdown, inline code is written between backticks (`)

Some text with `some code` inside,

Or indent several lines of code by at least four spaces:

    line 1 of code
    line 2 of code
    line 3 of code

For Lab and Tutorial Authoring, the Sugested approach is the github flavour which allows you to set the code language in the first line of the snippet:


	```` C#
		public void foo()
	    {
	    	    int a;
		    a = 1;
		    a ++;
	    }
    ````

And the Output:

````C#
	public void foo()
	{
		int a;
		a = 1;
		a ++;
	}
````


## Notes ##

	> **Note:** Make sure you have checked all the dependencies for this lab before running the setup.

And the output:

> **Note:** Make sure you have checked all the dependencies for this lab before running the setup.


## Images ##
Images are added with the following code:

	![alt text here](./images/myimage.png "title image here")

Output:

![Alt Text](./images/myimage.png "Image Title")


## Tables ##

In Markdown, tables are not supported out of the box but there are several engines that support an extension using the following syntax:
Example:
	
	| **ColHeader1** | **ColHeader2** |
	|----------------|----------------|
	| Field1         | Field2         |
	| Field3         | Field4         |
	| Field5         | Field6         |
	
	
Output:

| **ColHeader1** | **ColHeader2** |
|----------------|----------------|
| Field1         | Field2         |
| Field3         | Field4         |
| Field5         | Field6         |



