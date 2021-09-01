# google-homepage

## Introduction
This is the first project in the Odin Project's Foundations course.  The project objective is to create a visual clone of the Google homepage.  For a more difficult objective, I also created a visual clone of the Google search results page.  It is just a visual clone of the page.  Nothing has to work.  The project is demonstration of one's HTML and CSS skills in recreating a page design.

## Google Homepage Clone
For a page that seems so simple, there's quite a few things going on in the HTML and CSS.  I tried to section off the page into different areas: header, main, and footer sections.  Within each section, I broke down each of the components and recreated them with the building blocks that I knew.  I used a lot of flexbox since it was easier to position and align elements.

### Header
The header has a group of links on the left side and another group of links with a sign in button on the right side.  To create the two groups that reside on the edges, I utilized flexbox and justifying the content with space-between.  This pushes the elements to the sides and leaves the middle open.

### Main
The main section consists of the logo, a search input, and finally the submit buttons for the search input.  The search bar was the most difficult of the section.  I chose to use a search-type input with icons in span elements to keep everything inline.  There was a lot of trial and error with the sizing and styling, but I learned a lot about putting a search box together.

One thing that looked weird after putting everything together in the main section was where the content was positioned.  The content in the main section actually sits a little bit highter than center.  There are plenty of ways to move the content up.  I chose to add padding to the main element to push the content up to the desired position.

After my first attempt, it seemed like things could be refactored to an easier configuration.  I went back and started to elminate some of the extra work that was mostly in the search input.  Although I've seen some developers use span elements for enclosing things, there really wasn't a need here because images are displayed in inline-block.  I enclosed the search elements into their own div and styled the border on the div instead of trying to piece together each individual element in the search bar.  This refactor cleaned up a lot of the HTML and CSS.

### Footer
Like the header, the footer consists of links pushed to the sides.  A simple flexbox with the space-between setting for justify-content was all that was needed.  My first attempt had this separated, but since the styling was exactly the same as the header, I combined them together on the second attempt and saved a few more lines of code.

### Google Hompage Clone Summary
I was definitely concerned with trying to clone the exact design.  I spent quite a bit of time trying to position everything as exact as possible, with the exact coloring from looking at the example styling.  It felt good to know that I can get close to cloning a webpage's design.  It's a skill I want to continue to develop since a lot of front-end development is trying to recreate what a designer envisions in a project.  And stepping away helped because looking at it with fresh eyes helped to refactor the HTML and CSS to a smaller size.

## Google Search Page Clone
I decided to go a bit further and take on the difficult assignment of recreating the search results page of Google.  This one is a bit more involved than the clean and simple homepage.  There were a lot more icons and a lot more spacing properties to work with.  I was able to reuse some of the code from the homepage clone, but because there were so many parts it's more likely that I wrote out the code.

### Header
The logo is smaller than the homepage and tucked away in the left hand corner.  The search bar with some slight rearranging was basically the same.  The right hand group was similar to the homepage.  What's new is the addition of the filtering for the different kinds of search, but this addition actually doesn't belong in the header section per se.

There's an added feature that the header does when scrolling.  The header section minus the filtering section will become fixed once scrolling begins.  The header utilizes the sticky property to create the effect of having the search bar available when scrolling through the page results.  Having sticky elements like that is great for user experience because one doesn't have to scroll back up to the top if another search needs to be made.

### Main
Building the mock search results was just a matter of breaking down the individual elements that make up a result.  Breaking down each result to a URL link, a page title link, and the meta description, each element of the result can be grouped together and styled using a class.  There's also a suggested search section that was pretty straight forward.  For the page navigation with the Google logo, I followed the original and created a table.  Modern CSS would have made this into a gridbox, but I figured I would try to create a table for the first time.  I had to individually style some of the elements, but otherwise was able to recreate the page navigation.

### Footer
This footer was not that much different than the footer from the homepage.  There's some visual styling changes, but nothing major that would warrant a drastic coding challenge.

### Google Search Clone Summary
The search results page was more involved.  There were many more parts to this page than the homepage, but complexities can be broken down into smaller elements.  With a little bit of time, it was satisfying in the end to have tackled the more difficult challenge and be able to work on webpage that was more involved.
