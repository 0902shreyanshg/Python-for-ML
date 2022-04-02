# Changing Jupyter Notebook in dark theme:

## File Path (changing CSS):
- Select Show Hidden files from view.
```C:\ProgramData\Anaconda3\Lib\site-packages\notebook\static\custom.css```

## Paste the following code in custom.css file and save it:
```
/*
Placeholder for custom user CSS

mainly to be overridden in profile/static/custom/custom.css

This will always be an empty file
*/


#ipython-main-app {
    position: relative;
}
#jupyter-main-app {
    position: relative;
}


html {
    filter: invert(1) hue-rotate(180deg) /*inverts all colors*/
}
img, picture, video {
    filter: invert(1) hue-rotate(180deg) /*invert images again so they are of original color*/
}
#notebook-container {
    background: #e0e0e0; /* make the code editing region lighter than the default from invert*/
}
.notebook_app {
      background-color: #fafafa; /* make the background region darker than the code editing region */
}
```
