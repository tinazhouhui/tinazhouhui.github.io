# PF using HTML and CSS
This project started as an application for mentorship with ReactGirlsPrague, check them out at https://www.reactgirls.com/.  The goal was to create a PF without the use of Wordpress or other templates and deploy it using GitHub or Netlify.

Pull requests are welcome, if you have any suggestions on improvement 🙌

## Run
- Access the PF (here on this link)[https://tinazhouhui.github.io/]. 
- Clone this repository locally and open ```index.html```

## Technology
- code: HTML and CSS
- deploy: GitHub Pages

## Snow effect 
The biggest challenge of this effect was to create the feeling of randomness of falling snow. I have achieved that by selecting an nth element of div and changing these four parameters:
- animation keyframes - fall-left or fall-right
- animation function - ease-in or ease-out
- animation duration - 13-16 seconds
- animation delay - 4-7 minutes - this created two "batches" of falling snow
- position from which the snow flake is starting from the top - negative values so when they hit screen, they are already in motion

To decide for the calculation of nth element, I have used the help of excel. I have 30 snowflakes, so using trial and error I tried to cover all snowflakes while at the same time trying to limit each child-group to max 5 elements.

###How does it work
1. Create a ```<div>``` that would be overlapping everything else and set it to screen size - this is the area that will "hold" the snow.
2. Create your ```flakes```, here we can be more creative, either using unicode emojis like ```❄``` or in my case two divs - one for normal and one for fat snowflake. I also added a slight halo effect.
3. Define animation keyframes, or in other words the trajectory of the snowflake. Good idea is to create more than one to create variety.  
4. Create groups of snowflakes, each with its unique set of parameters mentioned above.
5. Optimise for randomness by tweaking the parameters.
6. Play ```Let it snow``` and enjoy your work.
