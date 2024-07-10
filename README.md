
Here is a README file for your HTML and CSS project:

---

# Button Project

This project is a simple HTML and CSS implementation of a centered button with a hover effect.

## Project Structure

The project consists of the following files:
- `index.html`: The main HTML file.
- `style.css`: The CSS file for styling the HTML elements.

## Getting Started

To view and edit this project, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone <https://github.com/KoushalThakur/Modern-Button/>
    ```

2. **Navigate to the project directory**:
    ```bash
    cd <https://github.com/KoushalThakur/Modern-Button/>
    ```

3. **Open `index.html` in your web browser**:
    - You can double-click on the `index.html` file.
    - Alternatively, you can serve the file using a local server if you have one set up.

## HTML Structure

The HTML file (`index.html`) includes the following sections:

- **DOCTYPE Declaration**:
    ```html
    <!DOCTYPE html>
    ```

- **HTML Element**:
    ```html
    <html lang="en">
    ```

- **Head Element**:
    - Specifies the character set and viewport settings.
    - Includes the title of the page.
    - Links to the external CSS file `style.css`.

- **Body Element**:
    - Contains a wrapper div that centers the button.
    - Inside the wrapper, there is a div with the class `btn-pink` which represents the button.

## CSS Styling

The CSS file (`style.css`) includes the following styles:

- **Global Styles**:
    - Removes default margin and padding.
    - Sets `box-sizing` to `border-box` for all elements.

    ```css
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    ```

- **Wrapper Styles**:
    - Sets the height and width to 100vh to cover the viewport.
    - Uses flexbox to center the content.

    ```css
    #wrapper{
        height: 100vh;
        width: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    ```

- **Button Styles**:
    - Sets the background color, padding, text color, font size, and box shadow.
    - Positions the button relative to the page.

    ```css
    .btn-pink{
        background-color: #e84949;
        padding: 0.8rem 2.3rem;
        color: white;
        font-size: 18px;
        box-shadow: 5px 5px 7px 0px #0000003f;
        position: relative;
        z-index: 1;
    }
    ```

- **Button Hover Effect**:
    - Uses the `::before` pseudo-element to create a background overlay.
    - Transforms the overlay on hover to create an animation.

    ```css
    .btn-pink::before{
        content: "";
        background-color: #1f1f1f;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        transform: scaleX(0);
        transform-origin: left;
        transition: all 1s;
        z-index: -1;
    }

    .btn-pink:hover::before{
        transform: scaleX(1);
    }
    ```

## Usage

- **Modifying the Button Text**:
    - Change the text inside the `div` with the class `btn-pink` in the HTML file.

    ```html
    <div class="btn-pink">Hire me</div>
    ```

- **Customizing Styles**:
    - Modify the styles in `style.css` to customize the appearance of the button and the hover effect.


This README file provides an overview of the project, instructions for getting started, details about the HTML structure and CSS styling, usage guidelines, and licensing information.
This is a simple HTML and CSS code to create a stylish button with a hover effect. It can be used for various purposes like job applications, contact forms, or any other call-to-action buttons.
