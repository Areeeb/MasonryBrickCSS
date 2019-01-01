# MasonryBrickCSS
`
Masonry is a JavaScript grid layout library. It helps to place elements optimally so that the grid looks impressive. Pinterest is an example of Masonry CSS.
`

To add masonry to your project, first it is preferred to add jquery as it makes your webpage faster. To add jquery, use the following command:
```
npm install jquery
```
Then make reference to jquery inside your code.

Then add a reference to masonrypackage either by downloading the package to your local project directory or by making a reference to `masonry.pkgd.js` over the web.
```
<script src="https://unpkg.com/masonry-layout@4/dist/masonry.pkgd.js" ></script>
```
or
```
<script src="https://unpkg.com/masonry-layout@4/dist/masonry.pkgd.min.js" ></script>
```

Make a div and add “grid” class to it. Then insert your child divs or child images into it. Add “grid-item” class to your child tags.
```
<div class="grid">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
    <img class="grid-item" src='../Your/Image/Path' alt="Image">
</div>
```
Add styles to `grid-item` class. For this project, You can find it [here](https://github.com/Areeeb/MasonryBrickCSS/blob/master/styles.css)
```
.grid-item {
    font-size: 30px;
    text-align: center;
    width: 200px;
}
```
Call masonry constructor, add `grid-item` as `itemSelector` and add `columnWidth` that you desire. it depend upon the number of columns that you want. For this project, you can find it [here](https://github.com/Areeeb/MasonryBrickCSS/blob/master/default.js)
```
$('.grid').masonry({
   // options
   itemSelector: '.grid-item',
   columnWidth: 200 
});
```

Execute the code and you are good to go.
