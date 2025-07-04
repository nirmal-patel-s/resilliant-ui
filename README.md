# Resilient UI/UX Engineering Presentation

This presentation showcases resilience engineering principles in UI/UX design using reveal.js with embedded HTML slides.

## Structure

- **index.html** - Main presentation file using reveal.js
- **1-resilliant-ui-introduction.html** - Introduction slide content
- **2-real-world-scenarios.html** - Real-world scenarios slide content
- **reveal.js-master/** - Reveal.js framework (unchanged)

## Features

✅ **Slide Navigation**: Use arrow keys, space bar, or on-screen controls to navigate between slides  
✅ **Preserved Styling**: All CSS from your individual HTML files maintains highest priority  
✅ **Responsive Design**: Works on desktop, tablet, and mobile devices  
✅ **Keyboard Shortcuts**: Press `?` to see all available shortcuts  
✅ **Overview Mode**: Press `Esc` to see all slides at once  
✅ **URL Navigation**: Each slide has a unique URL for easy sharing  

## How to Use

1. **Open the presentation**: Open `index.html` in your web browser
2. **Navigate slides**: 
   - Use arrow keys (← →) to move between slides
   - Use spacebar to go to the next slide
   - Press `Esc` for overview mode
   - Press `?` for help with shortcuts
3. **Add more slides**: Simply add more `<section>` elements with iframes pointing to your HTML files

## Navigation Controls

- **Arrow Keys**: Navigate between slides
- **Space Bar**: Next slide
- **Shift + Space**: Previous slide
- **Home**: First slide
- **End**: Last slide
- **Esc**: Toggle overview mode
- **?**: Show help overlay

## Adding New Slides

To add a new slide, simply add it to the `index.html` file:

```html
<section class="iframe-slide">
    <iframe src="your-new-slide.html" 
            frameborder="0" 
            allowfullscreen
            loading="eager">
    </iframe>
</section>
```

## Customization

### Changing Themes
Edit the theme link in `index.html`:
```html
<link rel="stylesheet" href="reveal.js-master/dist/theme/[THEME].css" id="theme">
```

Available themes: black, white, league, beige, sky, night, serif, simple, solarized, blood, moon

### Modifying Transitions
Change the transition in the JavaScript configuration:
```javascript
transition: 'slide', // none/fade/slide/convex/concave/zoom
```

### Customizing Controls
Modify the controls in the reveal.js configuration:
```javascript
controls: true,
controlsLayout: 'bottom-right', // edges/bottom-right
```

## Technical Details

- **Framework**: Reveal.js 4.x
- **Iframe Loading**: Eager loading for better performance
- **Styling Priority**: Custom CSS ensures your HTML file styles take precedence
- **Responsive**: Optimized for various screen sizes
- **Performance**: Preloads iframes for smooth navigation

## Browser Support

- Chrome (recommended)
- Firefox
- Safari  
- Edge
- Mobile browsers

## Notes

- Your individual HTML files (`1-resilliant-ui-introduction.html`, `2-real-world-scenarios.html`) remain completely unchanged
- All styling from your HTML files is preserved with highest priority
- The reveal.js-master folder is never modified
- Navigation works seamlessly between your embedded content

## Troubleshooting

If slides don't load properly:
1. Ensure all files are in the same directory
2. Check that file paths are correct
3. Verify your HTML files are valid
4. Try opening in a different browser
5. Check browser console for errors

For the best experience, run this from a local web server rather than opening the file directly in a browser.
