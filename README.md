### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

## My process
 
I downloaded the zip file of this challenge which consist of folders and files, after extracted it and move it to my code editor [vscode]. I read through the instructions and guide , followed the step which gives me few comprehensive of the layout mobile and destop respectively.

 I did  few modification in the index file that **index.html**  came with the assest and started the coding Journey.

***Me on the index.html***  i created a `<nav></nav>` tag with and gave it class of `class="nav-bar"` which stand as parent for the nav and header section, i was a bit skeptical inbtw `class` or `id`  but i decided sit on `class`. Going forward,  i created children that hold the logo and navigation items. 

```<nav class="nav-bar">
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

Secondly, I created a cascading file **style.css** for styling and link it together `<link rel="stylesheet" href="style.css" />` I navigate [Googlefont] on my brower as it was instructed on the project guide and i searched for [Raleway] and [Opensans]. fortunately, i found them and i embedded the fonts together, copied the link and paste it inside my `<head></head>` tag of my html file. After insert the link i moved to back the **styles.css** file, i created a global styling and color variables because it pretty simple to use and i believed it is advanced way of writing css.


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
  --Cyan: hsl(176, 68%, 64%);
  --Blue: hsl(198, 60%, 50%);
  --White: hsl(0, 0%, 100%);
  --body-font: "Open Sans", sans-serif;
  --Headings-Header-Navigation-fonts: "Raleway", "san-serif";
  /* border-radius: ; */
  --radius: 5px;
}
main {
  position: relative;
  padding-bottom: 150px;
}
html,
body {
  color: var(--White);
  background-color: var(--main-background);
  font-size: 14px;
  font-family: var(--body-font);
  font-weight: 400;
  box-sizing: border-box;
  scroll-behavior: smooth;
}
nav,
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
### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Live Demo[Add live site URL here](https://your-live-site-url.com)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

 I learned how to use css property `grid-template` and the values needed for styling in **footer** section. I also applied it on the mobile view that makes it well-aligned.


```footer {
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


### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [GoogleFont](https://www.googlefont.com) - This helped me for achieving the accurate font family [Raleway](https://fonts.google.com/specimen/Raleway) [Open Sans](https://fonts.google.com/specimen/Open+Sans)and font-weight for this challenge as it is instructed to be understand. 

- [CSS-gradient-genrator-factory](http://www.css3factory.com/linear-gradients/) -This is amazing tools that literally helped in achieving colour gradient for the button.


## Author

- Frontend Mentor [@yourusername](https://www.frontendmentor.io/profile/Brymmobaggins)
- Twitter [@Brymmobaggins](https://www.twitter.com/Brymmobaggins)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
