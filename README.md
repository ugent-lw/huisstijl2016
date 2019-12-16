# UGent 2016 huisstijl

Static front-end templates for the UGent website based on [Bootstrap v3.3.7](http://getbootstrap.com).

## Usage

All files that are needed to apply the new styling of UGent websites are located in the [static](static) directory. If no further development is required, it suffices to copy this directory and include the files as demonstrated in [example.html](examples/example.html).

#### Icons
Icons are a collection of custom icons, Bootstrap-Glyphicons and Font Awesome.
New icons can be added with Font Awesome since the complete collection is loaded into the pages: http://fontawesome.io/cheatsheet/

#### Features

##### Table of contents

A table of contents can be generated (see [examples/inpage_nav_left.html](examples/inpage_nav_left.html)). This features uses the [tocbot.js library](https://tscanlin.github.io/tocbot/). The JavaScript code to enable this effect is present in [main.js](js/main.js).

To enable, add a navigation block to your page.

    <aside class="col-sm-3 inpage-nav-container xs-hide">
        <div id="nav-anchor"></div>
        <nav role="navigation" data-lockfixed="true" class="padding-default bg-tertiary">
            <h2>On this page</h2>
            <div id="toc"></div>
        </nav>
    </aside>

Make sure your page content is inside #content-core block.

##### Editor CSS

A stripped-down css is generated for online editors (ckeditor/tinemce). An example can be found [here](examples/editor-ckeditor.html). 
