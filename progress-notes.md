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