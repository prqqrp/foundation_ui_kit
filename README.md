# Foundatin UI Kit

Foundation is a toolbox for Sketch that helps designers quickly compose robust user interfaces using flexible components and interchangeable libraries.

## Core libraries for type, color, and icons
Foundation decouples basic libraries from your main design document to make it easier to adapt the design system to different branding or visual styles. Rather than rebuilding a button component for every new project, use the "Button" element from Foundation and skin it to your styling via the overrides.  This means designers can focus on creating experiences, not components.  You can also leverage Sketch's file versioning and history to track changes specific to each color, type, and element library, too.

## Scaling small parts
Since each library governs an aspect of the design system, it's easy to swap out parts with project-specific design elements. If you need a custom set of branc colors, just make a new document called "brand_colors.sketch" and add some swatches that are 200px x 100px.  Save it as a library and Sketch will automatically find those and allow you to swap them into the Foundation design elements.  You can even add those swatches to your sketch file as a symbol, instead of using a library, to save some steps.  Overall, this reduces large-file redundancies as designers only add to the existing libraries instead of cloning them.

## Flexible design elements
Most UI elements are made of basic shapes that mask an imported color swatch.  Any text references an external type library, and icons are from the icon library.  This approach offers 2 key advantages:

1. It gives designers a single source of truth for building a library of design elements.  No more copy / pasting Sketch files and hoping you have the latest updates... everything in Foundation can be shared across a larger design system or organization to ensure teams are always using the same version of a kit.

2. The elements can be overridden when instanced to use external type, color, and icon libraries.  So if a designer wants to go rogue, they can, and none of the symbils will break (or even pass changes upstream to the master system).  This gives each element limitless flexibility.

