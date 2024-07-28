
# Create Animated Heartfelt Message with Dynamic Heart Effects

## Overview

The **Surprise Proposal Animation** project creates an interactive and engaging proposal experience using HTML, CSS, and JavaScript. It combines animations, a typewriter effect, and responsive design to deliver a heartfelt message in a visually appealing way. The project dynamically adjusts the content and layout based on the device's screen size, enhancing the user experience across different platforms.

## Features

- **Typewriter Effect**: Presents a personalized message with a typewriter animation.
- **Floating Hearts**: Adds a romantic touch with hearts that float across the screen.
- **Responsive Design**: Adapts to various screen sizes with device-specific background images.
- **Background Image Transitions**: Changes background images and animations based on specific characters in the typewriter message.
- **Background Music**: Plays a background music track continuously, looping every 65 seconds to enhance the experience.

## Files Included

- `index.html`: The main HTML file containing the structure of the page.

## Key Implementations

### 1. Typewriter Effect

The typewriter effect reveals a personalized message one character at a time. Special characters in the message (`<`, `>`, `|`, `9`) trigger specific actions:
- `<` inserts a line break.
- `>` clears the displayed text.
- `|` changes the background image and increases heart animation frequency.
- `9` clears the background image and sets a new background image based on the device type.

### 2. Floating Hearts Animation

Hearts float upwards in a continuous loop, adding a romantic element to the animation. The hearts are styled with CSS and dynamically created using JavaScript. The animation is handled with CSS keyframes to make the hearts move smoothly and fade out as they float up.

### 3. Responsive Design

The design adjusts for mobile and desktop screens:

- **For Mobile Screens**:
  - A mobile-specific background image is used.
  - Layout and sizes are adjusted to fit smaller screens.
- **For Larger Screens**:
  - A different background image is used.
  - Layout adjustments ensure the content fits well on larger displays.

#### Mobile-Specific Adjustments:
- **Background Image**: When the `9` character is encountered, a specific background image for mobile devices is applied if the viewport width is below a defined breakpoint (e.g., 768px).
- **Layout Adjustments**: Ensures the image and text are properly positioned and sized for mobile viewing.

### 4. Background Image Handling

The project changes background images based on the typewriter message:
- **Character `|`**: 
  - Updates the background image to `final.gif`.
  - Increases the frequency of heart animations.
- **Character `9`**: 
  - Removes the current background image and sets a new one.
  - Adapts the background image for mobile devices by checking the viewport width.

### 5. Background Music

The project includes background music that plays continuously:

- **Music Loop**: The audio plays continuously and loops every 65 seconds. It starts automatically when the user clicks the "Hi" button, and stops only when the page is closed.
- **Audio Implementation**:
  - **Play and Pause**: The music starts playing when the user interacts with the page by clicking the "Hi" button.
  - **Looping Mechanism**: The audio is set to repeat every 65 seconds using JavaScript. An interval is created to handle this looping effect.

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/kamalkolisetty/proposal1.git
   cd proposal1
   ```

2. **Open the HTML File**
   Open `index.html` in a web browser to view the animation.

3. **Customize the Content**
   - **Update Background Images**: Modify the URLs in the JavaScript code to use your preferred images.
   - **Adjust Typewriter Message**: Customize the `txt1` variable in `script` to include your personal message and formatting.
   - **Update Audio**: Replace the `src` attribute in the `<audio>` element with your preferred audio file URL.

4. **Modify Responsive Settings**
   - Adjust the breakpoint in the `isMobileDevice` function in `script` to fit different screen sizes if needed.
   - Update styles in `styles.css` to fine-tune the layout and appearance.

## Development and Contribution

Feel free to contribute to this project:
- **Issues**: Report any bugs or issues you encounter.
- **Pull Requests**: Submit changes or improvements to the project.

## Acknowledgements

- **Font Awesome**: For providing the heart icons used in the animation.
- **Google Fonts**: For typography.
