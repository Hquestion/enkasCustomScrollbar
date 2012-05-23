You have an example of use in demo_extended.php

# Installation guide:

## 1) Load .js files

    <code>
        <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7/jquery.min.js"></script>
        <script src="http://ajax.googleapis.com/ajax/libs/jqueryui/1.8/jquery-ui.min.js"></script>
        <script type="text/javascript" src="js/jquery.easing.1.3.js"></script>
        <script type="text/javascript" src="js/jquery.mousewheel.min.js"></script>
        <script src="js/jquery.mCustomScrollbar.js"></script>
        <script src="js/jquery.mCustomScrollbar.enkas.js"></script>
    </code>

## 2) Add on your elements the class 'scrollbar' and make sure your elements that has the 'scrollbar' class set has also set an unique id attribute

ex:
    <code><pre>
        <div id="my_container" class="scrollbar">
            <h1>Adjustable scroller height without easing</h1>
            <p>In hac habitasse platea dictumst. Aliquam erat volutpat. Maecenas non tortor nulla, non malesuada velit. Nullam felis tellus, tristique nec egestas in, luctus sed diam. Suspendisse potenti. Cras venenatis condimentum nibh a mollis. Duis id sapien nibh. Vivamus porttitor, felis quis blandit tincidunt, erat magna scelerisque urna, a faucibus erat nisl eget nisl. Aliquam consequat turpis id velit egestas a posuere orci semper.</p>
            <h1>the end.</h1>
        </div>
    </pre></code>

## 3) Have fun! All set.

## 4) Function to load new content dynamically

    <code>
        $("#" + id + ' .content').load(file, function(){
            reInitIdScrollbar(id);
        });
    </code>