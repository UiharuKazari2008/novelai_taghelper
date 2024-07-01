# NovelAI Tag Helper Plus

This is a simple in-browser utility designed for support AI art prompt building/organization in [NovelAI](https://novelai.net/image).

You may access it [here](https://uiharukazari2008.github.io/novelai_taghelper/).

## Usage
Add tags using either the textfield or the `+` button. Tags can be edited by double-clicking and moved around with drag and drop. Once you have finished organizing your taglist, the full prompt can then be copied to the clipboard through the `<>` button.

## Additions
- Rewrite of a lot of functions
- Realistic icons that depict what the function is
- Added Delete button to delete a tag from the list
- Tag group storage
  - Load preset queries into the workspace
  - Check the box to include the tags in your copied results
    - There hidden from your workspace to keep things simple
- Handles encapsulated groups correctly
- `CTRL+D` replaces `CTRL+C`
- `CTRL+I`: Adds clipboard to tag list (Deduplicate Input against workspace and enabled items)
- `CTRL+SHIFT+I`: Replaces tag list from clipboard

### ToDo List
- Dark Mode
- StableDiffustion Tag system mode
- Saving groups of tags
- Saving taglist as a preset

## Controls and Features

 - `+` (at the top menu): Appends a new tag to the bottom of the list. This tag can then be renamed by double-clicking the tag item.
 - Mouse drag-and-drop: Reorders the selected tag to the mouse position. Users may also delete tags by spilling (dragging tags outside the taglist area).
 - `x`: Clears all tags from the taglist.
 - `↓`: Saves current tags to local storage (persists taglist on page reload).
 - `<>`: Copies current taglist (ordered) to the clipboard. The output separates each tag is separated by `,` (comma) and replaces `_` (underscore) danbooru-style tag notation to ` ` (whitespace) characters.
 - `+` (at taglist): Raises tag priority -- encloses the tag with `{}` each time it is clicked. If the tag is enclosed by `[]`, it removes one pair of the square brackets instead.
 - `—`: Lowers tag priority -- encloses the tag with `[]` each time it is clicked. If the tag is enclosed by `{}`, it remove one pair of the curly brackets instead.
  - `Hide/unhide`: Tags that are hidden will not be included in the clipboard export.
