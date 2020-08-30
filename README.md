# __My Responsive Portfolio__
<!-- spellchecker: enable -->
For this project, my goal was to create a responsive 'About Me' page which replicated images that were provided to me during my [Coding Boot Camp.](https://bootcamp.pe.gatech.edu/coding/)

Throughout this project, we utilized the [Bootstrap](getbootstrap.com) CSS framework in order to appropriately style our elements on the page. 

While I will, in all likelihood, create a new, personalized, 'About Me' page; this project allowed me to explore different Bootstrap Components and how to utilize them. Please see below for some of the important techniques and components that were used throughout this project.

## __VIP Components, Utilities and Techniques__

### __.nav__

The [.nav](https://getbootstrap.com/docs/4.5/components/navs/) component in Bootstrap allowed us to apply styling to our `<header>` elements which we could then customize using different Bootstrap classes within our HTML.

### __.card__

We used the [.card](getbootstrap.com/docs/4.5/components/card/) component throughout this project to apply Bootstrap styling to a `<div>` with the class of `.container`.

### __Flex__
Bootstrap components often incorporate [Flex](https://getbootstrap.com/docs/4.5/utilities/flex/), allowing us to position content within a container using flex properties. This gives us greater control over how elements behave on a page. 

### __Grid System__
In tandem with Flex, using a [Grid System](getbootstrap.com/docs/4.5/layout/grid/) was essential to styling the webpage's layout. This allows us to more effectively control elements on the page by assigning them into rows and columns which can be given Bootstrap classes to control their individual breakpoints.


## __Challenges__

The challenge of this project came primarily in the form of diligent reference to the Bootstrap [Documentation](getbootstrap.com/docs/4.5/getting-started/introduction/).


The tools needed to complete this project are all readily available on the Bootstrap website, but in order to use them properly, it was important to read carefully through the documentation and make changes to your local code as necessary. 

Along with the understanding of the individual components, it was essential to gain a conceptual understanding of what exactly the Grid System was doing and how it worked.


## __Issues During Production__

One of the most technically challenging stages of this project for me personally was trying to get the `<footer>` to behave as it should on the page.

I could set the footer to be fixed to the bottom of the page, but not keep it below the content.

I ended up accomplishing this researching footer behavior and eventually finding a class of `.footer-copyright` which I added to my `<footer>` element. I then set the `min-height` of my `<main>` element to be:

(100% of the Viewport Height - (total height of my `<header>`) - (total height of my `<footer>`) using the css `calc()` function. 

This makes it so that as long as the content is shorter than the viewport height, the footer displays at the bottom of the page, but when the content extends past the viewport height, the footer is then pushed down below. 

You can see the corresponding code below:

    main {
    min-height: calc(100vh - 62px - 69px);
    }

While this does work, I know, after researching, that this solution my cause issues in some browsers. 

I believe the same result can be accomplished by setting a `<footer>` to be _absolutely_ position at the bottom of a page, _relative_ to the body, and then adding padding equivalent to the pixel height of the footer. I plan on trying to replicate the same result in a separate project and updating this file with the results.

## __Credits__

I collaborated on this project with the help of my classmates from the Coding Boot Camp.

Additionally, I frequently referenced resources including: 

* https://getbootstrap.com/
* https://www.w3schools.com/
* https://developer.mozilla.org/en-US/
* https://www.stevensegallery.com/

## __Links__

Please find the links to the published webpage and the repository below. 
<br>

[__Web Page__ ](https://ad-fleming.github.io/alexander-my-responsive-portfolio/)

[__Repository__ ](https://github.com/ad-fleming/alexander-my-responsive-portfolio)













    
