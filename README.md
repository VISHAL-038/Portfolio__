# Protfolio

## Overview

This project is a responsive web application designed to showcase various projects. The application allows users to filter projects based on categories and provides a dynamic and visually appealing layout using CSS Grid and Flexbox techniques.

## Features

- **Project Filtering**: Users can filter projects based on selected categories. The filter menu is hidden by default and displayed when the user interacts with the filter select box.
- **Responsive Design**: The application is designed to be fully responsive, adapting to different screen sizes.
- **Smooth Animations**: Projects are displayed with smooth scaling animations, providing a visually engaging user experience.
- **Hover Effects**: Each project features a hover effect that reveals additional information and enhances the user interface.

## Technologies Used

- **HTML5**: Markup for structuring the content of the web application.
- **CSS3**: Styling the application, including custom properties (variables), grid layout, flexbox, transitions, and animations.

## CSS Breakdown

### Filter Menu

- **`.filter-select-box`**: Contains the filter select box. Positioned relative to allow the dropdown list to be positioned absolutely.
- **`.filter-select`**: Styles the filter select box. It’s styled to match the overall theme, with a dark background and light text.
- **`.select-list`**: Contains the dropdown list of filter options. Initially hidden, it becomes visible when the select box is active.
- **`.select-item button:hover`**: Changes the background color when a filter option is hovered.

### Project Grid

- **`.project-list`**: Uses CSS Grid to layout the project items. The grid layout ensures the projects are displayed in a single column by default.
- **`.project-item`**: Represents an individual project. The project items are hidden by default and shown when they are active.
- **`.project-img`**: Contains the project image. Includes hover effects to slightly darken the image when hovered.
- **`.project-item-icon-box`**: Displays an icon on hover, indicating that the project is clickable.

### Animation

- **`@keyframes scaleUp`**: Defines the animation for scaling up the project items when they are displayed.

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/project-showcase.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd project-showcase
   ```
3. **Open `index.html` in your browser**:
   - Double-click the `index.html` file or right-click and select "Open with" followed by your preferred browser.

4. **Interact with the Application**:
   - Use the filter menu to display projects based on categories.
   - Hover over project images to view additional information.

## Customization

You can easily customize the project by editing the following CSS variables in your `styles.css` file:

- `--eerie-black-2`: Adjusts the background color of various elements.
- `--light-gray`: Changes the text color for elements.
- `--jet`: Alters the border color.
- `--orange-yellow-crayola`: Customizes the color of the hover icons.
- `--transition-1`: Modifies the transition speed for hover effects and animations.

## Troubleshooting

### Overlapping Project Items

If you encounter issues with project items overlapping, ensure that:
- The `grid-auto-rows` property is either removed or properly adjusted.
- Consistent height is set for `.project-item` to avoid layout inconsistencies.
- Flexbox can be used instead of grid if necessary to handle varying content sizes.

