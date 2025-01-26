# Tailwind CSS Hover Effects Not Working on Dynamic Content

This repository demonstrates a bug where hover effects in Tailwind CSS do not work correctly on dynamically rendered content.

## Description
The issue occurs when using Tailwind CSS classes on elements that are added to the DOM after the initial page load.  Hover effects, such as `hover:bg-blue-700`, do not apply to these elements.

## Reproduction
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe that the hover effect on the button only partially works. The initial render has the correct hover style, but additional renders from button clicks may not update the hover effect correctly.

## Solution
The solution involves ensuring that Tailwind CSS is able to re-process the styles after the new elements are added.  See `bugSolution.js` for a possible solution.

## Technologies Used
* React
* Tailwind CSS