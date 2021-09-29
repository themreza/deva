# Text Contrast

## Description

The color contrast ratio between the background and foreground text should be:

* 4.5:1 for body text
* 3:1 for large text, active user interface components, and graphical objects like icons and graphs

An enhanced contrast ratio ensure better accessibility:

* 7:1 for body text
* 4.5:1 for large text

More information:

* https://web.dev/color-and-contrast-accessibility/
* https://developer.mozilla.org/en-US/docs/Web/Accessibility/Understanding_WCAG/Perceivable/Color_contrast
* https://colourcontrast.cc/

## Valid Examples

* https://web.archive.org/web/20210927123418/https://www.amazon.com/

![](valid-1.jpg)

## Invalid Examples

* https://web.archive.org/web/20210927233500/https://decalonz.wixsite.com/decalonzgraphicz

![](invalid-1.jpg)

## Element Detection

The design should be scanned for textual elements, ideally of any language.

If possible, the relative sizes of textual elements should be identified with respect to the overall design.

## Technical Implementation

Using the stroke width transform method, it is possible to create bounding boxes around pieces of text in an image.

### Example (Needs Improvement) 

#### Original Image

![](orig_img.png)

#### Stroke Width Transform

![](swtpruned3C_img.png)

#### Stroke Width Transform Pruned and with Bounding Boxes

![](swtpruned_bbox.png)

### More information: 

* https://web.archive.org/web/20210929005209/http://www.math.tau.ac.il/~turkel/imagepapers/text_detection.pdf
* https://github.com/marrrcin/swt-python
* https://github.com/ag-ds-bubble/swtloc