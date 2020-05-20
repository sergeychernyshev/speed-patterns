---
layout: default
title: Skeleton Designs
---
# {{ page.title }}

## TODO

- Record video examples and convert to animated GIF format to include on the page
- Find a good existing examples of websites to include (e.g. Facebook's timeline)
- Use WebPageTest to record a filmstrip illustrating successful implementation
- Use WebPageTest to record a filmstrip illustrating failure scenario, e.g. when nothing is shown or spinner is used particularly badly
- Find existing solutions for popular frameworks

skeleton desgins are a way to show progression towards a visual user experience by hinting at the content and layout to come to keep the user in an active state of mind. Another benefit is minimizing coginitive load by interpretting the visual layout of the page before the actual content arrives.

## Features

skeleton designs often include several distinct features.

### Content Types

To reduce cognitive load for the user, it is helpful to indicate the type of the content that will be displayed.

For instance, image placeholders can be made of solid blocks of color. User's avatar images are often represented with a solid color circles if thats the shape of avatars in the completed user interface.

<figure>
<figcaption>LinkedIn Skeleton Screen</figcaption>
<img src="{{ "/assets/linkedin_skeleton.jpg" | absolute_url }}" width="500" height="273" alt="LinkedIn Skeleton Screen (static)"/>
</figure>

Text can be represented as a sequence of horizontal lines to mimic headers and paragraphs.

### Boundaries / Layout Sections

When types of the upcoming content and it's positions can not be predicted reliably by the time skeleton design is displayed, it is recommended to at least identify areas of the interface where content is going to be displayed. This is often done using background color of the loaded area, logically separating it from other areas of the page.

### Pulsating Gradients

It has been proven that progress bars that use color gradients and pulsation animations are percieved faster reducing user's anxiety.

Similar techniques are often used in skeleton designs where solid colors are replaces with gradients of similar color that animate left-to-right showing percieved progression.

<figure>
<figcaption>LinkedIn Pulsating Skeleton Screen</figcaption>
<video controls width="500" alt="LinkedIn Skeleton Screen pulsating" autoplay loop>
    <source src="{{ "/assets/linkedin_skeleton.mp4" | absolute_url }}" type="video/mp4">
    Sorry, your browser doesn't support embedded videos.
</video>

</figure>

## The challenges of skeleton degisgn

- understanding the content that will be loaded
- dynamic data-driven layouts / user generated content
- content types, images vs text
- indicating areas of interaction and focal points

## Examples

- Facebook timeline
- LinkedIn timeline
- YouTube video list
- [ios loading screen guidelines](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/launch-screen/)

## Replacing Existing Solutions

Why we recommned skeleton designs over the alternatives:

- `spinners` don't provide layout hints to the user and don't show progression as they revert the state after every spin
- `blank screens` don't provide any hints of visual progress and indicate pure delay (bad)
- `loading bars` while better than spinners in showing progression, still do not provide layout hints

## Related patterns

- [immutable layout](immutable_layout.html)
- no spinners

## Resources

- [Mobile Design Details: Avoid The Spinner](https://www.lukew.com/ff/entry.asp?1797) by Luke Wroblewski
- [Everything you need to know about skeleton screens](https://uxdesign.cc/what-you-should-know-about-skeleton-screens-a820c45a571a) by Bill Chung
