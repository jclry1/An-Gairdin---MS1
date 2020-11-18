# An Gáirdín
An Gáirdín is an ecology and education center located in Portumna, Co Galway, Ireland.

The organisation runs a small organic market garden and orchard and also has a dedicated educational space for running courses and workshops. These range from spirituality to organic gardening to plastic pollution and climate change.

[View website in GitHub Pages](https://workingedge.github.io/An-Gairdin---MS1/)

### Site Purpose 
An Gairdin has an [existing Wordpress](https://www.angairdin.ie) site but it is infrequently updated and the lack of design (the site is a simple Wordpress template) means it comes across as distant, clinical, and superficial. The aim of this redesign is to create a more welcoming online space for people interested in the project to get a sense of what it is about, the values it strives to uphold, and the activities that go on there. The target audience includes a demographic that may not necessarily be very tech-savvy. With this in mind, the site should present simple, consistent navigation and contact options. Links to any external sites should be clearly accessible on all pages.

## UX
The site design aims to provide a simple and inviting space, encouraging further interaction with the project either online or in person.
A brief history of the project should be included as well as information on the main activities.
A contact option should be available and this should be straighforward and non-intimidating.

## Target audience
The primary audience for the website is local to the area (within 100 km) and encompasses regular visitors who may wish to get in contact or see updates, and new visitors who may become supporters. 

### User Stories
* As a visitor familiar with the project, I want to be able to easily get in touch with a comment or question.
* As a new visitor unfamiliar with the project I want to see a visually appealing introduction to the aims and activites undertaken and be able to easily join a mailing list or otherwise get in touch.
* As a local food enthusiast, I want to see information about the garden produce and see where this is sold locally.
* As a like-minded educator, I want to see some background information on the project and then easily get in touch with collaboration ideas using a contact form.
* As an older user or a user less-accustomed to online interation, I want to see an inviting and easy to navigate space that makes me feel at ease and is in line with my experience of the physical space.

* As a site-owner, I want to have an interenet presence that employs a look and feel in line with our aims, practices and goals. The site should mirror the atmosphere we endeavour to achieve in the physical location. 
* As a site-owner, I want site visitors to easily be able to get in touch with a question or comment, or to ask to be added to the mailing list.
* As a site-owner, I want any contact initiated on the website to go directly to my mail inbox. (nice to have, not a requirement for MS-1).
* As a site-owner, I want a visitor to be able to quickly jump to our social-media presence (facebook) where we have more up-to-date info.

### Wireframe Mockups
[Wireframe mockups](assets/docs/wireframe_v1.pdf) were developed before any coding took place and aim to give an outline of the final layout and flow of the site.

The initial version of the wireframe was largely adhered to but there were some changes as the design was built, including:
* Plan to have an image carousel is pending the delivery of images of sufficient quality
* Plan to have navigation buttons on the home page was discarded as they looked cluttered and detracted from the look of the page. The hamburger icon is used on smaller screens and the navigation menu opens across the fixed top and larger scren sizes. Instead of navigation buttons, the landing page shows the entrance to the physical space and includes a message clearly identifying the underlying ethos of the organisation.
* Plan for an image carousel was replaced with the use of Bootstrap card decks with image caps. These provide context to the card text and provide sufficient graphic interest on each of the pages.  

### Color Palette
The color palette used in the site aims to mirror the changing colours of the seasons in a garden and to be at the same time warm, vibrant and inviting. Ideas in relation to colour have been gleaned from general reading. 
Two useful resources have been [elementor](https://elementor.com/blog/color-theory-web-design/?gclid=Cj0KCQjwreT8BRDTARIsAJLI0KKeRi1NNrRWesVXyhOmyfNpwLFH8CCWWnFQ6Ael53UB6eYECiUufkAaAmKeEALw_wcB) and [coolors] (https://coolors.co/f94144-f3722c-f8961e-f9c74f-90be6d-43aa8b-577590).
Color selection on the site is guided by the palette described in the [draft color scheme](assets/color/draft-color-scheme.pdf).

There are two main colours used across the site:
#f9c74f:
* header
* top border on blockquotes
* border of input fields on the contact form
* border and text (pending contrasat check) of the welcome circle on home page
* social links - hover

#438397 and variant rgba(67, 131, 151, 0.9)
* footer
* background of the welcome message on home page
* background of the form area

Additional colours complementing the above are:
* #fef8e9 - background colour on all pages (except index.html)
* #215445 - heading (h2, h5) on about and garden pages
* #fafafa - text in footer and contact form, social icons (no hover) in footer
* #193f34 - text (logo and nav items) in header
* #873408 - text: hover (logo and nav items) in the header

For information on some color changes due to accessibility testing see testing.

## Features

### Navigation bar 
The site has a navigation bar integrated into the header. This is consistent across the top of all pages (fixed/no-scroll) of the site and therefore easily learnable for users. It is also a very familiar pattern internet-wide and should present little or no difficulties for users. 
On small screen sizes the navigation is collapsed and can be expanded by clicking the hamburger icon. On larger screens, the navigation is expanded by default. 
The text logo on the right side of the header is also present on all pages and serves as a link back to the home page.
All links in the header are styled consistent with the site color scheme and have styling on hover.

**logo**
The project logo (text) is presented in the header on all pages.

### Footer 
Each page has a standard footer with copyright info (left) and social media links (right). In reality, this project has a presence on facebook only. For the purposes of the MS1 project, dummy links to social media sites are (facebook, twitter, vimeo).
Copyright information is consistently displayed in the page footer (left).

Social media links are styled on hover and change color consistently with the site pallette.

### Home Page

The home page (index.html) features a real sense of the physical space occupied by this project. The colors of the image and the site header echo each other, as do the site footer and the background of the welcome/mission text. The home page clearly sets the tone for the whole site - inviting to visitors and clear in its values.
The background image (of an entranceway) also echoes the purpose of the home page.

### About
The About page uses a Bootstrap card deck to present the history of the project.
The text content is broken into three sections to improve the visual appearance and add other points of interest - each text block is enhanced with a top image and a quote that reinforces the purpose and the influences that drive the project. For the purposes of semantic HTML, the quotes are <blockquote> and all inclue a cite attribute. The quotes are set off from the text with a top border echoing the site's header colour. The quotes replace the standard Bootstrap <card-footer> element.
Text and quotes have been allocated to cards to achieve a well-balanced and consistent (aligned) layout. 

### Garden
The Garden page has two sections: Produce and Process
The layout of each mirrors the layout of the about page and again each text block is enhanced with an appropriate image and blockquote. All images (all pages) have the alt attribute filled.

### Contact
The Contact page features a **contact form**
The contact form allows for a simple message and the option to subscribe to the project's mailing list. The text area limits input to 400 characters.
(Note: To make the form actually work is outside the scope of this MS1 project).
Styling of the contact form is consistent with the other pages of the site. For example, the hover color of input area borders align with the site header. The background aligns with the background of the welcome message onthe home page.

The bottom of the form contains a **Send Button**
The send button text is customised to maintain the welcoming feel of the project and the colour (incl hover) is also customised to align with the overall look and fel of the site. 
 
### Features to Implement in Future
Based on the exisitng design, here are what I feel are the most warranted additions in the short term:
* Make the contact form function
* Add a page with more visual content - photos and video
* Include a section that updates on a regular basis without input from the site owners - for example a twiiter feed or RSS. This could inlcude content from other sites with a similar purpose, or to provide information on aspects of the site that visitors may be interested in  - for example organic food news, climate change updates etc.

## Technologies Used

#### HTML
The site is built using HTML and uses semantic markup - for example blockquote with cite attribute and small element for copyright info.

#### CSS
Styling is achieved using CSS and aims to achieve a consistent look and fel across all pages. Media queries are used to maintain the desired performance at all screen resolutions - for example to shrink social media icons at very small screen sizes.

#### Bootstrap 4
The Bootsrap 4 framework is used to achieve the layout of content on teh about.html and garden.html pages. Custom CSS is added to achieve correct padding and alignment for text and blockquote elements withn the cards.

#### Gitpod
The Gitpod IDE is used for all development.

#### GitHub
GitHub is used to store the site repository.

#### Git 
Version control is achieved using Git.

## Additional Resources
#### Tiny JPG
[TinyJPG](https://tinyjpg.com/) is used to compress all images before being uploaded to the GitHub repository.

#### Coolors
[Coolors](https://coolors.co/) is used to generate a consistent and aligned color scheme.
 
#### Autoprefixer
[Autoprefixer](https://autoprefixer.github.io/) is used to add vendor prefixes in teh CSS file.

#### Responsinator
[Responsinator](https://www.responsinator.com/) is used to check the appearance of the published site on different devices.

## Testing
The site and the source code have both undergone testing. Issues found and the actions taken to resolve the issues are described below.

### Testing issues - resolutions
#### CSS
https://jigsaw.w3.org/css-validator/
CSS tested at several points during development. Issues such as a ':' in place of a ';' or a missing '}' were found.
These have been fixed and the CSS run through auto-prefixer - no issues found.
As of 18/11/2020 - no CSS errors.

#### HTML
HTML was checked using 
##### aria-controls
The W3C HTML checker shows an error that the aria-controls attribute is not pointing to an element in the same document. 
This is the recommended checker for ARIA: https://w3c.github.io/using-aria/#validation
Issue was reolved by removing the hash '#' before the ID, in contrast to the data-target attribute (which has the # for ID).

##### type attribute for <textarea>
The checker showed an error where I had included "type=text" for the textarea in the contact form.
After checking https://www.w3schools.com/tags/tag_textarea.asp and https://www.w3schools.com/tags/att_input_type.asp - I have verified this is an incorrect use of the type attribute and have therefore removed it.
Tested for any impact on functionality of the textarea - none.

### Test mobility
https://search.google.com/test/mobile-friendly
Tested 17 Novemeber, 2020
Result: Page is mobile friendly

### Test contrast
https://color.a11y.com/


### Test performance
https://www.webpagetest.org/

### Test cross-browser
https://app.crossbrowsertesting.com/public/i04a6e9c0e8a8600/screenshots/z2aa92594c65a69493d6
Action item from this test was to include rel="noopener" or rel="noreferrer" to external links
Resource: https://web.dev/external-anchors-use-rel-noopener/


### Test on actual devices
Chrome and Firefox on Linux
Edge and IE on Windows
Chrome and Safari on Mac
Chrome and DuckDuckGo on Android
Safari on iPad
Safari on iOS


## Deployment
The site is deployed using GitHub Pages. 

#### Deployment Steps
1. 

### How to run this project locally

## Credits
All images and text are copyright An Gairdin.

### Content
All text and image content is courtesy of An Gairdin. Quotes are copyright their authors as attributed in the text.

### Code
Code is my own but is based on the course mini-projects and on various online resources, documentation and tutorials, as follows:


## Acknowledgements
For initial general guidance on the development of the MS-1 project and the README, the following pages were very helpful:
[Jim Lynx](https://github.com/JimLynx/CI-MS1-Explore-Ireland)
[A Greaves](https://github.com/AJGreaves/portrait-artist)
[ByIlsa](https://github.com/byIlsa/Aloy-from-outcast-to-heroine)

## Disclaimer

The content of this website is for educational purposes only.