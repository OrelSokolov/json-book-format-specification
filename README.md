# JSON BOOK FORMAT DESCRIPTION

Entire document object contains:
*	Content array
    *	Content chunk 
        *	Font number
        *	Font size
        *	Font color
        *	Align type
        *	Content, of course
        *	Background color
        *	Role
            *	Default
            *	Header class
    *	Special chunk (tab, line break)
        *	Background color
    *	Special characters and formulas
    *	Table
        *	Table content
            *	Element
                *	Content
                *	Attributes
                    *	Border left
                    *	Border right
                    *	Border top
                    *	Border bottom
                    *	Background color
                    *	Align method
             *	Table name
                  *	Name
                  *	Number presence flag
*	Pages array
    *	Page
        *	Number
        *	Page class
        *	Default font size
        *	Images attached to page
            *	Image
                *	Position X
                *	Position Y
                *	Position Z
                *	Width
                *	Height
                *	Opacity
                *	Rotation degree
        *	Lines – automatically generated from text chunks
            *	Line
                *	Array of chunks
                *	Line height
*	Page classes array
    *	Class
        *	Number
        *	Name
        *	Background color
        *	Width
        *	Height
        *	Orientation
        *   Padding array [top, right, bottom, left] (does not depend of orientation)
*	Table classes array ( describes how rows and columns should be colored, just rules )
*	Fonts array
    *	Font
        *	Number 
        *	Name
        *	Source
*	Images array
    *	Image
        *	Description
        *	Base64 encoded content
*	Metadata
    *	Author
        *	Name
        *	Email
        *	Signature
*	Document
    *	Defaults
        *	Font number
        *	Font size
    *	Last edit date
    *	Creation date
    *	License 


## Some notes

Page attributes are copied from previous page if nothing else selected

### Cursor position
Page has text – after some symbol
Page has no text – where to insert new symbol

Page devided to pagelines
Pageline object – object, attached to page
It hast lineheight, line height is max font size height



