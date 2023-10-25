# Profile-card-component
Frontend Mentor is a website where front-end developers get a design and are asked to make it into a page to practice their skills. This repository is my approach for the following design: https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ

If you want to see this repository live you can do it here: https://avoscanemile.github.io/Profile-card-component/

**I do not own this design. If you've any questions related to it you should clarify them in the Frontend Mentor website.** 
## HTML Structure

The HTML structure of the profile card component is designed to be clean and semantically meaningful, making it easy to understand and style. Here's a detailed breakdown of the HTML structure:

### Document Structure

- `<!DOCTYPE html>`: This declaration defines the document type and version of HTML in use.

- `<html lang="en">`: The root HTML element specifies the language of the document, in this case, English.

### Head Section

- `<head>`: This section contains metadata and information about the document.

  - `<meta charset="UTF-8">`: Specifies the character encoding as UTF-8 for proper character representation.

  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Sets the viewport configuration to ensure proper scaling on different devices.

  - `<link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">`: Provides a favicon for the website.

  - `<link rel="preconnect" href="https://fonts.googleapis.com">` and `<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>`: These links establish connections to external resources (Google Fonts in this case) for improved loading performance.

  - `<link href="https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap" rel="stylesheet">`: Links to Google Fonts to import the 'Kumbh Sans' font family.

  - `<link rel="stylesheet" href="styles.css">`: This links the main CSS file, 'styles.css,' to style the HTML content.

  - `<title>Frontend Mentor | Profile card component</title>`: Sets the title of the web page, which appears in the browser's tab.

### Body Section

- `<body>`: The body section contains the visible content of the web page.

  - `<main class="card">`: This is the main container for the profile card component. It uses the 'card' class for styling and positioning.

    - `<img src="images/bg-pattern-card.svg" alt="blue circles" class="card__background">`: This image element displays the background pattern for the card. It is given the 'card__background' class for styling.

    - `<img src="images/image-victor.jpg" alt="Profile picture of a guy" class="card__profile-image">`: Displays the profile picture of the person, styled using the 'card__profile-image' class.

    - `<div class="card__info-container">`: This div contains the profile information and social statistics.

      - `<div class="card__general-info-container">`: This div is dedicated to general information about the person.

        - `<h1 class="card__general-info">Victor Crest <span class="card__age">26</span></h1>`: The person's name and age are displayed in this heading, with the name styled using the 'card__general-info' class and the age using the 'card__age' class.

        - `<p class="card__location">London</p>`: The person's location is displayed with styling provided by the 'card__location' class.

        - `<div class="card__social-info">`: Contains the social media statistics.
        
          - `<div class="card__followers">`: Displays information about followers.
        
            - `<p class="card__number">80K</p>`: Displays the number of followers with the 'card__number' class.
        
            - `<p class="card__number-tag">Followers</p>`: Indicates that these numbers represent followers using the 'card__number-tag' class.
        
          - `<div class="card__likes">`: Provides statistics on likes.
        
            - `<p class="card__number">803K</p>`: Displays the number of likes with the 'card__number' class.
        
            - `<p class="card__number-tag">Likes</p>`: Indicates that these numbers represent likes using the 'card__number-tag' class.
        
          - `<div class="card__photos">`: Displays information about the number of photos.
        
            - `<p class="card__number">1.4K</p>`: Shows the number of photos with the 'card__number' class.
        
            - `<p class="card__number-tag">Photos</p>`: Indicates that these numbers represent photos using the 'card__number-tag' class.


## CSS Styles

The CSS styles for this project are carefully structured and organized to achieve a visually appealing and responsive profile card component. Various CSS variables are used to maintain consistency in color schemes and fonts. Let's dive into the details:

### CSS Variables

The project uses CSS variables to define colors and fonts, making it easy to maintain a consistent look throughout the profile card component. Here are the variables used:

- `--clr-darkest-blue`: Represents the darkest blue color.
- `--clr-dark-blue`: Defines a slightly lighter blue color.
- `--clr-gray`: Used for gray color.
- `--clr-blue`: Specifies the primary blue color.
- `--ff`: Defines the font family, in this case, 'Kumbh Sans'.
- `--fs-big`: Sets the font size for larger text elements (e.g., the person's name).
- `--fs-small`: Determines the font size for smaller text elements (e.g., location).
- `--fs-very-small`: Sets an even smaller font size if needed.
- `--fw-regular`: Represents the regular font weight.
- `--fw-bold`: Defines a bolder font weight for emphasis.

### General Attributes

- `html`: The HTML element has some general attributes set to make the project more visually appealing and responsive. The project's background color is defined as `var(--clr-blue)`, which ensures a consistent color scheme. The `background-image` property adds background patterns, making the project more visually appealing. The `box-sizing` property is set to `border-box`, which helps with consistent box model behavior.

### Card Styling

The profile card component, defined by the `.card` class, is the central piece of this project. It's designed to create an aesthetically pleasing and responsive card. Here's a breakdown of the card styling:

- `background`: The background of the card is set to white, providing a clean and elegant appearance.
- `display`: The card is displayed using the grid layout, which allows for precise positioning of elements.
- `grid-template-rows` and `grid-template-columns`: These properties define the grid structure of the card, including rows and columns.
- `grid-template-areas`: This property maps the grid areas for the card, profile image, and information.
- `border-radius`: A rounded border radius of 20px gives the card a more modern look.
- `overflow`: Ensures that content within the card does not overflow.
- `width`: The card width is responsive and clamped between 300px and 350px.
- `justify-self`: The card is centered horizontally.
- `box-shadow`: Adds a subtle shadow to the card, providing depth and dimension.

### Card Elements

- `.card__background`: This element is responsible for styling the background image of the card. It covers the entire grid area of the card and ensures a visually appealing backdrop.

- `.card__profile-image`: This class styles the profile picture of the person. It ensures that the image is centered, rounded, and has a white border.

- `.card__info-container`: This class styles the container for the profile information. It employs grid layout to organize the content.

- `.card__general-info-container`: Within the information container, this class focuses on the general information section. It adds padding to ensure proper spacing.

- `.card__general-info`: Styles the person's name and age. It uses the defined font family, font size, font weight, and text color for consistency.

- `.card__age`: Specifically styles the age, setting a different font weight and color for distinction.

- `.card__location`: This class styles the location information. It ensures a consistent font family, font size, font weight, and text color.

- `.card__social-info`: Focuses on the container for social media statistics. It employs flexbox to arrange the statistics horizontally with space between them.

- `.card__number` and `.card__number-tag`: These classes style the numerical values and their associated tags (e.g., "Followers," "Likes," "Photos") within the social media statistics. They use the defined font family, font size, font weight, and text color for consistency.

## CSS Functions Used

- **hsl() Function**: The `--clr-darkest-blue` and other color variables use the `hsl()` function to define colors with specific hue, saturation, and lightness values.

   Example: `--clr-darkest-blue: hsl(229, 23%, 23%);`

- **var() Function**: Custom properties (CSS variables) are used throughout the CSS for defining fonts, font sizes, and other values. The `var()` function is used to apply these variables to various properties.

   Example: `font-family: var(--ff);`

- **clamp() Function**: The `width` property in the `.card` class uses the `clamp()` function to create a responsive width for the card based on the viewport width. It ensures that the card's width adapts to various screen sizes.

   Example: `width: clamp(300px, 90vw, 350px);`

**For more information on the HTML/CSS please refer to the files provided in the project**
