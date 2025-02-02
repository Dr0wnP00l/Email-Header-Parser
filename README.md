# Email Header Parser (w/ Attitude)

A **single-page web tool** that parses raw email headers and delivers **snarky insults** while sporting a color-pulsing UI. It’s a self-contained `.html` file—no dependencies or build steps required.


## Features

1. **Email Header Parsing**  
   - Extracts key info: **sender email**, **mail server name**, **mail server IP**, **message ID**, **date**, **subject**, etc.

2. **Snarky Insults**  
   - **Random** comedic lines appear in:
     - The **description** text at page load
     - The **Parse** button’s label
     - A final **“insult”** after parsing  
   - If you paste nothing, the parser *still* mocks you.

3. **Color-Pulsing UI**  
   - The interface transitions from **green → cyan → purple → green** on a 6-second loop.

4. **All-in-One HTML**  
   - Just open **index.html** in any modern browser—no external scripts or frameworks needed.

## Getting Started

1. **Clone or Download** this repository.  
2. **Open** the file `index.html` in your browser (Chrome, Firefox, Edge, etc.).  
3. **Paste** the raw email header into the text area.  
4. **Click** the snarky button to see the parsed fields and get roasted.

## Usage

- **Parsed Fields**: The code looks for common lines like `From:`, `Received:`, `Message-ID:`, etc.  
- **Snark**: Insults are defined in arrays at the top of the `<script>`—adjust them freely to tweak the tone.  

## Customization

- **Colors & Pulse Speed**: Tweak the `getPulseColor()` function to choose other color stops or change timing.  
- **Insults**: Swap out or add new lines in the arrays (`descriptionInsults`, `buttonInsults`, `finalInsults`) to personalize the mockery.  
- **Regex Fields**: Extend the `parseEmailHeader()` function to capture additional header fields or handle different formatting.


## License

This project is released under the [MIT License](LICENSE). Use it, remix it, and have fun—don’t forget to keep insulting your friends (or yourself)!
