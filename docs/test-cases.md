# Test Cases

## TC-001: Successful contact form submission

### Preconditions
- Website is opened.
- Contact form is visible.

### Test Data
- Name: Jan Kowalski
- Phone: 123456789
- VIN: WAUZZZ8V4KA123456
- Message: Problem with brakes.

### Steps
1. Fill in all required fields with valid data.
2. Click "Wyślij".

### Expected Result
- Form is submitted successfully.
- Success message is displayed.
- Form fields are cleared.

---

## TC-002: Required fields validation

### Preconditions
- Website is opened.
- Contact form is visible.

### Steps
1. Leave required fields empty.
2. Click "Wyślij".

### Expected Result
- Form is not submitted.
- Validation messages are displayed for required fields.

---

## TC-003: Name field validation

### Preconditions
- Website is opened.
- Contact form is visible.

### Test Data
- Name: 12345
- Name: @#$%^&
- Name: "     "

### Steps
1. Enter invalid value into the "Imię i nazwisko" field.
2. Fill the remaining required fields with valid data.
3. Click "Wyślij".

### Expected Result
- Form is not submitted.
- Validation error is displayed for the name field.

---

## TC-004: VIN length validation

### Preconditions
- Website is opened.
- Contact form is visible.

### Test Data
- VIN: 123
- VIN: 12345678901234567890

### Steps
1. Enter VIN with incorrect length.
2. Fill the remaining required fields with valid data.
3. Click "Wyślij".

### Expected Result
- Form is not submitted.
- Validation message is displayed.
- VIN must contain exactly 17 characters.

---

## TC-005: Mobile menu behavior

### Preconditions
- Website is opened in mobile viewport.

### Steps
1. Open the mobile menu.
2. Try to scroll the background page.
3. Click a navigation item.
4. Open and close the menu several times.

### Expected Result
- Mobile menu opens correctly.
- Background page does not scroll while menu is open.
- Menu closes after clicking a navigation item.
- No layout issues are detected.

---

## TC-006: Contact links verification

### Preconditions
- Website is opened.
- Contact section is visible.

### Steps
1. Click Telegram link.
2. Click phone number link.
3. Click email link.
4. Click map link.

### Expected Result
- Telegram opens expected destination.
- Phone link opens phone application.
- Email link opens default email client with correct recipient.
- Map opens expected location.

---

## TC-007: Responsive layout verification

### Preconditions
- Website is opened.

### Steps
1. Open website on desktop viewport.
2. Open website on tablet viewport.
3. Open website on mobile viewport.
4. Check layout in landscape orientation.

### Expected Result
- Layout works correctly on desktop, tablet and mobile devices.
- No overlapping elements are detected.
- No horizontal scrolling appears.
- Text remains readable.

---

## TC-008: Basic technical verification

### Preconditions
- Website is opened.

### Steps
1. Open browser DevTools.
2. Check Console tab.
3. Reload the page.
4. Verify main internal and external links.

### Expected Result
- Page loads successfully.
- No critical console errors are displayed.
- Links do not return 404 errors.