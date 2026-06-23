# Bug Reports

## BUG-001

### Title
Background page can be scrolled when mobile menu is open.

### Environment
- Chrome
- Mobile viewport (iPhone SE)

### Steps to Reproduce
1. Open the website.
2. Open mobile menu.
3. Try to scroll the page behind the menu.

### Actual Result
The background page can be scrolled while the mobile menu is open.

### Expected Result
Background scrolling should be disabled while the mobile menu is open.

### Severity
Low

### Priority
Medium

### Status
Closed

### Retest

**Retest Result:**
PASS

**Notes:**
Mobile menu was retested after the fix. Background page scrolling is disabled while the mobile menu is open.



## BUG-002

### Title

Name field accepts invalid characters.

### Environment

- Chrome
- Desktop

### Steps to Reproduce

1. Open the website.
2. Navigate to the contact form.
3. Enter special characters into the "Imię i nazwisko" field (e.g. @#$%^&*, 12345, "     ").
4. Fill the remaining required fields with valid data.
5. Click "Wyślij".

### Actual Result

The name field accepts special characters as a valid value and does not display a validation error.

### Expected Result

The name field should reject special characters and display a validation error. Only valid name characters should be accepted.

### Severity

Medium

### Priority

Medium

### Status

Closed

### Retest

**Retest Result:**
PASS

**Notes:**
Name field validation was retested after the fix. Numeric characters, special characters and invalid name values are rejected correctly.


## BUG-003

### Title
Email link contains outdated email address.

### Environment
- Chrome
- Desktop
- Production website

### Steps to Reproduce
1. Open the website.
2. Navigate to the contact section.
3. Inspect or copy the "Napisz e-mail" contact link.

### Actual Result
The email link uses the outdated email address:
`autoserwis.som@gmail.com`.

### Expected Result
The email link should use the current business email address.

### Severity
Medium

### Priority
High

### Status
Closed

### Retest

**Retest Result**
PASS

**Notes:**
Email link was retested after the fix. The default email client opens correctly and the recipient field contains the correct email address.