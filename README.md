# Responsive Carousel with Animations

This repository contains a responsive and animated carousel component, complete with navigation buttons, dynamic item transitions, and a detailed view feature. Built using HTML, CSS, and JavaScript, this carousel provides smooth animations and a user-friendly interface, optimized for different screen sizes.

## Features

- **Animated Transitions**: Each carousel item transitions smoothly with scaling, blurring, and translation effects to create depth and focus on the central item.
- **Navigation Controls**: Next and Previous buttons enable navigation between items.
- **Detailed View**: Each carousel item has a "See More" button that shows a detailed view. The view can be exited by clicking the "Back" button.
- **Responsive Design**: The carousel adjusts its layout and sizing to fit desktop, tablet, and mobile screens.

## Project Structure

The project includes the following files:

1. **index.html** - Contains the structure of the carousel and its elements.
2. **styles.css** - Contains styling and animations for the carousel, providing various effects based on item position and screen size.
3. **script.js** - Handles the carousel functionality, including navigation, item transitions, and the detailed view.

## Usage

1. Open `index.html` in a browser to view the carousel.

## Code Overview

### JavaScript Functionality

- **Event Listeners**: Event listeners are set up for:
  - **Next and Previous Buttons**: These trigger the `showSlider` function to move carousel items forward or backward.
  - **"See More" Buttons**: These toggle the carousel into "showDetail" mode, displaying a detailed view of the selected item.
  - **Back Button**: This button removes "showDetail" mode, returning to the carousel view.

- **`showSlider` Function**: This function manages the rotation of carousel items. Based on the navigation direction (`next` or `prev`), it appends or prepends items to keep the carousel rotating smoothly. The buttons are disabled momentarily to prevent multiple clicks during the animation.

### CSS Styling

The `styles.css` file contains:

- **Root Variables**: Variables control transform, filter, opacity, and z-index values to create different positions and styles for each carousel item.
- **Keyframe Animations**: Animations for each transition state are defined to produce smooth scaling, translation, and blurring effects as items move.
- **Responsive Design**: Media queries adjust the carousel layout and font sizes for optimal display on desktop, tablet, and mobile devices.

### HTML Structure

Each item in the carousel has a layout that includes an image, introduction text, and a "See More" button. The HTML layout is wrapped in a `.carousel` container, allowing the JavaScript to manage the carousel items and transitions.

## Customization

You can adjust the following aspects:

- **Transition Times**: Update the timing values in `script.js` or `styles.css` to customize the speed of animations.
- **Item Content**: Add or modify carousel items in `index.html` to update images, titles, descriptions, etc.
- **Styling**: Customize colors, fonts, and effects in `styles.css`.
