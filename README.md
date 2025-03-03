# html-css-lab-practice

<h1>HTML &amp; CSS Practice - building Figma wireframes for lab</h1>

<h2>Initialization</h2>
First steps: trying to create initial styles that will apply to create the "Buttons & Cards" slide:

![alt text]()

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

---
