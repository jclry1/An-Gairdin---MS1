This is for notes and resources grabbed along the way influencing decision or providing code examples etc.

Navbar:
https://getbootstrap.com/docs/4.0/components/navbar/
https://medium.com/coder-grrl/the-guide-to-customising-the-bootstrap-4-navbar-i-wish-id-had-6-months-ago-7bc6ce0e3c71
https://www.w3schools.com/bootstrap4/bootstrap_navbar.asp

required jquery, popper etc to enable functinoality ov navbar taken from:
https://getbootstrap.com/docs/4.3/getting-started/introduction/

Nav alignmnet:
Initial design was to have the hamburger button on the right, but after considering how it expands on the left, I would prefer to keep it positioned above where it will expand - so aligning top left.

Image compression for faster loading, less data usage:
https://tinyjpg.com/

Fixed bottom:
https://getbootstrap.com/docs/4.1/utilities/position/

Really troublesome issue with container-fluid introducing nwanted margin on right side at sm screen sizes. Finally resolved with:
.container-fluid{
    overflow-x: hidden;
}
Source:
https://stackoverflow.com/questions/25427407/bootstrap-3-and-4-container-fluid-with-grid-adding-unwanted-padding

Issue with getting the main content area to stretch vertically to fill the available space. Fixed with adding vh-100 to all parents:
https://stackoverflow.com/questions/30469177/make-bootstrap-column-touch-the-bottom-of-the-div/30480004#30480004

Responsive breakpoint for footer - sizing icons, col-layout:
https://getbootstrap.com/docs/4.1/layout/overview/

Accessibility: When to add "aria-hidden=true" for icons
https://fontawesome.com/how-to-use/on-the-web/other-topics/accessibility

Fixed header overlaying content issue - fixed by adding padding to the body:
https://stackoverflow.com/questions/10336194/top-nav-bar-blocking-top-content-of-the-page

Information and layout practice for using bootstrap card-decks:
https://getbootstrap.com/docs/4.0/components/card/
https://www.w3schools.com/bootstrap4/bootstrap_cards.asp

About Page:
about.html based on garden.html (cp garden.html about.html)


### Bootstrap card deck issues

Problems getting the footers in the boostrap cards (card-deck) to align. Tried several options from stackoverflow and elsewhere but none seemed to work. Best solution I've found so far was this:
In the card-body div (Bootstrap) add a new div below the title to contain the paragraph content. Call this .card-content. Set the parent card-body to be:
.card-body{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}
On the new child div, apply: 
.card-content{
  align-self: stretch;
  height: 100%;
}

It seems to need both the stretch and 100% to work. 

That pushes the footer to the end of th card. However, if the footers have differeing amount of content, they now push up to different heights at the bottom of the card. resolve this with a fixed-height footer to allow space for 3 lines of small text.

Info for this solution derived from: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container

### Placeholder text color - form textarea
Issue resolved using code and info from here: https://medium.com/@samanthaming/styling-placeholder-text-with-css-9a2a608b68bc


### Circle with text on index.html (welcome-mat)
Circle based on learning in the LoveRunning mini-project
Alignment using flex + margin/padding: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container

### Change card footers to blockquotes for more semantic mark-up and fix display issues
https://stackoverflow.com/questions/2205159/correct-use-of-blockquote-q-and-cite#:~:text=Yes.,%2C%20standard%2C%20URL%2C%20etc.&text=The%20blockquote%20element%20(also%20the,where%20the%20quote%20came%20from.
https://www.w3schools.com/tags/tag_blockquote.asp

### Put copyright info into 'small' element for semantic markup
https://stackoverflow.com/questions/5876021/correct-semantic-tag-for-copyright-info-html5

### Issue with header nav breaking at intermediate screen size
The issue here was that the header was expanding in vertical height when the menu was expanded at md size (to accommodate the icons and text being split onto separate lines). The effect of this was to disrupt the appearance of the logo on the right.
Solution has been to delay the menu-expand until the lg screen size.

## Wishlist

### Underline active nav 

### Style social media icons to have header color on hover - done

### Different widths for contact form based on screen sizes
90% is good for mobile butseems a bit too wide for desktop


