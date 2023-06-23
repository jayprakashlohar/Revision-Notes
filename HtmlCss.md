### HTML AND CSS

## How do you add CSS to an HTML webpage?

CSS can be added to an HTML webpage in one of three ways.

1. External CSS: This involves linking an external stylesheet to the HTML document. This is done by adding a <link> element to the <head> section.
2. Internal CSS: This involves adding CSS directly to the HTML document by using the <style> element in the <head> section.
3. Inline CSS: This involves adding CSS directly to an HTML element by using the style attribute.

## What does CSS stand for?

CSS stands for Cascading Style Sheets.
CSS stands for Cascading Style Sheets.
## What does HTML stand for?

HTML stands for Hypertext Markup Language.

## What are the features of HTML5?

1. Improved Semantic Elements: HTML5 offers new semantic elements like <header>, <footer>, <article>, <section>, <nav>, <figure>, <figcaption>, <aside>, <main>, etc.

2. Canvas: HTML5 provides a <canvas> element which is used to draw graphics on the fly via scripting (usually JavaScript).

3. Video and Audio: HTML5 provides a <video> and <audio> element for media playback.

4. Geolocation: HTML5 makes it easy to track user's location using JavaScript.

5. Drag and Drop: HTML5 makes it easy to drag and drop the element on the web page with the help of JavaScript.

6. Web Storage: HTML5 provides a client-side storage mechanism which is more secure and faster than the traditional cookies.

7. WebSocket: HTML5 introduces the WebSocket protocol which enables the client to communicate with the server in real time without any delay.

8. Microdata: HTML5 provides a mechanism for adding machine-readable data to a web page.

## What are the different types of storage in HTML5?

1. Local Storage
2. Session Storage

## What do the following mean in html

<section> - defines a section in a document, usually containing a group of related elements
<article> - defines an independent, self-contained content
<footer> - defines a footer for a document or section
<nav> - defines a section of navigation links
<aside> - defines content aside from the content it is placed in, usually related to the content nearby

## What are forms in HTML?

Forms are elements in HTML that allow users to enter data into a web page. Forms are typically used to gather information from a user, such as a name, address, or credit card information. Forms consist of various elements, such as text fields, checkboxes, radio buttons, dropdowns, and submit buttons, that allow users to enter and submit this data.

## What are event listeners in HTML?

Event listeners in HTML are attributes that can be added to HTML elements to define a function that will be executed when a certain event is triggered. For example, an event listener can be used to respond to a mouse click, a key press, or a form submission.

## What are event listeners in HTML?

Event listeners in HTML are attributes that can be added to HTML elements to define a function that will be executed when a certain event is triggered. For example, an event listener can be used to respond to a mouse click, a key press, or a form submission.

## what is onload event?

The onload event is a JavaScript event that occurs when the entire page has finished loading. It is commonly used to perform tasks that need to be done after the page has loaded, such as setting up the page or making Ajax requests.

## What is scroll event?

A scroll event is an event that is triggered when a user scrolls an element on a web page. The scroll event is typically used to update content on the page, such as loading more content when a user scrolls to the bottom of a page.

## How do you use Geo Location API?

The Geolocation API is accessed via a call to navigator.geolocation; this will cause the user's browser to ask them for permission to access their location data. If they accept, then the browser will use the best available functionality on the device to access this information (for example, GPS).

## How do you know if a user is offline or not? What API does the browser provide for that?

The best way to determine if a user is offline or not is to use the navigator.onLine property of the browser's window object. This property is a boolean value that will indicate if the browser is online or offline. The navigator object is part of the Web API provided by the browser, and it provides a way for web pages to access information about the browser and its environment.

## How do you use Video and Audio tags?

Video:
<video width="640" height="360" controls>

  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Audio:
<audio controls>

  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

### CSS

## What are CSS selectors?

CSS selectors are used to "select" an element or set of elements in an HTML document to apply style rules to them. Selectors can range from simple element selectors such as "p" to more complex combinations of elements, classes, and IDs.

## What are CSS variables?

CSS variables are an advanced feature of CSS that allows developers to define custom variables and values that can be reused throughout the stylesheet. They are a powerful tool for creating dynamic and reusable styles, allowing developers to easily change values in one place and have the changes cascade throughout the stylesheet.

## What is the difference between position absolute and relative?

Position absolute is an element's position relative to its containing block. It is removed from the regular flow of the page and is not affected by other elements on the page.

Position relative is an element's position relative to its normal position. It is affected by other elements on the page and is part of the normal flow of the page.

## What is Box Model?

