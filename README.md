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
