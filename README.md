#  Annie (Zhiqing) Zhang – SFX Portfolio Website

An interactive portfolio site created to showcase sound design work with dynamic visuals, embedded media, and custom JavaScript-driven audio features. This project combines thoughtful layout, responsive design, and immersive audio-visual experiences.

---

##  Project Overview

This personal website serves as a showcase for Annie's sound design, featuring:

- A looping full-screen background video
- Interactive sound-triggering logo
- Custom-styled navigation and layout
- Embedded images and YouTube iframe content
- Multiple embedded audio players for previewing work

---

##  Development Process

### 1. HTML Layout (`index.html`) Mean page
- Used semantic tags: `<header>`, `<main>`, `<section>`, `<footer>`
- Added navigation bar with internal links
- Included media: images and YouTube iframe
- Added HTML5 `<video>` element for full-screen background:
  ```html
  <video autoplay loop muted playsinline id="bgVideo">
    <source src="video/background.mp4" type="video/mp4">
  </video>
###  Features & Corresponding CSS

1. Global Reset
2. Base Page Layout
3. Header (Fixed Top Navigation)
4. Showcase Hero Section with Background Video
5. Sound Redesign Section
6. Footer

1. White Space Under Page Instead of Full Background
Issue: There was extra white space at the bottom of the page, preventing the background video from covering the entire viewport.
Fix: Set html, body { height: 100%; }, and removed the bottom margin on elements to ensure the background covered the full page.

2. Header Logo Too Large/High
Issue: The logo in the header appeared too large and high on the page.
Fix: Used background-size: 30px 30px;, adjusted line-height, and tweaked background-position to properly size and position the logo.

3. MP4 Video Not Playing
Issue: The background MP4 video wasn’t playing.
Fix: Confirmed the correct file path, set autoplay, muted, and loop attributes, and verified browser compatibility.

4. Background Shows Incorrect Color Behind Sections
Issue: Sections had an incorrect background color that covered the video.
Fix: Applied background-color: inherit to sections to allow the video background to show through.

5. Footer Not Sticking to Bottom
Issue: The footer didn’t stick to the bottom of the page on shorter screens.
Fix: Added margin/padding to push the footer down or used a flexbox layout to ensure the footer stayed at the bottom.

6. Logo Not Clickable
Issue: The logo wasn’t clickable or interacting with JavaScript correctly.
Fix: Added id="logo" to the logo element and ensured the JavaScript targets it correctly.

7. Audio Overlapping
Issue: Multiple audio tracks could play at the same time.
Fix: Updated the script to stop any currently playing audio before starting a new one.

8. Audio Not Playing
Issue: Audio files were not playing.
Fix: Checked the autoplay policy (muted, triggered by user interaction) and verified the file paths.

9. Music Players Stacked Vertically or Misaligned
Issue: Music players were stacking vertically or misaligned in the layout.
Fix: Wrapped the music players in a .music-gallery container and applied display: flex;, flex-wrap: wrap;, and justify-content: center; for better alignment.

10. Music Players Appeared at Bottom-Left
Issue: The music players were appearing at the bottom-left of the page.
Fix: Used appropriate padding and layout structure in the <main> element to properly position the music players.

11. Header Overlapping Content
Issue: The fixed header was overlapping the main content.
Fix: Added padding-top to <main> to account for the fixed header’s height.

12. Flexbox Not Centering
Issue: Content wasn’t properly centered using Flexbox.
Fix: Verified the use of justify-content: center; and align-items: center; on the parent container to properly center the content.

###Technologies Used
HTML5: Semantic structure and multimedia integration

CSS3: Flexbox layout, visual styling, background handling

JavaScript: Audio playback interactivity, DOM manipulation

Libraries:

p5.js (included for future interactivity)


## Music Page

This is a custom music webpage created to showcase Annie's original music compositions. It features a clean, horizontally scrollable layout of interactive music players with a dynamic background video.

---

### Features

- **Responsive layout** for displaying music player cards in a horizontal scroll.
- **Background looping video** adds immersive atmosphere.
- **Multiple music players**, each with its own cover art, track title, and functional play/pause button.
- **Font Awesome icons** for navigation and media controls.
- **Custom JavaScript function** to handle individual play/pause for each track.
- **Modern styling** with flexbox, shadows, and translucent backgrounds for readability.

---

### 🛠 Troubleshooting & Challenges

1. Audio Playback Overlap  
**Issue:** All tracks could play at once.  
**Fix:** Added independent play/pause buttons per track. In the future, a function can be added to auto-pause other tracks.

2. Background Video Overlaying Content  
**Issue:** The video obscured player content.  
**Fix:** Set correct `z-index` for content and added a translucent background to players for readability.

3. Header Visibility  
**Issue:** Fixed header overlapped top content.  
**Fix:** Added `padding-top` to `main` so content doesn’t hide behind the header.

4. Music Progress Bar Sync  
**Issue:** Progress bars don't update with playback.  
**Note:** Currently static; future versions may use JS to sync.

5. Responsive Issues  
**Issue:** Layout broke on smaller screens.  
**Fix:** Used `overflow-x: auto` and `flex-shrink: 0` to allow horizontal scroll.

6. Font Awesome Icons Not Showing  
**Fix:** Verified and updated CDN to Font Awesome v6.5.0.

## Cosplay Page

### Overview
This page showcases a collection of Annie's cosplay photo edits and highlights her unique visual style. The page includes animated ghost effects, a background video, and a dynamic photo gallery. 
I mostly follow the tutorial from https://codepen.io/CreativeCoder111/pen/XWyjBab, so there isn't much debugging. 

### Features
- **Background Video**: A full-screen video plays in the background, creating a cinematic atmosphere.
- **Interactive Ghost Animation**: A spooky ghost that moves around the screen with a customizable toggle button to hide or show the animation.
- **Dynamic Photo Gallery**: A slideshow of cosplay images with brief descriptions, allowing users to view more images.
- **Sticky Header Navigation**: A fixed header with navigation links to other sections of the website.

### Technologies Used
- **HTML5**: Markup language used to structure the webpage.
- **CSS3**: Styling and layout for the page. Key features include:
  - Flexbox layout for positioning elements.
  - CSS animations for the ghost element.
  - Responsive design to ensure compatibility across devices.
- **JavaScript**: Used for handling the interaction with the ghost toggle button and enabling the dynamic features of the page.
- **Font Awesome**: For icon-based buttons (e.g., navigation arrows).
- **External CSS**: Imported libraries for font styling and animation effects.

### Code Structure
#### 1. HTML (cosplay.html)
   - Contains the structure of the page, including the header, navigation links, background video, photo gallery, and the ghost element.
   - Includes an embedded JavaScript function for toggling the visibility of the ghost.

#### 2. CSS (style.css)
   - **Global Styles**: Basic styling for body, header, and elements like buttons.
   - **Background Video**: Ensures the video fills the entire screen and is placed behind other elements.
   - **Ghost Animation**: CSS keyframes for animating the ghost element across the page.
   - **Slideshow Gallery**: Layout for the photo gallery using absolute positioning for the images and flexbox for responsiveness.
   - **Responsive Design**: Ensures proper display on smaller screen sizes, adjusting the layout of the gallery.

#### 3. JavaScript (app.js)
   - Contains logic for the ghost toggle button to show or hide the ghost element.
   - Controls the transitions for the button’s text and the visibility of the ghost.

## Cosplay Page

###I leave it in blank for now
