# Preview
<div style="text-align: center;">
   <video controls>
       <source src="res/preview.mp4" type="video/mp4">
       Your browser does not support the video tag.
   </video>
</div>

## Installation Guide

### 1. Install Firefox
Make sure to have [Firefox](https://www.mozilla.org/firefox/new/) installed.

### 2. Access Firefox Profiles
- Open Firefox and navigate to `about:profiles`
    - Find and open the root directory of your profile
- Open Firefox and navigate to `about:config`
    - Set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`

### 3. Add Custom Files
- Choose either `userChrome_v1` or `userChrome_v2` in the `chrome` folder (the v2 enables a smooth animation for the auto-hidden sidebar).
- Be sure to rename the file you chose to `userChrome.css`.
- Add the `chrome` folder to the `.default-release` folder in the root directory.

### 4. Install Sidebery
- Make sure to have [Sidebery](https://addons.mozilla.org/firefox/addon/sidebery/) added as an extension for Firefox.

### 5. Configure Sidebery
- Go to Sidebery's settings.
- In the styles editor, add the contents of `sidebery.css` to the CSS option.

## FAQ

### I want to move the sidebar to the right
Steps: 
1. Change this:
    ```css
    #sidebar-header {
        display: none;
        color: var(--background-color);
    }
    ```
2. To this:
    ```css
    #sidebar-header {
        display: visible;
        color: var(--background-color);
    }
    ```
3. Move the bar to the side you desire:
   <div style="text-align: center;">
       <img src="res/move_sidebery.png" alt="Move Sidebery Sidebar">
   </div>