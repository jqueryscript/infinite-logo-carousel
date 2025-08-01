# Pure CSS Responsive Infinite Logo Carousel with Fade Effects

A simple, elegant, and responsive infinite logo carousel created entirely with HTML and CSS.

[🔗 Documentation](https://www.cssscript.com/infinite-logo-carousel-fade/)

[🔗 Live Demo](https://www.cssscript.com/demo/infinite-logo-carousel-fade/)

## Features

- **Pure CSS:** No JavaScript required, ensuring lightweight and fast performance.
- **Infinite Scroll:** Logos scroll endlessly in a seamless loop.
- **Responsive:** The marquee adapts to different screen sizes.
- **Fade Effect:** A smooth gradient fade-out effect on the sides for a polished look.
- **Pause on Hover:** Pauses all logo animations simultaneously when users hover over the container area.
- **Highly Customizable:** Easily change the logo size, animation speed, and number of visible logos using CSS custom properties.

## Technical Details

- The core infinite scrolling animation is achieved using the `offset-path` and `offset-distance` CSS properties. Each logo is animated along a horizontal line defined by `offset`.
- The seamless loop is created by calculating a delayed start for each logo's animation using `calc(-1 * sibling-index() * var(--d) / sibling-count())`.
- The fade-in and fade-out effect on the sides is implemented with the `mask` property, using a `linear-gradient` to create a transparent-to-opaque-to-transparent overlay.

## Acknowledgements

This project is based on the "Responsive infinite logo marquee" Codepen by Temani Afif. You can find the original work here: [https://codepen.io/t_afif/pen/QwjGqEJ](https://codepen.io/t_afif/pen/QwjGqEJ)

## License

This project is open source and available under the MIT License.
