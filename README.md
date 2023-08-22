# Street Monochrome

Black and white darktable styles for street photographers.

## Usage

These styles are designed to be applied in the **display-referred** workflow after the default workflow modules.

*You can change the default workflow in the `settings > processing > auto apply pixel workflow defaults > display referred (legacy)`.*

### Step 1. RAW.

The styles in the first step are related to the RAW files.

#### 0 (zero)

This style includes every module that can't be saved as LUT - `demosaic`, `denoise`, `raw chromatic aberrations`, `contrast equalizer` and `sharpen`. This style should be used as the base. It doesn't change the overall look of the image that much, but it can help with the texture. If your camera requires any special preparations - consider changing it. If you want to just get the look, but not to play with anything else - you can just skip this first step.

#### SM

This style includes the `rgb curve` + `monochrome` modules. Basically, it's the heart of the whole pack of these styles. It makes the character. If you want to use this curve somewhere else for some reason - this style is for you. In the standard workflow you'll probably never need it, since it's included in every style in the step 2.

### Step 2. Look.

These styles create the look of the street monochrome. The additional LUT files are created to use the same styles in the different editing programs, with JPEG files, or just to get the fast previews of the photos. You can use the 0 + LUT and it'll work as good as the 0 + any of the styles in the step 2.

#### S (standard)

![examples](examples-s.jpg)

This is a high contrast style with a lot of blacks. It doesn't emulate any existing film, although you can find some parallels with the JCH StreetPan 400 or with the pushed Kodak Tri-X 400 film stocks. In most situations it'll work better for the underexposed images. Protect the highlights, embrace the shadows, and it'll work as intended. Don't be afraid to lower the exposure.

#### L (landscape)

![examples](examples-l.jpg)

The L version makes the blues darker and keeps more details in the shadows and the highlights. Usually it makes the street photos look softer even though the technical contrast is almost the same as in the standard style. It makes the sky darker, it doesn't emphasize the objects in the foreground as much. It makes the bright reflections of the sky darker, they stand out less. It adds some details to the silhouettes, they are not as inky black as before. In the result, the images tend to look softer overall.

#### F (flat)

![examples](examples-f.jpg)

The F version has the noticeable 50% mask on the `rgb curve`. It reduces the overall contrast a lot, but keeps the character. The blue tones are getting darker as well. In the result we can get more dynamic range and save the details in both the shadows and the highlights. This style is good for more old-school documentary photography.

#### FN (flat natural)

The FN style is the variant of the F style, but without any color corrections at all. It's just a flat style with the most natural color rendering.

#### LC, FC, FNC (clean)

These versions don't use the mask on the rgb curve. The contrast is reduced by the standard `contrast` slider. In the result, we lose some of the darkness in the shadows and get some contrast in the midtones instead. The images will look more detailed, more clean overall. In some cases they will increase the exposure a bit. These styles can help in the situations when the standard L, F, FN styles give us too muddy results.

*Tip: If you need to increase the exposure - consider using the `color balance rgb > global brilliance` slider instead of the one in the `exposure` module. It'll change the contrast in the relation to the exposure changes, and everything will look more natural. The standard `exposure` module works if you need to fix the overexposed areas, but if you need to make a photo a little bit brighter - it can raise the shadows too much and change the character of the photo. The `global brilliance` slider doesn't affect the shadows as much.*

### Step 3. Effects.

There are some additional effects here:

#### + extra crispy

This effect adds even more contrast to the highlights. It can be required in some cases of printing. But use it carefully - this kind of effect can create visible artifacts with outlines.

## License

CC BY 4.0

Copyright (c) 2023 Ivan Bogachev

https://instagram.com/sfi0zy
