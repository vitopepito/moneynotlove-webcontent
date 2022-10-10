---
title: Cheatsheet
menu: Cheatsheet
---

##### A guide to markdown and how things are done with the custom 'money' theme for the site moneynotlove.ch running on Grav CMS. Reading this should make it easy for anyone to edit the pages of our website. For other instructions, see the [Documentation](/documentation). {.banner .text-soft}

---

### Titles

There are six levels of titles, corresponding to the six html `<h>` tags.

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

### Just body copy

Paragraphs are the easiest, since they do not require any special code. However, a line-break will only be added if there is a blank line in between two paragraphs. Text formatting can be applied, _italics_, __bold__ and ~~strikethrough~~.

Like so.
Not so.

If you need additional line-break, add `<br />`.

<br />



### Lists

Making list is also very easy, just precede each line with a line.
- First line
- Second line
- Third line

1. also
2. ordered
3. lists

### Links

Links can be added inside copy, for example to our [round-table](/round-table) or and [external site](https://getgrav.org).

### Images

Images are added in a similar manner to links, like so ![logo](/images/logo.png?resize=200,200). If you are using the grav admin panel, it is possible to just drag-and-drop images into the editor. Grav also provides many more functions and filters for images, [documented here](https://learn.getgrav.org/content/media)

### Code

    You can highlight text by indenting it with four spaces. Can be used for code or anything else. All character appear as-is.


### Some special code

In our theme, there is a little bit of special code for certain formatting. We use [markdown extra](https://michelf.ca/projects/php-markdown/extra/) syntax for that. This works for the following elements:
- headers (titles)
- links
- images

<br />

###### Make text coloured. {.text-soft}

###### In two variants.  {.text-hard}

###### Created a banner with any content you like. It will add spacing above and below and center the text. {.banner}

# A first level heading with colour! {.banner .text-soft}

    ---
    ##### A guide to markdown and how things are done with the custom 'money' theme for the site moneynotlove.ch running on Grav CMS. Reading this should make it easy for anyone to edit the pages of our website. For other instructions, see the [Documentation](/documentation). {.banner .text-soft}

    ---

    ### Titles

    There are six levels of titles, corresponding to the six html `<h>` tags.

    # Heading 1
    ## Heading 2
    ### Heading 3
    #### Heading 4
    ##### Heading 5
    ###### Heading 6

    ### Just body copy

    Paragraphs are the easiest, since they do not require any special code. However, a line-break will only be added if there is a blank line in between two paragraphs. Text formatting can be applied, _italics_, __bold__ and ~~strikethrough~~.

    Like so.
    But not so.

    If you need additional line-break, add `<br />`.

    <br />



    ### Lists

    Making list is also very easy, just precede each line with a line.
    - First line
    - Second line
    - Third line

    1. also
    2. ordered
    3. lists

    ### Links

    Links can be added inside copy, for example to our [round-table](/round-table) or and [external site](https://getgrav.org).

    ### Images

    Images are added in a similar manner to links, like so ![logo](/images/logo.png?resize=200,200). If you are using the grav admin panel, it is possible to just drag-and-drop images into the editor. Grav also provides many more functions and filters for images, [documented here](https://learn.getgrav.org/content/media)

    ### Code

        You can highlight text by indenting it with four spaces. Can be used for code or anything else. All character appear as-is.


    ### Some special code

    In our theme, there is a little bit of special code for certain formatting. We use [markdown extra](https://michelf.ca/projects/php-markdown/extra/) syntax for that. This works for the following elements:
    - headers (titles)
    - links
    - images

    <br />

    ###### Make text coloured. {.text-soft}

    ###### In two variants.  {.text-hard}

    ###### Created a banner with any content you like. It will add spacing above and below and center the text. {.banner}

    # A first level heading with colour! {.banner .text-soft}

    ---
