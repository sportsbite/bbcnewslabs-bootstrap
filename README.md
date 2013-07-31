# Themestrap

**Themestrap** is a simple starter kit for constructing Twitter Bootstrap 3+ themes. It provides the skeleton
for a simple, maintainable theme that always uses code directly from Bootstrap with as little replacement as
possible.

## Themestrap's Philosophy

Themes should be as lightweight as possible and do as much as possible to be maintainable as the
framework evolves. To this end, Themestrap provides you with two simple files to modify: **variables.less**
and **theme.less** (both in the `less` directory).

You can tweak any and all of the Bootstrap variables in **variables.less** and support any additional code
or classes you'd like in **theme.less**. The compiled theme CSS will be appended after the Bootstrap CSS.

In cases where you need to do a more in-depth overhaul of a portion of Bootstrap's LESS, you may do so by
simply creating a file of the same name in Themestrap's `less` directory. Because it takes priority over
the Bower-installed Bootstrap LESS, it will automatically override the Bootstrap default. In fact, this
is how `variables.less` works already...delete it and the default Bootstrap variables will be back in play.

## Creating a Theme with Themestrap

To create a theme, first start by cloning the Themestrap repository into a directory named for
your theme. We recommend a `bootstrap-theme-THEME_NAME` naming scheme:

    git clone https://github.com/divshot/themestrap.git bootstrap-theme-THEME_NAME
    
Next, you should open `bower.json` and change the package name from `bootstrap-theme-themestrap`
to match what you want your theme to be named. Now you're ready to install dependencies using
[Grunt](http://gruntjs.com) and [Bower](https://github.com/bower/bower) (you must have these
installed).

    npm install
    bower install
    
Now you're ready to go! Simply edit `less/variables.less` and `less/theme.less` to your liking.
When you're ready, just run `grunt` and it will compile and minify the distribution for you.
You can also run `grunt watch` to automatically compile as you work.

## License

Copyright (c) 2013 Divshot

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.