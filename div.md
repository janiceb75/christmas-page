## DIV ##

The div tag helps with flexibility in CSS styling.

In the following, I have a main div which is the parent div.  It is a parent div because inside of it, there are 3 child divs called div1, div2, and div3.  



```
    <head>
        <style>
            .d1{
                width: 300px;
                height: 250px;
                background-color:blue;

            }
             .d2{
                width: 300px;
                height: 250px;
                background-color:red;

            }
             .d3{
                width: 300px;
                height: 250px;
                background-color:yellow;

            }

            .main{
                display:flex;
            }



    <body>
        <div class="main">

            <div class="d1">

            <\div>

            <div class="d2">

            <\div>

            <div class="d3">

            <\div>
        <\div>


```

This would produce 3 squares on the left of our screen.  If we wanted to move d2 to the right of d1, we would adjust margins and other changes that would not look the same on different screens. It wouldn't be a consistent solution.

So, we don't want to use margins.

We want to use FLEXBOX. the display: flex; code needs to be used when your div contains children.  
1. By default, the display:flex; makes the children divs inside of that parent go side by side.
2. You cannot apply flex to child divs if they don't have anything in it.  
3. So if you want to have 2 or more divs side by side, you need to put them in a parent div and apply a flexbox to the parent.


## Flexbox properties ##

1. justify-content: space-around;  - This equally creates space around the child divs, seperating them.  This can only be in the parent div that has a flexbox applied to it. 
2. justify-content: space-between; - gives even more space
3. justify-content: space-evenly; - less space in middle.

1. align-items: center; - align items in the center vertically. It may not be able to move in the border in main does not have enough height.  
2. align-items: flex end; - the will go at the end of the border, which means the bottom since this is vertical. 



