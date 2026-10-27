# 🎨 ColorHex Studio — Color Converter

> **Every shade. One beautiful space.**
>
> Convert HEX, RGB, and HSL colors instantly, preview shades, generate harmonious color palettes, and copy CSS color codes — all in a lightweight, browser-based application. No installation, no server, and no external dependencies required.

---

## ✨ Features

🎨 **HEX, RGB & HSL Conversion**
- Convert colors between HEX, RGB, and HSL formats.
- Enter color values manually and press Enter to apply them.
- Automatically update all color representations after conversion.
- Validate input and display clear error messages for invalid values.

🌈 **Live Color Preview**
- Preview selected colors instantly.
- Choose colors using the built-in visual color picker.
- Display the selected HEX code and RGB values.
- Explore different shades with real-time updates.

🖌️ **Color Palette Generator**
- Generate complementary color palettes.
- Create analogous color combinations.
- Explore triadic color harmonies.
- Generate monochromatic palettes.
- Click any palette shade to select and preview it.
- Copy the complete generated palette with one click.

⚡ **Random Color Generator**
- Discover random colors instantly.
- Update the color preview and conversion values automatically.
- Add random colors to your recent color history.

📋 **Convenient Controls**
- Copy HEX, RGB, and HSL values.
- Copy CSS custom property declarations.
- Copy complete color palettes.
- Save selected colors to the recent color history.
- Restore previously saved colors during the current session.
- Clear color history whenever needed.

💜 **Modern User Interface**
- Purple glass-inspired dark theme.
- Gradient backgrounds and translucent panels.
- Responsive layout for desktops, tablets, and mobile devices.
- Clean input fields and readable color previews.
- Smooth hover effects and status notifications.

🔒 **Privacy-Friendly**
- Color calculations happen locally in your browser.
- No backend server or database required.
- No account or registration required.
- No external API calls are needed for conversion.
- Your color inputs are not intentionally transmitted by the application.

---

## 📂 Project Structure

```text
ColorHex-Studio/
│
├── index.html       ← Complete web application
└── README.md        ← Project documentation
```

The application is contained in a single HTML file, including the HTML structure, CSS styling, and JavaScript logic.

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/rsamwilson2323-cloud/ColorHex-Studio.git
```

### 2️⃣ Open the Project Folder

```bash
cd ColorHex-Studio
```

### 3️⃣ Run the Application

Open `index.html` in any modern web browser.

**Windows users:** Double-click `index.html` to launch the application in your default browser.

**Note:** If your downloaded file is named `ColorHex_Studio.html`, rename it to `index.html` before publishing it through GitHub Pages.

✅ No installation process required.

---

## 📦 Requirements

```text
HTML5             Page structure and application interface
CSS3              Styling, gradients, and responsive layout
JavaScript        Color conversion and palette generation
Clipboard API     Copy color codes and palettes
Modern Browser    Chrome, Edge, Firefox, or Safari
```

**No additional dependencies are required.**

- No Node.js
- No Python
- No npm packages
- No database
- No backend server
- No external APIs

---

## 🚀 Live Demo

The application can be hosted using GitHub Pages after enabling it for the repository.

**Repository:**  
https://github.com/rsamwilson2323-cloud/ColorHex-Studio

**Application file:**  
https://github.com/rsamwilson2323-cloud/ColorHex-Studio/blob/main/index.html

**Live website:**  
https://rsamwilson2323-cloud.github.io/ColorHex-Studio/

> The live website URL will work after GitHub Pages is configured successfully and the application is published.

### Enable GitHub Pages

1. Open the ColorHex Studio repository.
2. Navigate to **Settings → Pages**.
3. Under the build and deployment settings, select **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder.
5. Click **Save**.
6. Wait for GitHub Pages to publish the website.

---

## ▶️ Usage

### 🎨 1. Choose a Color

1. Open the application.
2. Use the visual color picker to select a shade.
3. View the selected color in the preview panel.
4. Check its HEX, RGB, and HSL representations.
5. Click **Random** to discover another color.

### 🔢 2. Convert HEX, RGB, and HSL

Enter a color value in the appropriate field and press Enter.

**Example HEX input:**

```text
#8B5CF6
```

**RGB output:**

```text
139, 92, 246
```

**HSL output:**

```text
258, 90%, 66%
```

The displayed RGB and HSL values are rounded to whole numbers, so converting between formats may produce small rounding differences.

### 🌈 3. Generate Color Palettes

1. Select a base color.
2. Open the **Color Harmony** dropdown.
3. Choose a palette type.
4. Click **Generate Palette**.
5. Click any shade to select it.
6. Use **Copy Palette** to copy all generated HEX codes.

Available palette types:

- **Complementary:** Combines colors with opposite hues.
- **Analogous:** Uses neighboring hues on the color wheel.
- **Triadic:** Uses hues spaced around the color wheel.
- **Monochromatic:** Varies the lightness of a single hue.

### 📋 4. Copy CSS Color Codes

1. Select your desired color.
2. Click the relevant **Copy** button.
3. Use **Copy CSS Variable** to copy a declaration such as:

```css
--primary-color: #8B5CF6;
```

You can use this variable in your own CSS stylesheets.

### 🕘 5. Save and Restore Colors

- Click **Save to History** to save the selected color.
- Click a saved color to restore it.
- Click **Clear History** to remove all saved colors.

The current implementation stores history in memory only. Reloading the page clears the history.

---

## 🧠 How It Works

### HEX to RGB

HEX represents red, green, and blue components using hexadecimal digits.

For example:

```text
HEX:  #8B5CF6
Red:  139
Green: 92
Blue: 246
```

JavaScript parses each pair of hexadecimal digits into a decimal RGB value.

### RGB to HSL

The RGB values are normalized and converted into hue, saturation, and lightness using standard color conversion formulas.

```text
RGB: 139, 92, 246
HSL: 258, 90%, 66%
```

### HSL to RGB

The application converts the entered hue, saturation, and lightness values back into RGB values and generates the corresponding HEX code.

### Color Palette Generation

The palette generator calculates new hues and lightness values based on the selected harmony mode. Each generated color is converted to HEX for display and copying.

### Conversion Flow

```text
        COLOR INPUT
             │
             ▼
      HEX / RGB / HSL
             │
             ▼
     JavaScript Conversion
             │
             ▼
       Live Color Preview
             │
             ▼
      Palette Generation
             │
             ▼
      Copy CSS / HEX Codes
