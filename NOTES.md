# Candidate notes

Add any notes here you'd like for reviewers to see in regard to your challenge submission.

## General Questions

- What's the goal of this component?
    - Who is it for? 
    - What is it for? 
    - When is it used? 
    - Where is it being used? 
    - Why is it being used (what problem does it solve)?
- Would this entire component be a clickable link?
- Should the elements inside the "Meta Links" be actual links?
- Is this component considered self-contained?
- What browsers should be supported? Will there be IE support? 
- What's the expectation for the mobile design?

## Assumptions

- This is a reusable, self-contained widget/component.
- It should be accessible.
    - Should use proper semantic tags.
    - Interactable elements should be tabbed through.
    - Interactable elements should have a prominent outline.
    - Decorative icons should be hidden
- Entire component isn't clickable
    - Location is a link to a Zoom address
    - More options icon button would present more options on click.

## Additional Notes

Given the above questions and assumptions, I decided to make this component out of an `<article>` element since it seems to be a self-contained and reusable component. According to caniuse, flexbox is widely supported in all major browsers and makes it simple to align content within the component.

In addition, and to make this component more accessible, I added a more prominent focus outline to the Zoom link and the More Options button, added an `.sr-only` class to the More Options button text to visually hide it, and added `aria-hidden=true` to the decorative SVGs.

Just for the purposes of fulfilling the challenge and because there's no additional content, I decided to hardcode the component `width`. This is not something I'd normally do in most cases, but I feel it's necessary to call it out here.

Finally, I decided to try my hand at mobile styling for the component just to give an idea of what it could look like. Unfortunately, I am not a designer.