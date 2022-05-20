# xcl-bootstrap4
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/2.0.0/active.svg)](https://github.com/xoopscube/xcl)
![License GPL](https://img.shields.io/badge/License-GPL-green)
![X-Updare Store](https://img.shields.io/badge/X--Update%20Store-Pending-red)

## ///// — XCL BOOTSTRAP 4 + Custom TEMPLATES

![XCL Theme HTML5 Boilerplate](https://repository-images.githubusercontent.com/494114640/90688ec1-9e15-4f63-acbe-f1bf37e2952)
  

---

THEME | xcl-bootstrap4
------------ | -------------
Description | Starter Theme built with Bootstrap4.x with custom modules templates
Render Engine | Smarty v2 and Smarty v3
Version | 2.3.1
Author | [https://github.com/twbs](https://github.com/twbs)
Author | @gigamaster Nuno Luciano (XCL23)
Copyright | 2011-2022 Authors
License | MIT


##### :computer: The Minimum Requirements



          Apache, Nginx, etc. PHP 7.2.x
          MySQL 5.6, MariaDB  InnoDB utf8 / utf8mb4
          XCL version >= 2.3.1



-----


## Overview   

Bootstrap is a popular front-end framework for creating websites and web applications.

Render Engine - Smarty is a template engine for PHP, facilitating the separation of presentation (HTML/CSS) from application logic.  
This implies that PHP code is application logic, and is separated from the presentation, making it easier to customize theme and templates.

[What is Smarty v2](https://www.smarty.net/docsv2/en/what.is.smarty.tpl)    
[Smarty 3 Overview](https://www.smarty.net/v3_overview)    


### Features


- Layout aside left
- Layout aside right
- Header nav offcanvas
- Header nav social links
- Header nav usermenu
- Bottom center blocks
- Custom components   


### Install or Update Themes

1. Select the main branch from this repo and, from the dropdown button "Code" select Clone or Download zip.  
2. Extract and upload the folder "theme-name" to your domain, eg.: public/html/themes/theme-name/*.*  
3. Login to your Administration Control Panel » Theme Management, activate the Theme (checkbox/select).  

### User-friendly installation

**X-Update Store**  

1. Login to your the Administration Control Panel » X-Update » Themes    
2. Select the theme from the Theme Store    
3. Proceed to automatically download and install.

    
### Components 

Edit the file **theme.html** to change the header nav component or the side menu to include.    
Smarty tag comment are similar to HTML comments that begin with <! –– and are closed with ––>   
However, a Smarty tag comment is not rendered and uses an asterisk  `*`  to begin and to close i.e.:  

``` smarty
<{* smarty tag comment *}> 
```

To change the header nav, just remove the asterisk `*` from one include and
add an asterisk  `*`  to the others :    

``` smarty

<{include file="$xoops_theme/component/inc_header_nav_offcanvas.html"}>

<{* include file="$xoops_theme/component/inc_header_nav_socialinks.html" *}>

<{* include file="$xoops_theme/component/inc_header_nav_usermenu.html" *}>
```
    
To change the layout side menu, edit the file **theme.html** and change from _layout left_ to _layout right_ :    

``` smarty

<{* include file="$xoops_theme/component/layout_right.html" *}>

<{include file="$xoops_theme/component/layout_left.html"}>
```

### Theme Folder Structure

Technically, themes only require four files : manifesto.ini.php, screenshot.png, style.css, theme.html.   
You can create a folder **assets** for all the assets used in the theme, including images, stylesheets, and javascript files.    
The following is an example of the files and folders that can be found in XCL Bootstrap4 theme folder structure.</p>
        
```bash
themes
└───theme-name
    │   manifesto.ini.php
    │   style.css
    │   theme.html
    │   xcl-bootstrap45.png
    │
    ├───component
    ├───img
    └───templates
        ├───d3forum
        ├───legacy
        ├───message
        ├───pico
        └───user
```


License
-------

The Themes are released under a BSD or Creative Commons license.  
Some Components and Plugins can be released under licenses that   
guarantee a certain specific set of freedoms - GPL, MIT, etc.  

[LICENSE](LICENSE)

Code contributions
----------------

If find a bug or it's a feature that you think should be implemented [please open an issue first](https://github.com/xoopscube-themes/xcl-html5-boilerplate/issues),   
join or start a [new discussion](https://github.com/orgs/xoopscube-themes/discussions).    

Otherwise, you can follow this process:

1. Fork the project [Fork a Repo](http://help.github.com/fork-a-repo/)
2. Create a feature branch : `git checkout -b my_branch`
3. Push your changes to your new branch : `git push origin my_branch`
4. Initiate a pull request [About Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
5. Your pull request will be reviewed and hopefully merged :)

Have Fun ^_^/
