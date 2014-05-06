Orange Grid
============

A dead simple SASS grid system.

How to use
---------
First, wrap your divs in a container:

        <div class="container">
        </div>

Then use `column-*` to define the grid width. The default grid is 12 columns wide.

        <div class="container">
            <div class="column-6">Hello world</div>
            <div class="column-4">Hello world</div>
            <div class="column-2">Hello World</div>
        </div>

Mixins
---------
You can also use SASS mixins to make your HTML more semantic:

        <div class="main-content">
            <aside>This is 3 cells wide</aside>
            <section>This is 9 cells wide</section>
        </div>

        .main-content { @include container }
        aside         { @include make-column(3) }
        section       { @include make-column(9) }