The Box Model is a way of visualizing the elements on a web page. It is composed of four elements: margin, border, padding, and content. The margins create a space around the element, the border surrounds the content and padding, and the content is the actual content of the element. The box model can be used to define the size, layout, and spacing of elements on a web page.

## What is a flex-box?

A flex-box is a layout mode in CSS that allows elements to be laid out in any direction and to respond dynamically to the available space. It provides a more efficient way to lay out, align, and distribute elements on a page, and makes it easier to create a responsive design.

## What does justify-content, justifyItems, justifySelf mean?

Justify-content: This CSS property defines how the browser distributes the space between and around content items along the main-axis of a flex container. It helps to align the items on the main-axis of the current line of a flex container.

Justify-items: This CSS property defines how the browser distributes space between and around all items on the main-axis of a flex container. It helps to align the items on the main-axis of the flex container, even if the items have different sizes.

Justify-self: This CSS property defines how a single item is aligned on the main-axis of a flex container. The alignment of individual items can be different from the alignment of the other items in the flex container.

## What does justify-content, justifyItems, justifySelf mean?

Justify-content: This CSS property defines how the browser distributes the space between and around content items along the main-axis of a flex container. It helps to align the items on the main-axis of the current line of a flex container.

Justify-items: This CSS property defines how the browser distributes space between and around all items on the main-axis of a flex container. It helps to align the items on the main-axis of the flex container, even if the items have different sizes.

Justify-self: This CSS property defines how a single item is aligned on the main-axis of a flex container. The alignment of individual items can be different from the alignment of the other items in the flex container.

## What do AlignItems, AlignContent, and AlignSelf mean?

AlignItems is a property of the Flexbox layout, which is used to align the items within a container along the cross axis. AlignContent is a property of the Flexbox layout which is used to align the lines within a container along the cross axis. AlignSelf is a property of the Flexbox layout which is used to override the parent container's AlignItems setting for a specific item.

## What are grids?

Grids are a system of intersecting vertical and horizontal lines that are used to structure content on a page or screen. They can be used to organize the layout of elements and help make a page look more balanced and visually appealing. Grids can be used to create complex page layouts and to give a page a consistent look and feel.

## What are the differences between Flex and Grids?

Flex and Grid are both layout tools used in web design, though they have different capabilities.

Flex is a layout tool that uses a flexible box model to arrange elements on a page. It is great for quickly creating simple layouts with minimal effort. Flex elements can be stacked vertically or horizontally, and can also be re-sized and re-positioned easily.

Grid is a two-dimensional layout tool that divides a page into columns and rows. It is great for creating complex layouts with more control over the placement and sizing of elements. Grid elements are organized into columns and rows, and can span multiple columns and rows. Grid is also more suited for responsive design, allowing elements to be rearranged and re-sized based on the size of the screen.

## What is specificity, and how do you calculate it?

Specificity is a measure of how well a classifier can distinguish between different classes. It is calculated by taking the number of true positives (TP) divided by the number of true positives plus the number of false positives (TP + FP). This gives a ratio between 0 and 1, where 1 indicates a perfect score and 0 indicates a very poor score.

## What are media queries?

Media queries are a feature of CSS that allows a webpage to adapt its layout, content, and styling to different screen sizes, resolutions, and orientations. They allow for more responsive web design, allowing for a more consistent user experience across different platforms, browsers, and devices.

## What is the difference between min-width and max-width in media queries?

Min-width is used to set the minimum browser width that a style will apply to. It is used to create responsive designs that display properly on different screen sizes. Max-width is used to set the maximum browser width that a style will apply to. It is used to create responsive designs that display properly on different screen sizes.

## What are animation and keyframes?

Animation is the process of creating the illusion of motion and change by displaying a series of still images in rapid succession. Keyframes are specific points in time within an animated sequence that define the start and end points of a change. Keyframes are used to control the timing and values of specific changes, such as position, scale, rotation, and color.

## What are SVGs?

SVGs (Scalable Vector Graphics) are a type of image file that uses mathematical equations to draw shapes, lines, and curves, rather than using a grid of pixels like a JPEG or PNG. This allows them to be scaled up or down without losing any quality, making them ideal for use in web and mobile applications.

## How do you animate SVGs?

To animate SVGs, you can use a combination of CSS, JavaScript, and the SVG animation elements such as <animate>, <set>, and <animateTransform>. CSS can be used to apply motion effects to an SVG, such as rotation, scaling, and translation. JavaScript can be used to control the animation, such as setting the duration or timing functions for the animation. SVG animation elements can be used to animate specific SVG attributes, such as the x, y, width, height, and fill attributes.


