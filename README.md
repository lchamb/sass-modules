Sass modules
===

Not really a framework.


What is this
---

This is the general way in which I organize my sass files in an internet website(tm) project. There is a manifest file called `application.css.scss` that looks for these files:

```
normalize
variables
functions
mixins
animations
base
grid
typography
lists
buttons
forms
tables
```

Each file contains a skeleton designed to get you started in building your styles.

For example, the _buttons.scss file looks like this:

```
button,
.button {

  &:hover {}
  
  &.disabled,
  &[disabled] {}
}

input[type="input"] {

}
```


Media queries
---

Media queries are included at the bottom of each file. All of the built-in media queries target screens _above_ a certain screen width, so most of your styles are targeted to small screens, with extra styles included to make them work on larger screens. The goal is to enforce a mobile-first mentality.


FAQ
---

**Q: Who fills in the styles to make the internet look nice.**

_A: You do._

**Q: But I want someone else to do all the hard work.**

_A: There are frameworks for that._
