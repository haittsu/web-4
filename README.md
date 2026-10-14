# Assignment 4: Forms and Validation

This project demonstrates HTML forms, native HTML5 validation, and Bootstrap
form styling. It follows the three parts of Assignment 4: Basic HTML Forms,
Bootstrap Forms, and an Advanced Form Project.

## Tasks

| Part | Task | Page | Description |
| --- | --- | --- | --- |
| Basic HTML Forms | 0. Simple Contact Form | [index.html](index.html) | Name, email, message, and a Submit button with labels for every field. |
| Basic HTML Forms | 1. Form with HTML5 Validation | [task1.html](task1.html) | Contact form with required fields, email format validation, and maximum lengths. |
| Bootstrap Forms | 2. Bootstrap Form Styling | [task2.html](task2.html) | Contact form styled with Bootstrap form classes, a responsive grid, placeholders, and helper text. |
| Bootstrap Forms | 3. Bootstrap Validation Styles | [task3.html](task3.html) | Interactive validation feedback and fixed examples of the `is-valid` and `is-invalid` classes. |
| Advanced Form Project | 4. Registration Form | [task4.html](task4.html) | Registration fields, Bootstrap Grid, HTML5 validation, feedback messages, and Submit and Reset buttons. |

Every page includes navigation links to all five tasks.

The registration form includes first name, last name, email, password, password
confirmation, gender radio buttons, optional hobby checkboxes, and a country
dropdown.

## Technologies

- HTML5 for page structure, form controls, and built-in validation.
- Bootstrap 5.3.8 CSS, loaded from the jsDelivr CDN, for Tasks 2–4.

The project uses no JavaScript, package manager, or build tools.

## How to Run

1. Download or clone the repository.
2. Open `index.html` in a web browser.
3. Use the navigation links to open the other tasks.

An internet connection is needed to load Bootstrap CSS on Tasks 2–4.

## How Validation Works

HTML5 attributes define the rules checked by the browser:

- `required` prevents submission when a mandatory field is empty.
- `type="email"` checks the format of an email address.
- `maxlength` limits the length of text fields.
- `minlength="8"` requires at least eight characters in both password fields.

In Task 1, the maximum lengths are 80 characters for the name, 254 for the email,
and 1,000 for the message. The browser blocks invalid submissions and displays
its own validation messages.

Tasks 3 and 4 use `was-validated` on the form. Bootstrap styles the browser's
`:valid` and `:invalid` states and displays `valid-feedback` or
`invalid-feedback` below the fields. Feedback is enabled from page load and
updates as values change. Task 3 also shows fixed, disabled examples using
`is-valid` and `is-invalid`.

The forms are frontend demonstrations with no backend to process submissions
or create accounts. Password confirmation is required and checked for minimum
length, but matching the two passwords is not implemented. Comparing two fields
requires JavaScript or server-side validation.

## Manual Testing

1. In Task 1, submit an empty form and check that required fields block submission.
2. Enter `not-an-email`, then `alex@example.com`, to compare invalid and valid email formats.
3. Check the maximum text lengths in the contact form.
4. In Task 3, fill and clear fields to observe error and success feedback.
5. In Task 4, try a password shorter than eight characters, then one with at least eight characters.
6. Check that Task 4 requires a gender and country, allows multiple hobbies, and clears the form with Reset.
7. Resize the browser: Bootstrap grid fields should stack on narrow screens and share rows on wider screens.

## Submission

The assignment requires publishing the project with GitHub Pages or Netlify and
submitting the GitHub repository link by the deadline specified in Moodle.
Students must also defend the assignment during the practice lesson and explain
the HTML, Bootstrap classes, and validation behavior.

## Assignment Resources

- [Bootstrap Getting Started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [Bootstrap Forms](https://getbootstrap.com/docs/5.3/forms/overview/)
- [MDN Web Forms](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms)
- [HTML Form Attributes](https://www.w3schools.com/html/html_form_attributes.asp)
