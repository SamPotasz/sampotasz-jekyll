---
title: Styled components in RCT Clothes
date: 2020-04-20 00:00:00
description: This is a demo post that shows what you can do inside portfolio and blog posts. We’ve included everything you need to create engaging posts and case studies to show off your work in a beautiful way.
# featured_image: '/images/demo.jpg'
---

Today I started switching some components in RCT Shop over to `styled-components` and I found it pretty dang sweet. `styled-components` is a plugin that lets you to style your React components by writing javascript and solves some of the issues you run into writing css in large applications (such as duplicating class names or creating heavily nested class names while following [BEM](http://getbem.com/)). 

Plus, since you're writing Javascript and not css or even Sass, you can do a lot more, logic-wise. Before, you'd maybe do some logic in your component to render a different className based on a prop. 
`<component className={{isSpecial ? "special" : "notSpecial"}}/>`

That's kind of ugly.

With styled-components, you can just pass `isSpecial` into the style sheet via props, and figure out which css to render with javascript. Pretty cool, imo.

`<styledComponent {...props}> {children} </styledComponent>`

The style sheet for styledComponent is going to get `isSpecial` because you passed in `{...props}` and you can do whatever you want with it. Cool beans.

Other quick things to note when starting out with `styled-components` is that you can style not just native DOM elements, but complex React components as well. For example, you can write `StyledLink = styled(Link)` if you're importing `Link` from `react-router-dom` (or any other component you want to style).

Lastly, when switching your components over to `styled-components`, note that the newly-switched components won't have their old css class names by default. So if some other components (that contain the switched-over components, most likely) apply some styles to these class names, make sure you update these references appropriately. Adding in the `className` prop in the container component is probably the easiest method. Something like

`<Container>
    <NewlySwitchedStyledComponent className="oldClassName" />
</Container>`