## An improvement to using document symbols
Foundation lets designers spin up an application design without having to create a single symbol in their design file. Rather than green-fielding new components each time, designers can simply import an element, modify it's properties to their needs, and get to designing.  Imported symbols are nice because they won't clone themselves accidentally when you duplicate or copy / paste an artboard (if it's happened to you once you know how scary it is to untangle repeated symbol parents in Sketch).

Alternatively, if you don't want to copy / paste symbols around your document you can still import an element from the library, change all of the overridden properties to suite your app, then save THAT as a symbol in your document.  This creates a "preset" of sorts that you can reference any time in your design and you won't need to bother with changing the overrides again.  You can also "lock" specific attributes of this symbol so you don't accidentally change the text-style or background color.

## More great features of Foundation:

- Smart symbols that scale and resize as expected
- Emoji override names for easy updates
- Solid, opacity steps, gradients, and photo fills for _Color components
- Basic type scale with dark, light, and primary colors (Open Sans required)
- Material Design (Rounded) Icon library pre-configured to use _Colors fill
- Robust library of common UI elements including buttons, inputs, toggles, lists, chips, selectors, map pins, tabs, ratings, links, pagination, and more
- Stock iOS and Android mobile design elements for headers and navigation

Unlike other design kits on the market, Foundation won't give you a skeleton banking app out of the box. It isn't designed to be an instant Dribble portfolio, either. This toolbox is meant to give designers an awesome grab-bag of parts to start building their own interfaces - without all the tedium of making components and symbols every time.

Foundation is also a fantastic addition to any design system, offering governance around key elements like color, type, and iconography that can be iterated on without breaking the consuming design components. It's also free, because why not. Download it now!

# Installation

0. Install the Open Sans font (included) as provided by Google.

1. Move the contents of this folder to a safe place, something like...
> ⁨Macintosh HD⁩/⁨Users⁩/your_name/Library⁩/Application Support⁩/com.bohemiancoding.sketch3⁩/Libraries

2. Open sketch

3. Open _Colors.sketch first!  Go to File > Add as Library...

4. Open _Type.sketch second! Go to File > Add as library...

5. Open _Icons.sketch third! Go to File > Add as library...

6. Open _Elements.sketch fourth! Go to File > Add as library...


# The libraries

## Colors
The \_Colors.sketch file gives you access to a robust mixture of symbols for any situation. These are best used when you need a block of color somewhere in your design. Specifically these symbols are used as fills for icons, buttons, border shapes, radius shapes, etc in all the other library files.

\_Colors.sketch includes a swath of traditional color chips for system colors and a primary palette.  It also features a combo swatch using 10% opacity steps from 0-90%.  The main swatch can be exchanged for any other swatch in the library.

There are also gradient fils that use an alpha mask from a foreground color to background color, using radial and linear gradients of various orientations.

\_Colors.sketch includes a photo fill, as well.  Any symbol can be used in another, allowing designers to create a dazzling amount combinations of color, fades, and photos.

If you want to use your own colors just make a new symbol in the library, in another library, or directly in your file, and make it 100px tall by 200px wide. Then, anywhere a color chip is used you can swap out to use your symbol instead.  Easy.

## Type
There's a big ol' \_Type.sketch file included which has a massive type scale set up by default.  It includes a hierarchy of type with light, dark, and primary color variations.  Each has been saved as a text style and can be imported / used in any symbol or document that has text.

If you want to change any of the text styles simply select the sample, change the properties, then in the text styles dropdown select "update text style", then save the document.  Now any other file that consumes a text style from this page will get a purple badge noting the update.  Once your update is applied the new text will appear.

You can update ALL the text if you'd like.  For instance, you can select all of the primary colored text and change the color value.  Then select "update text styles" from the overrides panel and BOOM, every piece of primary colored text will be saved for consumption.  You can also add new text styles fairly easily by typing some text, changing the values, and saving the text style to this document.

## Elements
The \_Elements.sketch file is where the meat of the system is.  This includes list items, buttons, form fields, combos of photos and text styles, combo shapes as fill and outlines, chips and pills, nav tabs, tab bars, stock OS components for Android and iOS, map markers, pagination... and more.

The secret sauce here is how the \_Elements.sketch symbols work with the other libraries. Any symbol that uses an icon references the \_Icons.sketch library.  The referenced icon can be swapped out for any other symbol that's 24px x 24px, from any other sketch library (or symbols in the design document). Icons have a fill driven by the \_Colors.sketch library so you can govern all the fills in one place and swap them out at your convenience.  You can also use the gradients, opacity, and photo color symbols as fills for your icons.

\_Elements.sketch has a whole mess of basic shapes that let you use border or solid fills anywhere in your design (like cards, text inputs, photo fills, etc.).  I've taken extra steps to offer radius version of both fill types, including 4px, 8px, 16px, and 24px radius options.  I went a step further by offering single-corner rounding and offset rounding.  This means you can create a text input with squared edges and an outline, and a button element with rounded corners and solid fill, using the same set of shape overrides.  Nearly every symbol in this library is comprised of a shape with a fill color, a text style, and an icon.

# Getting started

You probably don't live in my brain, so getting started may not seem super easy to you.  I've outlined some basic instructions below to get you going.  It covers how to use the symbols, save overrides, and customize the elements to suit your app needs.  As time permits I hope to add more detailed usage instructions or videos.

First, I recommend creating a folder for your project.  Name it accordingly.

Inside make a new Sketch file and name it (projectName)\_Colors.sketch. Create your project color palette here by drawing some rectangles that are 100px tall by 200px wide.  Each rectangle should be on it's own artboard.  Change the fill of your rectangle to be the branding color you need.  Select the artboard for your rectangle and choose "create symbol" from the menu.  Name it accordingly "brand/primary", "brand/secondary", "brand/a11y", etc.  Save your document as a library via file > add as library.

> Why a library?  So it can be abstracted from your app design, and potentially used by other projects or app designs.

The default type is "Open Sans" font.  If you want to use your own font follow these steps.

Grab the \_Type.sketch file and copy it from your library directory.  Paste it into the new project folder and rename it to (projectName)\_Type.sketch.  I've provided some common type styles, alignments, and colors.  You can select ALL of the texts on the page and globally change to a new font family using the inspector on the right.  Once updated click the style overrides dropdown and choose "update all styles".  Save this document and add it as a library.  Now you can use the default "Open Sans" type or your "branded" type.  Any element that you import into your design file later will reference the default text, so you will simply need to select the override element, go to text style, and choose your library's text style instead.  Easy to update.

Make one last sketch file for your app in that directory, calling it (projectName).sketch or something similar.  That file is where you'll be whipping up your app design.  Go to "insert" > \_Elements > pick something like a list item.  Add it to your artboard. Modify the overrides in the inspector, swapping out color fills, icons, fonts, etc.  Once you're in that file and adding elements you will hopefully get the gist of how easy it is to start designign an app.

Once you get a symbol setup the way you like it just save this as a symbol in your actual sketch file. This creates a snapshot of your overrides and allows you to freeze any attribute that you don't want messed with (like type face, fills, icons, etc.).  The end result is a symbol crafted to your taste and app needs, that is easily saved for selective overriding throughout your design.  It takes longer to read this set of instructions than it does to actually get things working.

The point of all this is making it easier to whip up some UI components tailored to your app without wasting all your time figuring out how to build the right symbol for the occasion.  You just grab a symbol, swap some properties, then save it to your doc for easy updates.  And you can use all the same symbols for all your projects by changing how you overrride the instances.  Gone are the days of creating button after button after button for your project - setting up the symbols with snapping and positioning so they scale properly, adding icons, setting document colors, updating document colors.  Use Foundation, design something great, and ship it.

