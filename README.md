# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./images/testimonial.PNG)

### Links

- Solution URL: [https://github.com/cenkderman/Testimonials-grid-section](hhttps://github.com/cenkderman/Testimonials-grid-section)
- Live Site URL: [https://cenkderman.github.io/Testimonials-grid-section/](https://cenkderman.github.io/Testimonials-grid-section/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

Desktop grid

```css
.card-wraper {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-areas: "daniel daniel jonathan kira"
        "jeanette patrick patrick kira";
    gap: 2rem;
    max-width: 70rem;
    font-family: var(--ff);
}
```
Mobile grid

```css
@media screen and (max-width:428px) {
    .card-wraper {
        grid-template-columns: 1fr;
        grid-template-areas: "daniel"
            "jonathan"
            "jeanette"
            "patrick"
            "kira";
        gap: 1.25rem;
        max-width: 23rem;
        margin: 1.25rem;
    }
}
```