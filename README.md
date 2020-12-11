## Photo Slide Plug-in made with JavaScript ES6

In this simple documentation I shall explain how to implement my plugin into your application in order to improve your work :)

### Adding the slide plugin to your project

There are a few steps to do it, but first I have to say that I'm not the best at editing .md files so I don't know how to make internal links and all, but i'll try my best to explain how use this.

#### Functions()

Once you've downloaded the slide.js file, you'll have to import it and create a new Object just like that:

    import SlideNav from "./slide.js";

and then:

    const slide = new SlideNav(".slide", ".wrapper");

Where ".wrapper" will be the div or section that your slide will be in and ".slide" will be an ul
the Li with the images that you wanna display on your slide.

Now that you've imported the file, your next mission shall make it functional, so the next step is to init the script using:

    slide.init();

Once you've initied the slides it's already functional and you just have to add your controls, witch will be as arrows or images, by default if you do not configure custom controls you'll have to create two buttons, with the classes "prev", and "next" so you can access them in the JS using the follow function:

    slide.addArrow(".prev", ".next");

by doing it you have already added a way to go further and back in the images just having to add some styles in a css file.

##### Adding a custom control

In order to use a custom control you'll only have to create an ul with the desired control, as an example I used in the original project thumbnails of the same images, although you can use whatever you want as long you have the same ammount of images and controls.

    slide.addControl(".custom-controls");

With this function you'll have to put the class "custom-controls" in the ul that you've previously created. so it can be accessed.

#### CSS

You can style the slide the way you want, I'm leaving this style.css as an example so you can follow to create your own, hope you guys can use it :)
