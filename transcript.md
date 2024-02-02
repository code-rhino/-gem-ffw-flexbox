## Reference Video 

[Video](https://vimeo.com/user214919587/review/909134100/9aef9e8aed)

## Steps

To create a Bento Box style layout using Flexbox, follow these step-by-step instructions, which are derived from the provided script and code. This guide will help you understand how to implement a responsive layout that adjusts to different screen sizes, ideal for dashboards or layout designs that require elements to be organized in an efficient, flexible manner.

### Step 1: Setup the HTML Structure
Create an HTML file with a `div` element assigned the class `bento-box`. Inside this container, add six `div` elements, each with the class `box` and a unique ID (`box1`, `box2`, etc.). Each box contains a number indicating its order.

```html
<div class="bento-box">
    <div class="box" id="box1">1</div>
    <div class="box" id="box2">2</div>
    <div class="box" id="box3">3</div>
    <div class="box" id="box4">4</div>
    <div class="box" id="box5">5</div>
    <div class="box" id="box6">6</div>
</div>
```

### Step 2: Add CSS for the Basic Layout
Link a CSS file to your HTML and set basic styles. Set the display of `.bento-box` to flex, enabling Flexbox for its children (the boxes). Use `flex-wrap` to allow the boxes to wrap within the container, and `justify-content` to center them within the container. Add a gap between the boxes for spacing and padding inside the `.bento-box` container for some inner spacing.

```css
.bento-box {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
    padding: 10px;
}
```

### Step 3: Style the Boxes
For each `.box`, apply Flexbox to center their content both vertically (`align-items: center`) and horizontally (`justify-content: center`). Set the text color to white, font size to 24px, and font weight to bold. This ensures the content inside each box is centered and legible.

```css
.box {
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-size: 24px;
    font-weight: bold;
}
```

### Step 4: Customize Each Box
Assign specific background colors, widths, and heights to each box to create a visually appealing Bento Box layout. This step involves setting unique styles for each box by targeting their IDs.

```css
#box1 {
    background-color: #FF6347; /* Tomato */
    width: 150px;
    height: 100px;
}

#box2 {
    background-color: #4682B4; /* Steel Blue */
    width: 100px;
    height: 150px;
}

#box3 {
    background-color: #32CD32; /* Lime Green */
    width: 200px;
    height: 100px;
}

#box4 {
    background-color: #FFD700; /* Gold */
    width: 120px;
    height: 120px;
}

#box5 {
    background-color: #6A5ACD; /* Slate Blue */
    width: 180px;
    height: 90px;
}

#box6 {
    background-color: #FF69B4; /* Hot Pink */
    width: 100px;
    height: 200px;
}
```

### Step 5: Adjust and Test Responsiveness
The `flex-wrap` property ensures that as the viewport size changes, the boxes will wrap within the container, maintaining their sizes but adjusting their positions to fit the screen. Test your layout on different devices (desktop, tablet, mobile) to ensure the layout adjusts properly and maintains a visually pleasing arrangement.

### Final Notes
The combination of Flexbox properties like `display: flex`, `flex-wrap`, `justify-content`, and `align-items` with customized box dimensions and colors creates a responsive, adaptable Bento Box style layout. This layout can be further customized with media queries or additional styles to enhance responsiveness or visual appeal.