# Curso de Materialize

## Typography

### Headers

We provide some basic styling on header tags. In the example, you can see the the 6 header tags' different sizes.

# Heading h1

## Heading h2

### Heading h3

#### Heading h4

##### Heading h5

###### Heading h6

### Blockquotes

Blockquotes are mainly used to give emphasis to a quote or citation. You can also use these for some extra text hierarchy and emphasis.

> This is an example quotation that uses the blockquote tag.
> Here is another line to make it look bigger.

```markup
    <blockquote>
      This is an example quotation that uses the blockquote tag.
    </blockquote>
          
```

### Flow Text

TOGGLE FLOW-TEXT

One common flaw we've seen in many frameworks is a lack of support for truly responsive text. While elements on the page resize fluidly, text still resizes on a fixed basis. To ameliorate this problem, for text heavy pages, we've created a class that fluidly scales text size and line-height to optimize readability for the user. Line length stays between 45-80 characters and line height scales to be larger on smaller screens.



------



### Images

Images can be styled in different ways using Materialize



##### Responsive Images

To make images resize responsively to page width, you can add the class `responsive-img` to your image tag. It will now have a `max-width: 100%` and `height:auto`.

```markup
    <img class="responsive-img" src="cool_pic.jpg">
        
```



##### Circular images

![img](https://materializecss.com/images/yuna.jpg)

This is a square image. Add the "circle" class to it to make it appear circular.

To make images appear circular, simply add `class="circle"` to them

```markup
      <div class="col s12 m8 offset-m2 l6 offset-l3">
        <div class="card-panel grey lighten-5 z-depth-1">
          <div class="row valign-wrapper">
            <div class="col s2">
              <img src="images/yuna.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
            </div>
            <div class="col s10">
              <span class="black-text">
                This is a square image. Add the "circle" class to it to make it appear circular.
              </span>
            </div>
          </div>
        </div>
      </div>
            
```

### Videos

We provide a container for Embedded Videos that resizes them responsively.



##### Responsive Embeds

To make your embeds responsive, merely wrap them with a containing div which has the class `video-container`

<iframe width="853" height="480" src="https://www.youtube.com/embed/Q8TXgCzxEnw?rel=0" frameborder="0" allowfullscreen="" style="box-sizing: inherit; position: absolute; top: 0px; left: 0px; width: 688.7px; height: 387.388px;"></iframe>
```markup
      <div class="video-container">
        <iframe width="853" height="480" src="//www.youtube.com/embed/Q8TXgCzxEnw?rel=0" frameborder="0" allowfullscreen></iframe>
      </div>
        
```



##### Responsive Videos

To make your HTML5 Videos responsive just add the class `responsive-video` to the video tag.

<video width="100%" controls="" style="box-sizing: inherit; display: inline-block;"></video>
```markup
  <video class="responsive-video" controls>
    <source src="movie.mp4" type="video/mp4">
  </video>
        
```



------

# Buttons

There are 3 main button types described in material design. The raised button is a standard button that signify actions and seek to give depth to a mostly flat page. The floating circular action button is meant for very important functions. Flat buttons are usually used within elements that already have depth like cards or modals.

### Raised

BUTTON  

```markup
<a class="waves-effect waves-light btn">button</a>
<a class="waves-effect waves-light btn"><i class="material-icons left">cloud</i>button</a>
<a class="waves-effect waves-light btn"><i class="material-icons right">cloud</i>button</a>
        
```

### Floating

*add*

```markup
  <a class="btn-floating btn-large waves-effect waves-light red"><i class="material-icons">add</i></a>
        
```



##### Floating Action Button

See the documentation on [this page](https://materializecss.com/floating-action-button.html)

### Flat

Flat buttons are used to reduce excessive layering. For example, flat buttons are usually used for actions within a card or modal so there aren't too many overlapping shadows.

BUTTON

```markup
  <a class="waves-effect waves-teal btn-flat">Button</a>
        
```

### Submit Button

When you use a button to submit a form, instead of using a input tag, use a button tag with a type submit

SUBMIT*send*

```markup
  <button class="btn waves-effect waves-light" type="submit" name="action">Submit
    <i class="material-icons right">send</i>
  </button>
        
```

### Large

This button has a larger height for buttons that need more attention.

BUTTON  

```markup
<a class="waves-effect waves-light btn-large">Button</a>
<a class="waves-effect waves-light btn-large"><i class="material-icons left">cloud</i>button</a>
<a class="waves-effect waves-light btn-large"><i class="material-icons right">cloud</i>button</a>
        
```

### Small

When mouse and keyboard are the primary input methods, this smaller button is useful for denser UI layouts.

BUTTON  

```markup
<a class="waves-effect waves-light btn-small">Button</a>
<a class="waves-effect waves-light btn-small"><i class="material-icons left">cloud</i>button</a>
<a class="waves-effect waves-light btn-small"><i class="material-icons right">cloud</i>button</a>
        
```

### Disabled

This style can be applied to all button types

BUTTON   

```markup
<a class="btn-large disabled">Button</a>
<a class="btn disabled">Button</a>
<a class="btn-flat disabled">Button</a>
<a class="btn-floating disabled"><i class="material-icons">add</i></a>
        
```

