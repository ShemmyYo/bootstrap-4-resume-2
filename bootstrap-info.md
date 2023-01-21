__Bootstrap__

* CSS classes used in HTML 
    - sr-only - to hide text from page but visible for aria
    ```html
    <a href="#" target="_blank" class="cv-pdf">
        <i class="fa fa-download" aria-hidden="true"></i>
        <span class="sr-only">Download link</span>
    </a>
    ```

    - no-gutters - to remove space (of 1 space) around div which is added by bootstrap.
    ```html
    <div class="row no-gutters bg-color-name-title">
        <div class="col heading">
            <h1 class="name">Rosie Odenkirk</h1>
            <h2 class="title">Full Stack Developer</h2>
        </div>
    </div>
    ```
    
    - first divclass row and second div class col is a must as per example below
    - also, col-6, col-sm-3 are specific to bootstrap
    ```html
    <div class="row no-gutters">
        <div class="col">
            <ul id="nav" class="list-inline menucontainer">
                <li class="col-6 col-sm-3 ui-menu-color-home list-inline-item manuitem">
                    <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-home" aria-hidden="true"></i><span>Home</span></a>
                </li>
                <li class="col-6 col-sm-3 ui-menu-color-resume list-inline-item manuitem">
                    <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-graduation-cap" aria-hidden="true"></i><span>Resume</span></a>
                </li>
                <li class="col-6 col-sm-3 ui-menu-color-contact list-inline-item manuitem">
                    <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-comment-o" aria-hidden="true"></i><span>Contact</span></a>
                </li>
                <li class="col-6 col-sm-3 ui-menu-color-download list-inline-item manuitem">
                    <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-download" aria-hidden="true"></i><span>Download</span></a>
                </li>
            </ul>
        </div>
    </div>
    ```

    - section

    ```html
<section class="container-fluid"> 
        <div class="row row-table">
        <!-- row is a standard of bootstrap -->
        <!-- row-table adds table tructure (bootstrap) for same height -->
            <div class="col-md-8 bg-color-three-reasons section-column">
                <div class="row">
                    <div class="col"></div>
                </div>
            </div>
        </div>

            
    </section>
    ```



__Bootstrap index (header & footer) HTML & CSS__

HTML code

<details>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css" type="text/css" />
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" type="text/css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/hover.css/2.1.1/css/hover-min.css" type="text/css" />
    <link rel="stylesheet" href="assets/css/style.css">
    <title>Rosie</title>
</head>
<body>
    <header>
        <div class="row no-gutters">
            <a class="col-md-4 logo" href="index.html"></a>
            <div class="col-md-8">
                <div class="row no-gutters bg-color-name-title">
                    <div class="col heading">
                        <h1 class="name">Rosie Odenkirk</h1>
                        <h2 class="title">Full Stack Developer</h2>
                    </div>
                </div>
                <div class="row no-gutters">
                    <div class="col">
                        <ul id="nav" class="list-inline menucontainer">
                            <li class="col-6 col-sm-3 ui-menu-color-home list-inline-item manuitem">
                                <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-home" aria-hidden="true"></i><span>Home</span></a>
                            </li>
                            <li class="col-6 col-sm-3 ui-menu-color-resume list-inline-item manuitem">
                                <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-graduation-cap" aria-hidden="true"></i><span>Resume</span></a>
                            </li>
                            <li class="col-6 col-sm-3 ui-menu-color-contact list-inline-item manuitem">
                                <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-comment-o" aria-hidden="true"></i><span>Contact</span></a>
                            </li>
                            <li class="col-6 col-sm-3 ui-menu-color-download list-inline-item manuitem">
                                <a href="#" class="hvr-sweep-to-bottom"><i class="fa fa-download" aria-hidden="true"></i><span>Download</span></a>
                            </li>
                        </ul>
                    </div>
                </div>
        
            </div>
        </div>
    </header>
    <section>

            
    </section>
    <footer class="container-fluid">
        <div id="footer-details" class="row">
            <div class="col-sm-4">
                <h5 class="uppercase general-sub">About</h5>
                <p class="inline-block">
                    Full Stack Web Developer. Skilled in everything from HTML to Heroku.
                    The capacity for structural and design thinking. 
                </p>
            </div>
            <div class="col-sm-4">
                <h5 class="uppercase general-sub">Download</h5>
                <p class="inline-block">
                    Need a printable version of my CV? Download it here.
                    <a href="#" target="_blank" class="cv-pdf">
                        <i class="fa fa-download" aria-hidden="true"></i>
                        <span class="sr-only">Download link</span>
                    </a>
                </p>
            </div>
            <div class="col-sm-4">
                <h5 class="uppercase general-sub">Social</h5>
                <ul class="list-inline social-links">
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-facebook" aria-hidden="true"></i>
                            <span class="sr-only">Facebook</span>
                        </a>
                    </li>
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-twitter" aria-hidden="true"></i>
                            <span class="sr-only">Twitter</span>
                        </a>
                    </li>
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-linkedin" aria-hidden="true"></i>
                            <span class="sr-only">LinkedIn</span>
                        </a>
                    </li>
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-pinterest" aria-hidden="true"></i>
                            <span class="sr-only">Pintrest</span>
                        </a>
                    </li>
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-instagram" aria-hidden="true"></i>
                            <span class="sr-only">Instagram</span>
                        </a>
                    </li>
                    <li class="list-inline-item">
                        <a href="#" target="_blank">
                            <i class="fa fa-youtube" aria-hidden="true"></i>
                            <span class="sr-only">You Tube</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        
    </footer>
