If you want to use some bootstrap component go to
'node_modules/bootstrap/scss/bootstrap.min.scss' and choose your component
after select import that you need copy it and paste to your own component

Example: 

    bootstrap.scss
        - @import "nav";

    MOVE IT TO YOUR COMPONENT AND CHANGE THE PATH

    _my-component.scss
        - @import "bootstrap/scss/nav"

Just add the prefix "bootstrap/scss/" to your import - done!


By default, this project includes only 
    1. base bootstrap files, without any components  (https://getbootstrap.com/docs/5.0/getting-started/introduction/)
    2. bootstrap icons (https://icons.getbootstrap.com/)
    3. animate.css (https://animate.style/)

If you don't need something of default you can go to 'index.scss' and remove
unnecessary style imports

P.S. And don't forget to remove unnecessary styles from package.json dependencies 