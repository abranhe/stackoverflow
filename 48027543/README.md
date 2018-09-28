[View on StackOverflow](https://stackoverflow.com/a/48027543/7602110)

I would like to know what really you want to do, **split an image into two pieces?** or **two images one goes up and one goes down?**

If the case is with two images you can visit this [link](https://stackoverflow.com/questions/42193749/how-to-split-an-image-responsive-into-two-div-blocks-using-css), in the answers, you will see how to split to images, something like this:


<!-- begin snippet: js hide: false console: true babel: false -->

<!-- language: lang-css -->

    #image {
        position: relative;
    	width: 200px;
    }

    #half-image {
       	position: absolute;
       	top: 0;
       	left: 0;
       	width: 50%;
       	overflow: hidden;
    }

<!-- language: lang-html -->

    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet"/>

    <div id="image">
      <img src='https://placehold.it/200x200' id='outer' class='img-responsive'>
        <div id = "half-image">
          <img src='https://placehold.it/200/e8117f' id = 'inner'>
        </div>
    </div>

<!-- end snippet -->


Then you need to need to animate your images to move, you can use [animate.css](https://daneden.github.io/animate.css/) to your images.
View the source code on GitHub [here](https://github.com/daneden/animate.css). In the `README` file he explains it how to use it!

<!-- begin snippet: js hide: false console: true babel: false -->

<!-- language: lang-css -->

    #left {
      position: absolute;
      float: left;
    }

    #right {
      float: right;
    }


    .fadeOutDown {
      -webkit-animation-name: fadeOutDown;
      -moz-animation-name: fadeOutDown;
      animation-delay: 2s;
    }
    .fadeOutUp {
      -webkit-animation-name: fadeOutUp;
      -moz-animation-name: fadeOutUp;
      animation-delay: 2s;
    }

<!-- language: lang-html -->

    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/animate.css@3.5.2/animate.min.css">

    <div id="left">
    	<img src='https://cdn.abraham.gq/stackoverflow/48027310/left.png' class="animated fadeOutDown" >
    	<div id = "right">
    		<img src='https://cdn.abraham.gq/stackoverflow/48027310/right.png'  class="animated fadeOutUp" >
    	</div>
    </div>

<!-- end snippet -->
