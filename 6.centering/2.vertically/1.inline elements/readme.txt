Is it single line?
===================

Sometimes inline / text elements can appear vertically centered, just because there is equal padding above and below them.

padding-top: 30px;
padding-bottom: 30px;

If padding isn't an option for some reason, and you're trying to center some text that you know will not wrap, there is a trick were making the line-height equal to the height will center the text.

.center-text-trick {
  height: 100px;
  line-height: 100px;
  white-space: nowrap;
}


Is it multiple lines?
======================

Equal padding on top and bottom can give the centered effect for multiple lines of text too, but if that isn't going to work, perhaps the element the text is in can be a table cell, either literally or made to behave like one with CSS. The vertical-align property handles this, in this case, unlike what it normally does which is handle the alignment of elements aligned on a row. (More on that.)



If something table-like is out, perhaps you could use flexbox? A single flex-child can be made to center in a flex-parent pretty easily.

.flex-center-vertically {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 400px;
}