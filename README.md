# Street Monochrome

Black and white darktable styles for street photographers.


## Usage

These styles are designed to be applied in the **display-referred** workflow after the default workflow modules (after the base curve).

*You can change the default workflow in the `settings > processing > auto apply pixel workflow defaults > display referred (legacy)`.*


### Step 0. RAW.

The styles in the first step are related to the RAW files.

These styles include every module that can't be saved as LUT - `demosaic`, `denoise`, `raw chromatic aberrations`, `contrast equalizer` and `sharpen`. One of them should be used as the base. They don't change the overall look of the images that much, but they can help with the texture. If your camera requires any special preparations - consider changing them. If you want to just get the look, but not to play with anything else - you can just skip this first step.

#### 0 (base)

This is the standard base. Some denoise, some sharpening, some other tweaks. Nothing special. Makes the image cleaner in comparison to the default darktable settings.

#### 0V (vintage base)

This style turns off the `sharpen` module and uses the `contrast equalizer` to add some blur to the image. Not much, but enough to make the modern oversharpened image look more natural. If you don't have the AA filter on the sensor and want to make images look softer - this base is for you.


### Step 1. Look.

These styles create the look of the street monochrome. The additional LUT files are created to use the same styles in the different editing programs, with JPEG files, or just to get the fast previews of the photos. You can use the 0 + LUT and it'll work as good as the 0 + any of the styles in the step 1.

#### S (standard)

This is a high contrast style with a lot of blacks. It doesn't emulate any existing film, although you can find some parallels with the JCH StreetPan 400 or with the pushed Kodak Tri-X 400 film stocks. In most situations it'll work better for the underexposed images. Protect the highlights, embrace the shadows, and it'll work as intended. Don't be afraid to lower the exposure.

![examples](examples-s.jpg)

*Tip: If you need to increase the exposure - consider using the `color balance rgb > global brilliance` slider instead of the one in the `exposure` module. It'll change the contrast in the relation to the exposure changes, and everything will look more natural. The standard `exposure` module works if you need to fix the overexposed areas, but if you need to make a photo a little bit brighter - it can raise the shadows too much and change the character of the photo. The `global brilliance` slider doesn't affect the shadows as much.*

#### L (landscape)

The L version makes the blues darker and keeps more details in the shadows and the highlights. Usually it makes the street photos look softer even though the technical contrast is almost the same as in the standard style. It makes the sky darker, it doesn't emphasize the objects in the foreground as much. It makes the bright reflections of the sky darker, they stand out less. It adds some details to the silhouettes, they are not as inky black as before. In the result, the images tend to look softer overall.

![examples](examples-l.jpg)

*Tip: If you want to make the highlights even softer with this style - consider using the `color balance rgb > highlights gain` slider.*

#### F (flat)

The F version has the noticeable 50% mask on the `rgb curve`. It reduces the overall contrast a lot, but keeps the character. The blue tones are getting darker as well. In the result we can get more dynamic range and save the details in both the shadows and the highlights.

![examples](examples-f.jpg)

This style is good for night photography and documentary photography. Usually, it works well with the vintage base.

#### FN (flat natural)

The FN style is the variant of the F style, but without any color corrections at all. It's just a flat style with the most natural color rendering.

#### CL, CF, CFN (clean)

These versions don't use the mask on the rgb curve. The contrast is reduced by the standard `contrast` slider. In the result, we lose some of the darkness in the shadows and get some contrast in the midtones instead. The images will look more detailed, more clean overall. These styles can help in the situations when the standard L, F, FN styles give us too muddy results.


### Step 2. Effects.

There are some additional effects here:

#### + dodge and burn

This effect turns on the shadows and highlights module and makes the shadows darker and the highlights lighter (by default this module does everything in the opposite direction). Since it has the softening radius, the overall effect is different from the other exposure-related modules. It works somewhat similar to the classical dodging and burning process. It forms the existing light in the scene. It's a bit rough, but it'll do the job in the most cases.

#### + extra crispy

This effect adds even more contrast to the highlights. It can be required in some cases of printing. But use it carefully - this kind of effect can create visible artifacts with outlines.


### Step 3. Toning.

#### + cyanotype 5%, + sepia 3%

These are the toning effects. They are barely noticeable, but they can make a great impact on the viewer. There is no recipe for every situation here, but in general the sepia effect tends to make the shadows look deeper and the photo look warmer overall, and the cyanotype tends to make the photos look clean, cold and modern.

![examples](examples-toning.jpg)

The left photo in the example has the cyanotype toning, the middle one is a 100% black and white image, the right one has the sepia toning.


## License

CC BY 4.0

Copyright (c) 2023 Ivan Bogachev

https://instagram.com/sfi0zy