</body>
</html>
```

</details>

CSS code

<details>

```CSS
@import url('https://fonts.googleapis.com/css?family=Roboto:100,200,300,400,500,600,700|Exo:100,200,300,400,500,600,700|Exo:100,200,300,400,500,600,700');

/* ----------------------------------------- Colours */
.bg-color-name-title {
    background-color: #676767;
}

.ui-menu-color-home {
    background-color: #e67e22

}

.ui-menu-color-resume {
    background-color: #9b59b6

}

.ui-menu-color-contact {
    background-color: #3498db

}

.ui-menu-color-download {
    background-color: #525252

}

/* ----------------------------------------- Special Paddings/margins/text */

.uppercase {
    text-transform: uppercase;
} 

.general-sub {
    font-family: "Exo", sans-serif;
    font-weight: 300;
    color: #fafafa;
}

.inline-block {
    display: inline-block;
}

/* ----------------------------------------- Heading */

header {
    margin: 0;
    
}

.heading {
    margin-left: 50px;
}
.logo {
    background: url("../images/rosie.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 360px;
    transition: all .5s ease-in-out;
    -moz-transition: all .5s ease-in-out;
    -webkit-transition: all .5s ease-in-out;
}

.name {
    font-family: "Exo", sans-serif;
    font-weight: 100;
    font-size: 46px;
    margin-top: 50px;
    color: #fff
}

.title {
    font-family: "Roboto", sans-serif;
    font-weight: 200;
    font-size: 28px;
    margin-top: 20px;
    margin-bottom: 90px;
    color: #fff;
}

.list-inline-item:not(:last-child) {
    margin: 0;
}

.menucontainer {
    font-size: 0;
}

#nav {
    margin: 0;
}

#nav li {
    font-size: 14px;
    padding: 0;
}

.manuitem {
    height: 120px;
    text-align: center;
    padding: 0 ;
}

.manuitem a {
    width: 100%;
    text-decoration: none;
    color: #fff;
    height: 120px;
}

.manuitem a i {
    padding-top: 22px;
    display: block;
    color: #fafafa;
    font-size: 26px;
}

.manuitem span {
    display: block;
    width: 100%;
    padding-top: 5px;
    text-align: center;
    text-transform: uppercase;
    font-size: 14px;
    font-weight: 300;
    letter-spacing: 2px;
}

/* ----------------------------------------- HVR Hover Colour */

.hvr-sweep-to-bottom::before {
    background-color: rgba(0,0,0,0.2);
    height: 120px;
}

/* ----------------------------------------- Footer */

footer {
    background-color: #535353;
    color: #fafafa;
    min-height: 120px;
    margin: 0;
}

.cv-pdf i {
    font-size: 18px;
    color: #fafafa;
    text-align: center;
    padding-left: 5px;
    transition: all 0.35s ease-in-out;
    -moz-transition: all 0.35s ease-in-out;
    -o-transition: all 0.35s ease-in-out;
    -webkit-transition: all 0.35s ease-in-out;
}

.cv-pdf i:hover {
    color: #e84610;
}

.social-links {
    padding-bottom: 15px;
}

.social-links li a i {
    width: 32px;
    height: 32px;
    padding: 12px 0;
    border-radius: 50%;
    font-size: 13px;
    line-height: 7px;
    text-align: center;
    color: #fafafa;
    background-color: #8f8f8f;
    transition: all 0.35s ease-in-out;
    -moz-transition: all 0.35s ease-in-out;
    -o-transition: all 0.35s ease-in-out;
    -webkit-transition: all 0.35s ease-in-out;
}

.social-links li a i:hover {
    background-color: #e84610;
}

#footer-details {
    padding: 20px;
}
```

</details>