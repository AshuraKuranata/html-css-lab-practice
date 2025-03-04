# html-css-lab-practice

<h1>HTML &amp; CSS Practice - building Figma wireframes for lab</h1>

<h2>Initialization</h2>
First steps: trying to create initial styles that will apply to create the "Buttons & Cards" slide:

![alt text](https://github.com/AshuraKuranata/html-css-lab-practice/blob/main/img-html/Buttons%20and%20Cards%20Lab%20Practice.png)

Could not figure out why the style sheet wasn't reading in the html file.Learned that the "rel" in link specifically refers to the file being a stylesheet.

``` HTML
<link rel="stylesheet" href="./css/global.css">
```

Began with a light copy of the expected elements for the page:

``` HTML
<body>
    <header>
        <button id="first">See More</button>
        <button id="second">See More</button>
    </header>

    <div>
        <card-one>
            <blackboxwhitebox>Create a black box above & white box in the middle</blackboxwhitebox>
            Special Feature
            <footer>See More link</footer>
        </card-one>
        <card-two>
            <profile>Profile Picture look, small black circle</profile>
            <h2>Title</h2>
            <h3>Subtitle</h3>
            <ul>
                <li>Feature 1</li>
                <li>Feature 2</li>
                <li>Feature 3</li>
            </ul>
            <button id="start-now">Start Now</button>
        </card-two>
        <card-three>
            <largeblackbox>Create black box, can utilize card one's box feature as a start?</largeblackbox>
            <p>(DO FORMATTING) Lorem ipsum dolor sit, amet consectetur adipisicing elit</p>
            <footer id="three">Learn More</footer>
        </card-three>
    </div>

</body>
</html>
```

The first pass initialization on the HTML:

![alt text](https://github.com/AshuraKuranata/html-css-lab-practice/blob/main/img-html/First%20pass%20HTML%20lab.png)

---

<h2>Header See More Buttons</h2>

Added relevant color changes to the two buttons at the top of page.

Noticed similarites across all buttons (rounded corners, padding increase, transparent background for two buttons), research to learn that the CSS property to change is called "border-radius". Made adjustment to all buttons to reflect changes and some adjustments to the first "See More" button's different format (#first):

``` CSS
button {
    background-color: transparent;
    margin-right: 20px;
    border-radius: 5px;
    padding: 15px 40px 15px;
}

/*Buttons and Cards stylesheet*/
#first {
    background-color: black;
    color: white;
}
```

New view:

![alt text](https://github.com/AshuraKuranata/html-css-lab-practice/blob/main/img-html/See%20More%20Buttons%20update.png)

---

<h2>Setting up Card</h2>

Starting on the first card.  Running into a lot of issues related to understanding positioning, creating the objects within the HTML file to apply CSS changes.

Initially tried to create a single object that would then have multiple boxes within it that I'd have to position relative to that.  Searched for different answers, realized it'd be easier to break the boxes out that were positioned relative to each other.

Created the black box & a white box sectioned within it, utilized margins to properly position the object to the center. 

Completed the first box!

![alt text](https://github.com/AshuraKuranata/html-css-lab-practice/blob/main/img-html/First%20Card%20complete.png)

---

<h2>Getting other cards to align horizontally</h2>

Set .offsetbox class as "position: absolute" which then allowed any future boxes added to automatically position themselves based on the absolute position from this section.

Created second card inputs based on relative positioning of the offset box with paragraphs.

"Start Now" button was improperly setting, aligned into second box based on fixed position.

Third card easiest to set up.  Created new section based on absolute position, and aligned the third offset box in its own ID for the other items to relatively line up with.

Finalized code, output is as seen in the HTML file.