```

---

## 🛠️ Key Technical Details

| Feature | Implementation |
|---|---|
| Frontend | HTML5 |
| Styling | CSS3 |
| Application logic | Vanilla JavaScript |
| HEX conversion | JavaScript parsing and formatting |
| RGB conversion | Custom JavaScript functions |
| HSL conversion | Standard color conversion formulas |
| Color picker | HTML `<input type="color">` |
| Palette generation | HSL-based color harmony calculations |
| Clipboard | Clipboard API with fallback |
| Color history | In-memory JavaScript array |
| User interface | Responsive purple glass theme |
| Backend | Not required |
| External libraries | None |
| Internet connection | Not required for local conversion |

---

## 📌 Important Notes

- HEX input accepts six-digit codes and shorthand three-digit codes.
- RGB components must be between `0` and `255`.
- HSL saturation and lightness must be between `0%` and `100%`.
- HSL hue values can be entered outside the normal range and are normalized during conversion.
- Press Enter after editing a HEX, RGB, or HSL input to apply the value.
- Displayed HSL values are rounded to whole numbers.
- Color history is not persistent and is cleared when the page reloads.
- Clipboard functionality may depend on browser permissions and security restrictions.
- The application does not save color data to a database.
- Generated palettes are intended as practical color combinations; visual harmony is subjective.

---

## 🚀 Future Improvements

- 💾 Save color history using browser local storage.
- 📤 Export palettes as `.txt`, `.json`, or `.css` files.
- 🎨 Add custom gradient generation.
- 🌓 Add light and dark theme switching.
- 📊 Display RGB, HSL, and HEX values with more detailed color information.
- ♿ Improve accessibility and keyboard navigation.
- 🔍 Add contrast ratio calculations and WCAG accessibility checks.
- 🖼️ Extract color palettes from uploaded images.
- 🏷️ Allow users to name and organize saved palettes.
- 🔗 Generate shareable palette links.
- 🎯 Add color blindness simulation and accessible palette suggestions.

---

## ⚠️ Disclaimer

ColorHex Studio is intended for educational, creative, and personal use. It demonstrates color representation, conversion, and palette generation using standard web technologies.

The application does not guarantee that every generated palette will meet accessibility contrast requirements. Check contrast ratios separately when designing accessible interfaces.

---

## 👨‍💻 Author

**Sam Wilson**

🌐 GitHub: https://github.com/rsamwilson2323-cloud

💼 LinkedIn: https://www.linkedin.com/in/sam-wilson-14b554385/

---

## 📜 License

Add a `LICENSE` file to the repository to specify the terms under which others may use, modify, and distribute this project.

---

<div align="center">

### 🎨 ColorHex Studio

**Every shade. One beautiful space.**

*Built with HTML, CSS, and JavaScript.*

</div>
