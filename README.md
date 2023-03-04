# Planning
I decided to make a page about Personal Knowledge Management (PKM) in Obsidian.
Design decisions:
- Font selection: I went with Domine for the title and Open Sans for the body text, as I feel they make a nice aesthetic pairing appropriate for this kind of topic, and both are free web fonts.
- Colour scheme: an off-white text color on a dark brown background to match the colour scheme of my Obsidian vault seemed logical.
- I decided I want a fixed-position navbar at the top of the screen on larger screens, that becomes a statically positioned column of 100% width links on smaller screens.
# Building
- I set up the standard boilerplate HTML code and created a CSS stylesheet for the site.
- Initially I used some dummy text while making basic typography and colour scheme decisions, and to help plan the layout for the final page.
- I created a navbar with a fixed position and a set of links to quickly scroll to the different sections of the page, and styled them using CSS. The links organised via flexbox, with a plan to add a media query to make them display centered and one-per-line on smaller viewport sizes.
- @media query created to make the navbar display correctly on smaller screens / mobile.
# Debugging
- Early on I spent a lot of time trying various colour tweaks. Perhaps a content-first approach is better?
- I had to fiddle with flexbox settings a bit to get the navbar elements to display correctly (flexbox controls are slowly sticking with me though!)