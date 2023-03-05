# Planning
I decided to make a page about Personal Knowledge Management (PKM) in Obsidian.
Design decisions:
- Font selection: I went with Domine for the title and Open Sans for the body text, as I feel they make a nice aesthetic pairing appropriate for this kind of topic, and both are free web fonts.
- Colour scheme: an off-white text color on a dark brown background to match the colour scheme of my Obsidian vault seemed logical.
- Maybe one or two other colours for links and drawing attention to keywords (since this is an "educational" page of sorts)
- I decided I want a fixed-position navbar at the top of the screen on larger screens, that becomes a statically positioned column of 100% width links on smaller screens.
- The navbar should have links to the different sections of the page, and clicking them should smoothly scroll to the corresponding sections.
# Building
- I set up the standard boilerplate HTML code and created a CSS stylesheet for the site.
- Initially I used some dummy text while making basic typography and colour scheme decisions, and to help plan the layout for the final page.
- I created a navbar with a fixed position and a set of links to quickly scroll to the different sections of the page, and styled them using CSS. The links organised via flexbox, with a plan to add a media query to make them display centered and one-per-line on smaller viewport sizes.
- @media query created to make the navbar display correctly on smaller screens / mobile.
- I thought it might be nice to add some icons to the navbar and found some nice free open source SVG icons at https://feathericons.com/.
- Section headings added, and font sizes, margins and padding adjusted for different screen sizes via @media query.
# Debugging
- Early on I spent a lot of time trying various colour tweaks. Perhaps a content-first approach is better?
- I had to fiddle with flexbox settings a bit to get the navbar elements to display correctly (flexbox controls are slowly sticking with me though!)
- Ensuring the correct amount of padding below the fixed vs. statically positioned navbar at different screen sizes took some fiddling.
- Figuring out how to change SVG stroke colors from within CSS took a while, because I didn't realise that an SVG used as the src in an img tag could not have CSS class styles applied to its SVG code.
- accounting for the height of the navbar when scrolling to given sections was a major pain. I used a CSS ':before' pseudo-class to target section headings and add an extra 40px of space, then a negative bottom margin on the p:last-of-type of each section of the same size.