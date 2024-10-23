[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=16682051)
# Code Challenge 12: React Signup Widget

### Getting Started

Install dependencies:

```bash
npm install
```

Start the server on http://localhost:3000:

```bash
npm run dev
```

Run unit tests:

```bash
npm test
```

Run e2e tests:

```bash
npm run test:e2e
```

### Linting & Formatting the Code

```bash
npm run lint
npm run format
```

### Your task

1. Complete the **Signup Widget** component: `src/components/Signup Widget/Signup Widget.jsx`.
2. Style the **Signup Widget** component using CSS: `src/components/Signup Widget/Signup Widget.css`.

#### **Signup Widget Component Properties**

Implement the Signup Widget component to accept the props below:

```js
Widget.propTypes = {
  title: PropTypes.string.isRequired,
  content: PropTypes.string.isRequired,
  simulateNetworkRequestTime: PropTypes.number,
};
```

Set default values for the props using `defaultProps`:

```js
SignupWidget.defaultProps = {
  simulateNetworkRequestTime: 2000,
};
```

#### **Signup Widget Component Behavior**

**Form Submission:**

- The widget includes a subscription form with an email input field and a "Join" button.
- Users can input their email address in the input field.
- When users click the "Join" button, the form is submitted.

**Form Validation:**

- Email Validation: The component performs basic email validation to ensure that a valid email address is entered.
- If an invalid email format is provided, a message will be displayed, and the submission will be prevented.

**Form Submission Handling:**

- Upon successful form submission (valid email entered and "Join" clicked), the component simulates a network request by
  displaying "Joining..." and waiting for 2 seconds (simulating a response from a server).
- After the simulated request is complete, a success message will be displayed, acknowledging the user's subscription.
- The email input field will be disabled during the submission process.

**Loading State:**

- The "Join" button is disabled during the form submission process to prevent multiple submissions while waiting for a
  response.
- While the button is disabled, it displays "Joining..." to indicate that the submission is in progress.

### Signup Widget Component Styling

Apply CSS styling to the Signup Widget component to ensure it has the appearance described below:

**Form Structure and Styling (`signup-widget`):**

- `display`: Set to `flex` with a `flex-direction` of `column` to create a vertical layout.
- `padding`: Apply `24px` of padding to create spacing inside the widget.
- `border`: Add a `1px` solid border with a color of `#e0e0e0` to create a border around the widget.
- `border-radius`: Set to `6px` for slightly rounded corners.
- `box-shadow`: Apply a subtle box shadow with a value of `0 0 10px 0 rgba(0, 0, 0, 0.1)` for depth.
- `width`: Set to `100%` to make the widget responsive within its container.
- `max-width`: Limit the maximum width to `420px` to control the widget's width.
- `row-gap`: Add `12px` of spacing between rows.

**Widget Title (`h2`):**

- Use the `h2` element.
- `font-size`: Set to `24px`.
- `font-weight`: Set to `bold`.
- `color`: Use `#333`.

**Widget Description (`p`):**

- `font-size`: Set to `16px`.
- `color`: Use `#777`.

**Input Row Styling (`input-row`):**

- Set `display` to `flex` with a `flex-direction` of `row` to arrange elements horizontally.
- Add `column-gap` of `16px` to create spacing between input elements.

**Email Input (`input`):**

- `padding`: Apply `10px` of padding for comfortable input.
- `border`: Add a `1px` solid border with a color of `#e0e0e0`.
- `border-radius`: Set to `6px` for slightly rounded corners.
- Use `flex: 1` to make the input expand to fill available space.

**"Join" Button (`button`):**

- `padding`: Apply `2px` of vertical padding and `24px` of horizontal padding.
- `width`: Set to `42px` for an appropriate button width.
- `text-align`: Center the button text.
- `border-radius`: Set to `6px` for slightly rounded corners.
- `background-color`: Use `#4CAF50` as the background color.
- `color`: Set text color to white.
- `line-height`: Adjust to `16px`.
- `font-size`: Set to `14px`.
- `cursor`: Use the pointer cursor for interaction.

**Button Hover Effect (`button:hover`):**

- Change the `background-color` to `#45a049` on hover.

**Button Disabled State (`button:disabled`):**

- Set `opacity` to `0.7` to make it semi-transparent.
- Change the cursor to `not-allowed`.

---

## Preview

![Preview](https://github.com/Ensign-College/CS220-CC-12/assets/4071288/26654e86-be8b-4244-abaa-deff30a3ff3c)


