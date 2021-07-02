## flyo Dark theme landing page
![]()

### My process
 
I downloaded the zip file of this challenge which consist of folders and files, after extracted it and move it to my code editor [vscode]. I read through the instructions and guide , followed the step which gives me few comprehensive of the layout mobile and destop respectively.

 I did  few modification in the index file that **index.html**  came with the assest and started the coding Journey.

***Me on the index.html***  i created a `<nav></nav>` tag with and gave it class of `class="nav-bar"` which stand as parent for the nav and header section, i was a bit skeptical inbtw `class` or `id`  but i decided sit on `class`. Going forward,  i created children that hold the logo and navigation items. 

```
   <nav class="nav-bar">
      <a class="logo">
        <img src="images/logo.svg" alt="" />
      </a>
      <div class="nav-content">
        <ul>
          <li><a href="#" class="nav-link">Features</a></li>
          <li><a href="#" class="nav-link">Teams</a></li>
          <li><a href="#" class="nav-link">SignIn</a></li>
        </ul>
      </div>
    </nav>
```

Secondly, I created a cascading file **style.css** for styling and linked to the html file ***index.html** `<link rel="stylesheet" href="style.css" />` I navigates to [Googlefont](https://www.googlefont.com) on my brower as it was instructed on the project guide and i searched for [Raleway](https://fonts.google.com/specimen/Raleway) and [Opensans](https://fonts.google.com/specimen/Open+Sans). 

Fortunately, i found them and i embedded the fonts together, copied the link and pasted it inside my `<head></head>` tag of my html file. After insert the link i moved to back the **styles.css** file, i created a global styling and color variables, it pretty simple to use for me and i believed it is advanced way of writing css.

```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  /* css variables */
  --email-sign-up-background: hsl(217, 28%, 15%);
  --main-background: hsl(218, 28%, 13%);
  --footer-background: hsl(216, 53%, 9%);
  --testimonials-background: hsl(219, 30%, 18%);
\  --Blue: hsl(198, 60%, 50%);
  --Cyan: hsl(176, 68%, 64%);
  --White: hsl(0, 0%, 100%);
  --body-font: "Open Sans", sans-serif;
  --Headings-Header-Navigation-fonts: "Raleway", "san-serif";
  /* border-radius:*/
  --radius: 5px;
}
h2,
h3,
.btn {
  font-weight: 700;
  font-family: var(--Headings-Header-Navigation-font);
}
a {
  text-decoration: none;
  color: var(--White);
}
h2 {
  font-size: 40px;
}
ul,
li {
  list-style: none;
}
```

The layout consist of four sections, i created a custom class for each of them for easy styling and specification. on the first section `<article class="getStarted">....</article>` was pretty simple and as well as the styling, I had challenges specificing the background of the button, the given was shade of two colors that linear to each other proper `linear-gradient` value but chrome does not support the value from the documemtation i read. Whilst searching, i came across [CSS-gradient-genrator-factory](http://www.css3factory.com/linear-gradients/) that gave the right property from my custom color variables that is supported. that is  `-webkit-linear-gradient`. 

```
background-image: -webkit-linear-gradient(
    right,
    var(--Cyan) 0%,
    var(--Blue) 100%
  );
```

 Moving to the next section `<article class="features">.....</article>` had tons of elememt and children, i created the first and copy paste the sub children to save my precious time. layout consist four items sitting next to each other. I displayed the children with value of `grid` and supported it with `grid-template-columns` with value `: 1fr 1fr`; to give the section 1 fraction per row of available space on the section.

 Styling the `<footer></footer>` section was highly confusing and complex. I was able to achieve it with the help of `grid-template` properpty. 

### Links

- [live Demo](https://your-live-site-url.com)

### Built with

- Semantic HTML5 markup
- CSS 3
- Flexbox
- CSS Grid

### What I learned

 I learned how to use css property `grid-template` and the values needed for styling in **footer** section. I also applied it on the mobile view that makes it well-aligned.


```
footer {
  background-color: var(--footer-background);
  display: grid;
  grid-template-columns: 4fr 3fr 1fr 1fr 2fr;
  padding: 200px 80px 80px 100px;
  grid-template-rows: auto;
  column-gap: 3.75rem;
  grid-template-areas:
    "footerLogo . . . ."
    "footerlocation footerContact footer-link second social-media";

}
```
### Useful resources

- [GoogleFont](https://www.googlefont.com) - This helped me for achieving the accurate font family [Raleway](https://fonts.google.com/specimen/Raleway) [Open Sans](https://fonts.google.com/specimen/Open+Sans)and font-weight for this challenge as it is instructed to be understand. 

- [CSS-gradient-genrator-factory](http://www.css3factory.com/linear-gradients/) -This is amazing tools that literally helped in achieving colour gradient for the button.


## Author

- Frontend Mentor [@yourusername](https://www.frontendmentor.io/profile/Brymmobaggins)
- Twitter [@Brymmobaggins](https://www.twitter.com/Brymmobaggins)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

I  wil like give a shout out to (web dev simplified)[] from the contect providing on youtube and chao charles on 
