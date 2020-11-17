# An Gáirdín
An Gáirdín is a small organic garden and education center located in Portumna, Co Galway, Ireland.

The organisation runs a small organic market garden and orchard and also has a dedicated educational space for running courses and workshops. These range from spirituality to organic gardening to plastic pollution and climate change.

[View website in GitHub Pages](https://workingedge.github.io/An-Gairdin---MS1/)
 
## UX
The site design aims to provide a simple and inviting space, encouraging further interaction with the project either online or in person.
Navigation should be simple and clearly outline the project's mission and main activities.

## Target audience
The primary audience for the website is local to the area (within 100 km) and encompasses regular visitors who may wish to get in contact or see updates, and new visitors who may become supporters. Elements of the target demograpic may not be very commfortable with interacting online - therefore the content flow should be clear and any interactive elements clear and straightforward.

There is a simple contact form that allows a user to leave a comment or to subscribe to a mailing list.

Icons allow users to quickly access the organization's social media pages (facebook only at present).

## User Stories
* As a visitor familiar with the project, I want to be able to easily get in touch with a comment or question.
* As a new visitor unfamiliar with the project I want to see a visually appealing introduction to the aims and activites undertaken and be able to easily join a mailing list or otherwise get in touch.
* As a local food enthusiast, I want to see information about the garden produce and see where this is sold locally.
* As a like-minded educator, I want to see some background information on the project and then easily get in touch with collaboration ideas using a contact form.
* As an older user or a user less-accustomed to online interation, I want to see an inviting and easy to navigate space that makes me feel at ease and is in line with my experience of the physical space.

* As a site-owner, I want to have an interenet presence that employs a look and feel in line with our aims, practices and goals. The site should mirror the atmosphere we endeavour to achieve in the physical location. 
* As a site-owner, I want site visitors to easily be able to get in touch with a question or comment, or to ask to be added to the mailing list.
* As a site-owner, I want any contact initiated on the website to go directly to my mail inbox. (nice to have, not a requirement for MS-1).
* As a site-owner, I want a visitor to be able to quickly jump to our social-media presence (facebook) where we have more up-to-date info.

## Wireframe Mockups
Wireframe mockups were developed before any coding took place and aim to give an outline of the final layout and flow of the site.
Some deviation took place during development of the site, for example:
Plan to have an image carousel is pending the delivery of images of sufficient quality
Plan to have navigation buttons on the home page was discarded as they looked cluttered and detracted from the look of the page. The hamburger icon is used on smaller screens and the navigation menu opens across the fixed top and larger scren sizes.
Wireframe designs that informed the site development can be seen here:
[V1](assets/docs/wireframe_v1.pdf)

## Color Palette
The color palette used in the site aims to mirror the changing colours of the seasons in a garden and to be at the same time warm, vibrant and inviting. Ideas in relation to colour have been gleaned from general reading. Two useful resources have been [elementor](https://elementor.com/blog/color-theory-web-design/?gclid=Cj0KCQjwreT8BRDTARIsAJLI0KKeRi1NNrRWesVXyhOmyfNpwLFH8CCWWnFQ6Ael53UB6eYECiUufkAaAmKeEALw_wcB) and [coolors] (https://coolors.co/f94144-f3722c-f8961e-f9c74f-90be6d-43aa8b-577590).
As an initial guide, I will be using the palette described in the [draft color scheme](assets/color/draft-color-scheme.pdf).

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



### Features

**navigation bar** 
The site has a navigation bar integrated into the header (nav left and logo right). This is consistent across all pages of the site and therefore easily learnable for users. It is also a very familiar pattern internet-wide and should present little or no difficulties for users.

**logo**

The project logo (text) is presented in the header on al pages.

**footer** 
Each page has a standard footer with copyright info and social media links. In relaity, this project only has a presence on facebook only. For the purposes of the MS1 project, dummy links to social media sites are (facebook, twitter, vimeo).

**copyright information** 
Copyright information is consistently dispolayed in the page footer (left).

**social media icons**  
In reality, this project only has a presence on facebook only. For the purposes of the MS1 project, I shall also include dummy links to several other sovial media sites (youtube, instagram, twitter).

**hero image** 
The main image on the home page displays the entrance to the project's physical location. As an entrance, it mirrors the purpose of the home page. The colours are echoed in the site colour scheme.

##### Home

The Home page features a real sense of the physical space occupied by this project. The welcome text also clearly identifies the underlying project ethos and invites visitors to proceed further.

##### About
The About page uses a Bootstrap card deck to present the history of the project.
The text content is broken into three sections to improve the visual appearance and add other points of interest - each text block is enhanced with a top image and a quote. For the purposes of semantic HTML, the quotes are <blockquote> and all inclue a cite attribute. The quotes are set off from the text with a top border echoing the site's header colour. The quotes replace the standard Bootstrap <card-footer> element.

##### Garden
The Garden page has two sections: Produce and Process
The layout of each mirrors the layout of the about page and again each text block is enhanced with an appropriate image and blockquote. All images (all pages) have the alt attribute filled.

## Contact

The Contact page features a **contact form**
The contact form allows for a simple message and the option to subscribe to the project's mailing list. The text area limits input to 4oo characters.
(Note: To make the form actually work is outside the scope of this MS1 project)

The bottom of the form contains a **Send Button**
The send button text is customised to maintain the welcoming feel of the project and the colour (incl hover) is also customised to align with the overall look and fel of the site. 
 
### Existing Features

### Features to Implement in future

## Technologies Used
* HTML
* CSS
* Bootstrap 4
* Gitpod
* GitHub


## Resources

## Testing 
### Testing issues - resolutions
#### CSS
https://jigsaw.w3.org/css-validator/

#### HTML
##### aria-controls
The W3C HTML checker shows an error that the aria-controls attribute is not pointing to an element in the same document. 
This is the recommended checker for ARIA: https://w3c.github.io/using-aria/#validation
Issue was reolved by removing the hash '#' before the ID, in contrast to the data-target attribute.

##### type attribute for <textarea>
The checker showed an error where I had given included "type=text" for the textarea in the contact form.
After checking https://www.w3schools.com/tags/tag_textarea.asp and https://www.w3schools.com/tags/att_input_type.asp - I have verified this is an incorrect use of the type attribute and have therefore removed it.
Tested for any impact on functinoality of the textarea - none.

### Test mobility
https://search.google.com/test/mobile-friendly

### Test contrast
https://color.a11y.com/

### Test performance
https://www.webpagetest.org/

### Test cross-browser
http://browsershots.org/

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


### Media


### Code


## Acknowledgements
For initial general guidance on the development of the MS-1 project and the README, the following pages were very helpful:
[Jim Lynx](https://github.com/JimLynx/CI-MS1-Explore-Ireland)
[A Greaves](https://github.com/AJGreaves/portrait-artist)
[ByIlsa](https://github.com/byIlsa/Aloy-from-outcast-to-heroine)

## Disclaimer

The content of this website is for educational purposes only.