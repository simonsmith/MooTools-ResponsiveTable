# MooTools ResponsiveTable

Port of Filament Group's [Responsive Table jQuery plugin](http://filamentgroup.com/examples/rwd-table-patterns/). Allows a default set of columns to be shown at different screen sizes and enables user to toggle them with a display menu.

jsfiddle demo: [http://jsfiddle.net/Blink/kZUg8/](http://jsfiddle.net/Blink/kZUg8/)

## Usage

### Arguments
- - -

```js
new ResponsiveTable(table, options);
```

1. **table** - _(mixed)_ String selector or an Element referencing the table
2. **options** - _(object, optional)_ A key/value object for options

### Options
- - -

* **classes** - _(object)_ CSS Classes
	* **enhanced** - _(string)_ Applied to the table when an instance is created _default_ `enhanced`
	* **persist** - _(string)_ If present, the Class ignores this column and always shows it _default_ `persist`
 	* **colHidden** - _(string)_ Applied when a column is hidden by a checkbox _default_ 'col-hidden'
  	* **colVisible** -  _(string)_ Applied when a column is shown by a checkbox _default_ 'col-visible'

* **displayMenu** - _(object)_ Options for the element that contains the display checkboxes
	* **linkText** - _(string)_ Text used in the link _default_ `Display columns`
	* **position** - _(string)_ Where the display menu is injected in relation to the container _default_ `top`
* **checkInputEvents** - _(array|string)_ The state of the display menu checkboxes are checked against these events _default_ `['orientationchange', 'resize']`

### Events
- - -

* **checkInputState** - _(function)_ Checkbox state has been checked when a resize event fires
* **displayMenuToggle** - _(function)_ Display Menu is toggled
