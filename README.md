## Installation Guide

### 1. Install Firefox
Make sure to have [Firefox](https://www.mozilla.org/firefox/new/) installed.

### 2. Access Firefox Profiles
Open Firefox and navigate to `about:profiles`.

### 3. Locate Profile Directory
Find and open the root directory of your profile.

### 4. Add Custom Files
- Choose either `userChrome_v1` or `userChrome_v2` in the `chrome` folder (the v2 enables a smooth animation for the auto-hidden sidebar).
- Rename the file you chose to `userChrome_v1`.
- Add the `chrome` folder to the `.default-release` folder in the root directory.


### 1. Install Sidebery
Install Sidebery from the link above.

### 2. Configure Sidebery
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
   ![Move Sidebery Sidebar](res/move_sidebery.png)

## Notice

This theme requires the [Sidebery extension](https://addons.mozilla.org/firefox/addon/sidebery/).