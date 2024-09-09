# Prework Study Guide Webpage

## Cheyenna's Pre-work study guide for U of M Coding bootcamp

The Prework Study Guide Webpage was created as a helpful resource for bootcamp students. It provides notes and essential information on key topics like HTML, CSS, JavaScript, and Git. This guide serves as a foundation for understanding these technologies and helps students prepare for the upcoming bootcamp coursework.

- The motivation behind creating this webpage was to organize and consolidate key prework topics in a structured and accessible format.
- The purpose was to assist bootcamp students in their early learning journey.
- The webpage solves the problem of needing a centralized source for prework material, allowing students to easily reference and review the topics.
- Through this project, I learned how to apply basic web development concepts and organize information effectively.

# Table of Contents

1. [Introduction](#introduction)
2. [HTML](#html)
   - [HTML Elements and Structure](#html-elements-and-structure)
   - [HTML Element Types](#html-element-types)
   - [Metadata and the `<head>` Element](#metadata-and-the-head-element)
   - [HTML Attributes](#html-attributes)
   - [Parent and Child Elements](#parent-and-child-elements)
   - [Tags vs. Elements](#tags-vs-elements)
   - [List and Image Elements](#list-and-image-elements)
   - [Anchor and Break Elements](#anchor-and-break-elements)
3. [CSS](#css)
   - [CSS Overview](#css-overview)
   - [CSS Syntax](#css-syntax)
   - [Common CSS Selectors](#common-css-selectors)
   - [CSS Box Model](#css-box-model)
   - [CSS Positioning](#css-positioning)
   - [CSS Flexbox](#css-flexbox)
   - [CSS Grid](#css-grid)
   - [Media Queries](#media-queries)
   - [Pseudo-classes and Pseudo-elements](#pseudo-classes-and-pseudo-elements)
4. [Git](#git)
   - [Git Overview](#git-overview)
   - [Common Git Commands](#common-git-commands)
   - [Working with Branches](#working-with-branches)
5. [JavaScript](#javascript)
   - [JavaScript Overview](#javascript-overview)
   - [JavaScript Syntax](#javascript-syntax)
   - [JavaScript Functions](#javascript-functions)
   - [JavaScript DOM Manipulation](#javascript-dom-manipulation)
   - [JavaScript Events](#javascript-events)
   - [JavaScript Control Structures](#javascript-control-structures)
   - [Objects and Arrays](#objects-and-arrays)
   - [Asynchronous JavaScript](#asynchronous-javascript)
6. [Conclusion](#conclusion)


## Usage

To use this Prework Study Guide, follow these steps:

1. **Review the Notes**  
   Read through the notes in each section to familiarize yourself with the material.

2. **Open Chrome DevTools**  
   For suggestions on what to study first, open Chrome DevTools by pressing:
   - **Control + Shift + I** (for Windows)
   - **Command + Option + I** (for macOS)

   A console panel will appear either below or to the side of the webpage in your browser. 

3. **Check the Console Panel**  
   In the console panel, you will see a list of topics covered in the prework, along with a suggestion on which topic to study first.

## Credits

List your collaborators, if any, with links to their GitHub profiles.

If you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.

If you followed tutorials, include links to those here as well.

## License

This project is licensed under the MIT License.

## Badges

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Code Quality](https://img.shields.io/badge/code_quality-A%2B-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Last Commit](https://img.shields.io/github/last-commit/your-username/your-repo)

## Features

- **Interactive Console**: Opens Chrome DevTools to provide suggestions on what topics to study first.
- **Comprehensive Study Guide**: Covers HTML, CSS, Git, and JavaScript, with detailed explanations and examples.
- **Responsive Design**: The study guide is designed to be accessible and usable across different devices and screen sizes.
- **Easy Navigation**: Table of contents and internal links allow users to quickly find and access specific sections.
- **Customizable**: Easily update the study guide with additional content or changes as needed.

Feel free to explore and use the features provided to enhance your learning experience and make the most of the study guide!

## Tests

**Unit Tests**: To test individual JavaScript functions, ensuring they return the expected results.
- Create test files with a .test.js extension in the __tests__ directory. 
- Use the following command to run unit tests: npm test
- JavaScript Example:
test('should return a list of topic suggestions', () => {
  const suggestions = getTopicSuggestions();
  expect(suggestions).toContain('HTML');
  expect(suggestions).toContain('CSS');
});

**Integration Tests**: To test how different parts of the study guide interact, such as the integration between the HTML structure and JavaScript functionality.
- Create test files with a .int.test.js extension to test interactions.
- npm test -- --testPathPattern=integration
- JavaScript Example:
test('should display topic suggestions in the DOM', () => {
  document.body.innerHTML = '<div id="suggestions"></div>';
  updateSuggestions();
  const suggestions = document.querySelector('#suggestions').textContent;
  expect(suggestions).toContain('HTML');
  expect(suggestions).toContain('CSS');
});
Note: Adjust the paths/or configurations according to YOUR project's setup. Ensure that you have the appropriate test files and configuration files in place for each type of test.