# Filter

A group of radio buttons that lets you pick one option, hiding the rest, with a reset button to change your choice.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| filter | component | Applies to `forms` or `divs` containing radio buttons for item filtering. |
| filter-reset | part | Reset button alternative for non-form elements. |



<!-- Filtering with HTML Form: Radio Buttons and Reset Button -->
### Filter with HTML form: radio buttons and reset button

A HTML form for filtering with radio buttons and a reset option.

```html
<form class="filter">
  <input class="btn btn-square" type="reset" value="×"/>
  <input class="btn" type="radio" name="drink" aria-label="Tea"/>
  <input class="btn" type="radio" name="drink" aria-label="Coffee"/>
  <input class="btn" type="radio" name="drink" aria-label="Smoothie"/>
</form>
```

<!-- Filter without HTML form -->
### Implementing filter without HTML forms

Use this method when HTML forms are not an option.

```html
<div class="filter">
  <input class="btn filter-reset" type="radio" name="destination" aria-label="All"/>
  <input class="btn" type="radio" name="destination" aria-label="Jungle"/>
  <input class="btn" type="radio" name="destination" aria-label="Beach"/>
  <input class="btn" type="radio" name="destination" aria-label="Mountain"/>
</div>
```
