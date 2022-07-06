# Horiseon Solutions

### Horiseon solutions have a  webpage with bloated CSS and difficult to navigate HTML

#### Below i have detailed the process of making this code easier to manage & read.

<br>

## Changelog:

Functional:

    Fixed nav bar button labelled "Search engine optimisation", this was acheived my adding an id matching the buttons href to the section that it should direct to (Search engine optimisation)

Appearance:

    Changed website title to reflect the company name and added a Favicon (Of my own choice as a Favicon was not provided) to make the tab label in browser more useful & informative to a user

Code readbility:

    HTML:

    <div> containters swapped out for appropriate containers depending on use/location, these include:
    - <header> for the container that forms the header at the top of the page
    - <footer> for the container that forms the footer at the bottom of the page
    - <container> for the main content sections (left side)
    - <aside> for the secondary content sections that sits alongside the main content (right side)
    - <article> for content boxes within the <container> 
    - <section> for content boxes within the <aside> container

    Added notes to HTML file to explain function, changes and content separation

    CSS:

    Added notes to CSS to explain element selection 

    Grouping CSS rules that produce identical styling to simplify the CSS file and reduce number of rules. Original file contained ~35 rules, my file contains 22 rules, an example of one such grouping can be seen below:

    
    .benefit-lead {
        margin-bottom: 32px;
        color: #ffffff;
    }

    .benefit-brand {
        margin-bottom: 32px;
        color: #ffffff;
    }

    .benefit-cost {
        margin-bottom: 32px;
        color: #ffffff;
    }
    

    the same effect can be handled by my CSS rule (All 3 of the benifit-lead/brand/cost classes are article elements) reducing 3 rules to 1:

    
    article {
        margin-bottom: 20px;
        padding: 50px;
    }
    
Accesibility

    Accesility has been improved on the site by use of appropriate containers (see HTML section) as well as adding in alternative text for images using the "alt=" attribute on the <img> tag

Code edited by Michael Walters
