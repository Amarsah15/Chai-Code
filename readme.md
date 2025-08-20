# ChaiCode Landing Page

# Demo

You can view the live demo [here](https://chai-code-alpha.vercel.app/).

## Overview

This project implements a dynamic and responsive web component designed to showcase online courses with engaging animations and interactive UI elements. It features:

- A scaling video element that animates when it enters and leaves the viewport.
- A responsive typewriter text effect that adjusts to different screen sizes.
- A carousel slider for displaying multiple course offerings with video previews, outlines, pricing, and purchase links.
- Smooth animations and transitions powered by Intersection Observer and Swiper.js.
- Modern, clean, and responsive styling using CSS with custom animations and media queries.

The component is ideal for educational platforms or course marketplaces looking to present their offerings in a visually appealing and user-friendly manner.

---

## Features

### 1. Video Scaling Animation

- The main video element scales up when it is at least 50% visible in the viewport and scales down when it is not.
- This effect is implemented using the `IntersectionObserver` API for efficient viewport detection.
- Smooth CSS transitions handle the scaling animations.

### 2. Responsive Typewriter Effect

- A typewriter animation displays text with a blinking cursor.
- The width and animation duration dynamically adjust based on the viewport width to maintain readability and responsiveness.
- The effect recalculates on window resize events to adapt to screen changes.

### 3. Courses Carousel

- A carousel slider powered by Swiper.js displays multiple courses.
- Each course card includes:
  - Title and embedded YouTube video preview.
  - A detailed outline with icons representing course topics.
  - Pricing information including original price, discounted price, and savings.
  - "Buy Now" and "Learn More" buttons linking to course pages.
- The carousel supports looping, autoplay, pagination, navigation arrows, and responsive breakpoints for different screen sizes.

### 4. Styling and Animations

- Custom CSS animations for floating effects, glowing gradients, blinking dots, and scrolling tweet-like sections.
- Responsive design with media queries for mobile, tablet, laptop, and desktop breakpoints.
- Consistent typography using the "Poppins" font from Google Fonts.
- Interactive hover effects on buttons and navigation elements.

---

## Installation and Setup

## Getting Started

To get started with this project, follow these steps:

1.  **Clone the repository or download the source files:**

    ```text
    git clone https://github.com/Amarsah15/Chai-Code.git
    ```

2.  **Include the CSS and JavaScript files in your HTML:**

    ```xml
    <link rel="stylesheet" href="styles.css" />
    <script src="script.js" defer></script>
    ```

3.  **Add the required HTML structure:**

    - A video element with `id="scaleVideo"` for the scaling animation.
    - An element with class `typewriter` containing the text to animate.
    - A container with `id="swiper-wrapper"` inside a Swiper slider structure for the courses carousel.

4.  **Ensure Swiper.js library is included (via CDN or locally):**

    ```xml
    <link rel="stylesheet" href="[https://unpkg.com/swiper/swiper-bundle.min.css](https://unpkg.com/swiper/swiper-bundle.min.css)" />
    <script src="[https://unpkg.com/swiper/swiper-bundle.min.js](https://unpkg.com/swiper/swiper-bundle.min.js)"></script>
    ```

5.  **Include Tailwind CSS:**

    ```xml
    <script src="[https://cdn.tailwindcss.com](https://cdn.tailwindcss.com)"></script>
    ```

6.  **Open the HTML file in a browser to see the interactive component in action.**

### Prerequisites

- A modern web browser that supports ES6 JavaScript features and IntersectionObserver.
- Internet connection to load external fonts and YouTube embedded videos.
- Optional: Node.js and npm if integrating with a build process or local server.

---

## Usage

### Video Scaling

- The video element automatically scales when scrolled into view.
- No manual intervention needed.

### Typewriter Text

- Place any text inside an element with class `typewriter`.
- The script adjusts the animation width and speed based on screen size.

### Courses Carousel

- The `courses` array in `script.js` contains course data objects.
- Modify or add courses by editing this array.
- Each course object includes:

  - `title`: Course name.
  - `video`: YouTube embed URL.
  - `outline`: Array of strings describing course topics.
  - `price`, `original`, `discount`: Pricing details.
  - `buynow`, `learnmore`: URLs for purchase and information.

- The carousel automatically renders these courses and initializes Swiper with responsive settings.

---

## Technical Details

### JavaScript Highlights

- **IntersectionObserver** monitors the visibility of the video element to toggle CSS classes for scaling.
- **Responsive Typewriter Animation** calculates the width of the text dynamically using font size and text length, adjusting CSS custom properties and animation durations.
- **Swiper.js Integration** initializes a looping, autoplaying, and responsive slider with pagination and navigation controls.
- **Dynamic HTML Rendering** of course cards by iterating over the `courses` array and injecting structured HTML into the DOM.

### CSS Highlights

- Uses CSS variables and keyframe animations for smooth effects.
- Media queries optimize layout and font sizes for various device widths.
- Custom animations include floating, glowing gradients, blinking cursors, and smooth scrolling.
- Styling ensures accessibility and visual consistency.

---

## Customization

- **Adding Courses:** Extend the `courses` array in `script.js` with new course objects following the existing structure.
- **Styling:** Modify `styles.css` to change colors, fonts, animations, or layout.
- **Animation Timing:** Adjust animation durations and thresholds in the JavaScript for different visual pacing.
- **Video Source:** Replace the `video` URLs with your own YouTube embeds or other video sources.

---

## Dependencies

- [Swiper.js](https://swiperjs.com/) for the carousel functionality.
- Google Fonts - Poppins font family.
- Modern browser APIs: IntersectionObserver, CSS custom properties.

---

## Browser Support

Works on all modern browsers including Chrome, Firefox, Edge, and Safari that support ES6 and IntersectionObserver API.

---

## License

This project is open-source and free to use under the MIT License.

---

## Contact

For questions or support, please contact the developer or open an issue in the repository.

---
