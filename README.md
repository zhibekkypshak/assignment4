# Assignment #4. Forms and Validation

**Student:** Zhibek Kypshak 
**Group:** SE-2528   
**Repository:** https://github.com/zhibekkypshak/assignment4.git

## About the project

A multi-page website that demonstrates how to create user-friendly forms with HTML and style them with Bootstrap 5.3. It also shows two ways of form validation: built-in HTML5 validation and Bootstrap validation classes.

A **navbar** on every page links to all tasks.

## Pages and tasks

| Page | Task | Description |
|------|------|-------------|
| `index.html` | Task 0 | Simple contact form: Name, Email, Message, Submit. Every field has a `<label>`. |
| `html-validation.html` | Task 1 | HTML5 validation with `required`, `type="email"`, `minlength` and `maxlength`. |
| `bootstrap-form.html` | Task 2 | The same form styled with Bootstrap: `form-control`, grid (`row`, `col-md-6`), placeholders and helper text (`form-text`). |
| `validation.html` | Task 3 | Bootstrap validation styles: `is-valid`, `is-invalid`, `valid-feedback`, `invalid-feedback` with messages such as "Looks good!" and "Email is required". |
| `registration.html` | Task 4 | Registration form: First Name, Last Name, Email, Password, Confirm Password, Gender (radio), Hobbies (checkboxes), Country (select), Submit and Reset. |

## Features

- Responsive layout with the Bootstrap grid and custom media queries (desktop, tablet, phone)
- HTML5 validation attributes: `required`, `type`, `minlength`, `maxlength`
- Bootstrap validation feedback (green and red states with messages)
- Password and Confirm Password match check
- Reset button clears the form and the validation highlighting
- Custom CSS: gradient navbar, card design, focus effects, hover animations

## Project structure

```
assignment4/
├── index.html
├── html-validation.html
├── bootstrap-form.html
├── validation.html
├── registration.html
├── css/
│   └── style.css
├── js/
│   └── script.js
└── README.md
```


## How validation works

1. **HTML5 validation.** The browser checks the attributes (`required`, `type="email"`, `minlength`, `maxlength`) and shows its own messages (Task 1).
2. **Bootstrap validation.** The form has `novalidate` and the class `needs-validation`. On submit, `js/script.js` checks `form.checkValidity()` and adds the class `was-validated`. Bootstrap then colours the fields and shows `valid-feedback` or `invalid-feedback` (Tasks 3 and 4).
3. **Password match.** `setCustomValidity()` marks Confirm Password as invalid when it differs from Password.

## Technologies

- HTML5
- CSS3 (custom styles + media queries)
- Bootstrap 5.3.3 (CDN)
- JavaScript (a few lines for validation)
- Git and GitHub Pages

## Resources

- [Bootstrap 5.3 Forms](https://getbootstrap.com/docs/5.3/forms/overview/)
- [MDN: Web forms](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms)
- [W3Schools: HTML form attributes](https://www.w3schools.com/html/html_form_attributes.asp)
```

