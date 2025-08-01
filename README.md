# Pure CSS Responsive Infinite Logo Carousel with Fade Effects

A simple, elegant, and responsive infinite logo marquee created entirely with HTML and CSS. This project demonstrates the power of modern CSS for creating complex animations without any JavaScript.

## Features

- **Pure CSS:** No JavaScript required, ensuring lightweight and fast performance.
- **Infinite Scroll:** Logos scroll endlessly in a seamless loop.
- **Responsive:** The marquee adapts to different screen sizes.
- **Fade Effect:** A smooth gradient fade-out effect on the sides for a polished look.
- **Highly Customizable:** Easily change the logo size, animation speed, and number of visible logos using CSS custom properties.

## How to Use

1.  **HTML Structure:** Copy the HTML structure from `index.html` into your project. Place your logo images inside the `<div class="container">`.

    ```html
    <div class="container">
      <img src="path/to/your/logo1.png" alt="Logo 1">
      <img src="path/to/your/logo2.png" alt="Logo 2">
      <!-- Add more logos as needed -->
    </div>
    ```

2.  **CSS Styling:** Link the `style.css` file in the `<head>` of your HTML document.

    ```html
    <link rel="stylesheet" href="style.css">
    ```

## Customization

You can easily customize the marquee by modifying the CSS custom properties on the `.container` element, either directly in the CSS file or using inline styles.

```css
.container {
  --s: 150px; /* size of the logos */
  --d: 8s;    /* duration of the animation */
  --n: 4;     /* number of visible logos */
}
```

- `--s`: Controls the width of each logo.
- `--d`: Sets the total duration for one full loop of the animation.
- `--n`: Defines how many logos should be visible within the container at one time.

## Technical Details

- The core infinite scrolling animation is achieved using the `offset-path` and `offset-distance` CSS properties. Each logo is animated along a horizontal line defined by `offset`.
- The seamless loop is created by calculating a delayed start for each logo's animation using `calc(-1 * sibling-index() * var(--d) / sibling-count())`.
- The fade-in and fade-out effect on the sides is implemented with the `mask` property, using a `linear-gradient` to create a transparent-to-opaque-to-transparent overlay.

## Acknowledgements

This project is based on the "Responsive infinite logo marquee" Codepen by Temani Afif. You can find the original work here: [https://codepen.io/t_afif/pen/QwjGqEJ](https://codepen.io/t_afif/pen/QwjGqEJ)

## License

This project is open source and available under the MIT License.
