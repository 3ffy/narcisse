Narcisse
========

UX Design Experiment : How to keep a background image at its best of visibility in any vertical responsible website (background image / content).

> Narcisse got in love with his reflection; he didn't let it out of his sight and died of that illusion that had seduced him. -
Eugène Fromentin

The problem
-----------

1. I want to use a picture of a portrait at the left of my website. But i don't want to load pictures if we are in viewport phone to preserve bandwidth.

2. As i got only few space for the image container i would like to focus the visible part of that image on content that matter. I'm agreed to show the full image but only to fill the blank when space is sufficient.

3. In responsive design, we define breakpoints to manage the different website behaviours. When the main containers are set in percentage, the width of element will "jump" across the different breakpoints. It's a normal reaction relative to how media queries works, but it's really unpleasant to see for the human eyes, even more when it's about the width of a portrait !

4. Of ourse, i would like to do all that things in pure css as possible.

The solution
------------

1. Use the css property `background-size: cover` and a `custom background-position` and `background-image` [point 2].

2. Mix it with some responsive framework (bootstrap in the demo) and add css transition to give a "smooth" effect between media queries breakpoints [point 3].

3. Add some javascript to manage images and load them only if the viewport is big enought [point 1].

>Note that there is nothing "revolutionary" with Narcisse. But i never saw any website whose integrate a left background image in a such "clean" way. Most part of the time a lot of javascript is involved to redimentionize the images with a huge cpu cost and a really bad quality of result (the navigator really don't like js image manipulations and position:fixed, i won't enter into the details, but remember that image get a better rendering when managed in pure CSS).

Live demo
---------

<http://codepen.io/3ffy/pen/CmaGq>

[![A screenshot of Narcisse in action](https://raw.githubusercontent.com/3ffy/narcisse/master/img/demo2.jpg)](http://codepen.io/3ffy/pen/CmaGq)

*(Use the CodePen to get a good idea of Narcisse, but pls refer to the static demo version and launch the `index.htm` file because some features are not available on CodePen (svg support, uncatched js errors, etc.))*

> Resize the windows you will see a true fluid layout with the background image always positionned at his best.
> PS : To simplify the demo and because its purpose wasn't about bootstrap navbar, i used 2 different navbar. If you decide to fork narcisse in your own project, please don't be evil : use only 1 navbar and style it ! Scientist proved each time you duplicate some content, a kitten die somewhere.

Licence
-------

All files excepts the pictures and images are under the MIT licence, so you can do what you want with it. 

The pictures are taken by your servitor during a personal trip at Venice (Italie). They are not part of the licence, please don't use them without my agreement !

The images are random pokemon images taken over the internet for that demo purpose only. Don't use them without author agreement.

> :heart: This code is made with love, please give it some love back ! - 3ffy