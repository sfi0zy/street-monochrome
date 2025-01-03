# Street Monochrome

Black and white darktable styles for street photographers.


## Usage

These styles were tested in the darktable v4 and v5. Although they include all sorts of modules, they are designed to be applied in the **display-referred** workflow after the default workflow modules (after the base curve). Because of that most of the styles can be used with the JPG files as well as RAW files.

*Tip: You can change the default workflow in the `settings > processing > auto apply pixel workflow defaults > display referred (legacy)`.*


### Step 1. Look.

These styles create the look of the street monochrome. All of them utilize the same set of modules - `color balance rgb`, `rgb curve`, `color zones` and `monochrome`. We can switch between them easily.

The additional LUT files are created to use the same styles in the different editing programs, with JPEG files, or just to get the fast previews of the photos.

The looks are sorted from the brightest one to the darkest.

#### Standard

This is a high contrast style with a lot of blacks. It doesn't emulate any existing film, although you can find some parallels with the JCH StreetPan 400 or with the pushed Kodak Tri-X 400 film stocks. In most situations it'll work better for the underexposed images. Protect the highlights, embrace the shadows, and it'll work as intended. Don't be afraid to lower the exposure.

![examples](examples/standard.jpg)

*Tip: If you need to increase the exposure - consider using the `color balance rgb > global brilliance` slider instead of the one in the `exposure` module.*

#### Landscape

The landscape version makes the blues darker and keeps more details in the shadows and the highlights. Usually it makes the street photos look softer even though the technical contrast is almost the same as in the standard style. You may think about this style like it's a standard style with a red filter. Although it doesn't work like the real filter, the overall effect is similar in many ways. It makes the sky darker, it doesn't emphasize the objects in the foreground as much. It makes the bright reflections of the sky darker, they stand out less. It adds some details to the silhouettes, they are not as inky black as before. In the result, the images tend to look softer overall.

![examples](examples/landscape.jpg)

*Tip: If you want to make the highlights even softer with this style - consider using the `color balance rgb > highlights gain` slider.*

#### Flat

The flat version has the noticeable 50% mask on the `rgb curve`. It reduces the overall contrast a lot, but keeps the character. It's somewhat similar to the discontinued Agfa APX 25 film. The blue tones are getting darker, like in the landscape style. In the result we can get more dynamic range and save the details in both the shadows and the highlights.

![examples](examples/flat.jpg)

In some cases this style may look too flat, but it's a good choice for night photography and old school documentary photography. Usually, it works well with the vintage base.

#### Eerie

The eerie version pushes the overall balance towards the dark grey tones. It adds some Leica Monochrom vibes while keeping some of the character of the street monochrome styles. This is a good choice for the moody foggy days, dark parks, and, in some cases, the sunny days as well. It'll help to deal with the harsh sunlight. If the standard and landscape styles feel way too contrasty, and the flat looks burned out - eerie is a way to go.

![examples](examples/eerie.jpg)

*Tip: This style can be a good starting point to play with the `brilliance` sliders in the `color balance rgb` module.*


### Step 2. Effects.

There are some additional effects here.

#### + dodge and burn

This effect turns on the `shadows and highlights` module and makes the shadows darker and the highlights lighter (by default this module does everything in the opposite direction). Since it has the softening radius, the overall effect is different from the other exposure-related modules. It works somewhat similar to the classical dodging and burning process. It forms the existing light in the scene. It's a bit rough, but it'll do the job in the most cases.

*Tip: If you have a scene with a lot of details and shapes, like tree branches, try to play with the `radius` and `compress` sliders of the `shadows and highlights` module. Smaller radius and compress value less than 50% can help to form those shapes in a couple of clicks.*

#### + gradient ND2 bottom

This effect creates a ND2 gradient at the bottom of the frame (75% if we count it from the top) and rotates it 180 degrees, so it makes the bottom darker. In street photography this effect comes in handy when the floor is too bright in comparison to the other objects in the scene. For some reason all the standard presets for the `graduated density` module make the top part of the frame darker instead.

#### + cyanotype 5%, + sepia 3%

These are the toning effects. They use the `split-toning` module and are applied afterwards on top of the monochrome image. They are barely noticeable, but they can make a great impact on the viewer. There is no recipe for every situation here, but in general the sepia effect tends to make the shadows look deeper and the photo look warmer overall, and the cyanotype tends to make the photos look clean, cold and modern.

![examples](examples/toning.jpg)

The left photo in the example has the cyanotype toning, the middle one is a 100% black and white image, the right one has the sepia toning.


### Step 3 (optional). RAW Texture.

These styles are related to the RAW files.

These styles include modules that can't be saved as LUT - `demosaic`, `denoise`, `sigmoid`, `raw chromatic aberrations`, `contrast equalizer` and `sharpen`. One of them should be used as the base for the RAW files. They don't change the overall look of the images that much, but they can help with the texture. If your camera requires any special preparations - consider changing them.

*Tip: The algorithms in this step are quite demanding. If you have an old computer and it has troubles working with these modules in real time - consider editing/retouching the photos first and enabling these styles at the end.*

#### Modern

This is the standard base. Some denoise, some sharpening, some other tweaks. Nothing special. Makes the image a bit cleaner in comparison to the default darktable settings.

*Tip: The black point can be moved a bit here and it will cause underexposure. Be aware of that!*

#### Vintage

This style turns off the `sharpen` module and uses the `contrast equalizer` to add some blur to the image. Not much, but enough to make the modern oversharpened image look more soft and natural.

#### Muddy

This base is for the photos created in the darkness. ISO 51200 kind of darkness. We would not expect any fine details here. The modern base can look a bit edgy because of the random white pixels and not detailed enough at the same time. This style changes the `demosaic` algorithm and the `denoise` settings in order to get the different kind of grain. It's deep, but smooth, without any sharp edges. In normal scenarios, it'll make photos look very messy, but when we work with the insanely high ISO it does the opposite and makes them look cleaner overall and more detailed in some cases.


## Recipes

Here you'll find some recipes. They'll help you get the idea how to combine the styles to get the different results.

### Warm Vintage

flat + dodge and burn + sepia 3% + vintage

![examples](examples/vintage.jpg)

### Icy Modern

standard + cyanotype 5% + modern

![examples](examples/modern.jpg)


## Layout (experimental)

We don't really need all of the darktable modules to be on the screen while using Street Monochrome. Some of them can come in handy - `crop`, `rotate and perspective`, `exposure`, `retouch`, maybe `grain`. But the rest of them are not that useful. In order to make the work easier, you may choose to use the custom module layout. It'll have just two tabs - one for the active modules, they will be added to the list automatically, and the second one for the short list of some other modules, complementing them.

To import the layout go to `preferences > presets > modulegroups`. You'll see all the layouts you have. Use the `import` button to import the Street Monochrome layout from the `./presets/modulegroups` directory. It'll be shown there. You can always choose the layout, edit or remove them in the menu of the `modulegroups` module.


## License

CC BY 4.0

Copyright (c) 2024 Ivan Bogachev

https://instagram.com/sfi0zy
