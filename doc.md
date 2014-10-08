This simple application shows the use of a custom element where list data is
searchable. The demonstrates the following parts of Polymer:

- defining custom elements
- the <template> tag
- HTML imports
- data binding

The `<searchable-list>` element uses data binding to implement search. See the
`searchable_list.html` and the `searchable_list.dart` files for the code.

The `SearchableList` class uses three variables in the search implementation:

- `data` stores all the data in the list
- `searchParam` stores the search parameter
- `results` stores the elements of data that match the search paramater
When the user types in the search input, the `search()` method triggers, and the
value of `results` updates. Since `results` is an observable variable, its
representation in the UI automatically updates as its contents change.

Here is the minimal code for required to implement search
(searchable_list.dart):

IMPORT('repo/web/searchable_list.dart', 'search)

Any changes to searchParam trigger `search()`. Here is the code for that
(the `enteredView()` method in `searchable_list.dart`):

IMPORT('repo/web/searchable_list.dart', 'change')

