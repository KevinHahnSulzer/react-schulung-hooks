# Exercise: Hooks

## Description:

**A counter that counts words.** Create a component that displays a textarea, a button, and a count of the number of words in the textarea. When the button is clicked, the count should update to reflect the number of words in the textarea.

1. The component should use `useState` to store the text that the user has entered into the textarea.
2. The component should use `useEffect` to update the word count whenever the text in the textarea changes.
3. The component should use `useMemo` to calculate the word count only when the text in the textarea changes.

## Here are the steps to complete this exercise:

1. Create a new React component called `WordCounter` that renders a `textarea`, a `button`, and a count of the number of words in the textarea.
2. Use `useState` to create a state variable called `text` that will store the text entered by the user in the `textarea`.
3. Use `useMemo` to create a memoized value called `wordCount` that calculates the number of words in `text`.
4. Use `useEffect` to update `wordCount` whenever text changes.
5. Create a function called `handleClick` that will update the `text` state when the button is clicked.
6. Add an event listener to the button that calls `handleClick` when clicked.
7. Render the `textarea`, `button`, and the count of words in the `textarea`.

## Example Output

Here's an example of what the `WordCounter` component might look like when it's working:

```html
<textarea value="This is some text."></textarea>
<button>Count Words</button>
<p>Word count: 4</p>
```

When the user changes the text in the `textarea` **and** clicks the `Count Words` button, the word count should update to reflect the new text.

Before:

```html
<textarea value="This is some different text."></textarea>
<button>Count Words</button>
<p>Word count: 4</p>
```

After clicking the button:

```html
<textarea value="This is some different text."></textarea>
<button>Count Words</button>
<p>Word count: 5</p>
```
