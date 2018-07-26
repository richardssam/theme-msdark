# Dark MS Theme
This is simple fork of the Cayman theme, modified with dark background and Microsoft fonts (Segoe UI) and colours, plus some bonus features.

## Usage
Enable GitHub pages on your repo. Set the theme in `_config.yml` (in root of your repo) as follows:
```
remote_theme: benc-uk/theme-msdark
```

## Features
There are a few features and options beyond the basic Cayman theme

### Header Buttons
You can modify the buttons shown in the site header via several settings in `_config.yml`

`show_downloads: true/false` Show or hide download buttons. Default is hidden

`hide_github: true/false` Show or hide link to GitHub repo page. Default is shown

Array of custom buttons to show in the header can be set in `buttons:` Each button item needs two properties **name**, which is shown on the button, and **href** which is the link for the button 

Example:
```
buttons:
  - name: Test Header Button
    href: http://example.net
  - name: Blah Test
    href: http://google.com
```

### Header Icon
A semi-translucent icon can be shown in the top right of the header. These icons come from Font Awesome. You can get the [list of possible icons here](https://fontawesome.com/icons?d=gallery&m=free). This example below will show the [solid "comment-dots" icon](https://fontawesome.com/icons/comment-dots?style=solid) in the header
```
icon: fas fa-comment-dots
```

### Header Colours
The default header colours are a gradient from light to dark blue, you can change these colours in the `_config.yml`, as follows:
```
header-colours: 
  right: "#8a108c"
  left: "#cc580c"
```
Note. Be careful to enclose any HTML colour hex codes (e.g. `#00ff00`) in double quotes otherwise they will be treated as a comment


### Favicon
Set the URL of a PNG favicon for the site in `_config.yml`, e.g.
```
favicon: /assets/img/icon.png
```

### Custom CSS classes
Several custom CSS classes are provided
- `.btn-blue` - Convert link to a blue button
- `.btn-green` - Convert link to a green button
- `.btn-grey` - Convert link to a grey button
- `.framed` - Add a frame around images

To use these in Jekyll markdown use the special `{: .class}` annotation, which you can add after an element e.g.

```
[I Am A Button](docs/stuff.md){: .btn-blue}

![framed image](/img/picture.png){: .framed}
```

> Note. Any h4 and h5 headings which are also links will automatically be converted to buttons. This enables you to use buttons without cluttering you markdown with extra annotations, e.g.  
> `#### [Auto Button](http://example.net)`

## Demo

#### [Demo Page](demo)


