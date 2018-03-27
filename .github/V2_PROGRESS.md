# Info

How to convert a component to the new Vue InstantSearch architecture?

1.  make the new file under `/src/components` by copying `/src/components/__template__.vue`.
2.  import the connector in the file and add it to `beforeCreate`
3.  check which props to add as an option in [InstantSearch specs](https://instantsearch-css.netlify.com)
4.  add the props to the component
5.  add the `widgetParams` based on the props (usually copy-paste)
6.  copy `/stories/__template__.stories.js` into your own story
7.  see if it works
8.  ...
9.  Profit!

next steps are the DOM changes, which will be done after.

# Prep work

* [x] pass down an InstantSearch.js instance
* [ ] apply correct properties to the main component
* [x] allow passing of a connector on a widget
* [x] allow destroying of a widget
* [x] allow changing of parameters on a widget
* [x] allow widgetFactories without connector (i.e. `configure`)
* [x] define which options to use
* [x] define which DOM to use
* [ ] update `bem` function to `suit` (CSS)

# Components

A checklist for all of the components which are completely done.

* connectors
  * [x] `ais-breadcrumb`
  * [x] `ais-clear-refinements`
  * [x] `ais-configure`
  * [x] `ais-current-refinements`
  * [x] `ais-hierarchical-menu`
  * [ ] `ais-highlight`
  * [ ] `ais-hits-per-page`
  * [ ] `ais-hits`
  * [ ] `ais-index`
  * [ ] `ais-infinite-hits`
  * [ ] `ais-menu-select`
  * [ ] `ais-menu`
  * [ ] `ais-numeric-menu`
  * [ ] `ais-numeric-selector`
  * [ ] `ais-pagination`
  * [ ] `ais-panel`
  * [ ] `ais-powered-by`
  * [ ] `ais-range-input`
  * [ ] `ais-range-slider`
  * [ ] `ais-rating-menu`
  * [ ] `ais-refinement-list`
  * [ ] `ais-search-box`
  * [ ] `ais-snippet`
  * [ ] `ais-sort-by`
  * [ ] `ais-stats`
  * [ ] `ais-toggle-refinement`
  * [ ] `ais-index`
* DOM
  * [ ] `ais-breadcrumb`
  * [ ] `ais-clear-refinements`
  * [x] `ais-configure`
  * [ ] `ais-current-refinements`
  * [ ] `ais-hierarchical-menu`
  * [ ] `ais-highlight`
  * [ ] `ais-hits-per-page`
  * [ ] `ais-hits`
  * [ ] `ais-index`
  * [ ] `ais-infinite-hits`
  * [ ] `ais-menu-select`
  * [ ] `ais-menu`
  * [ ] `ais-numeric-menu`
  * [ ] `ais-numeric-selector`
  * [ ] `ais-pagination`
  * [ ] `ais-panel`
  * [ ] `ais-powered-by`
  * [ ] `ais-range-input`
  * [ ] `ais-range-slider`
  * [ ] `ais-rating-menu`
  * [ ] `ais-refinement-list`
  * [ ] `ais-search-box`
  * [ ] `ais-snippet`
  * [ ] `ais-sort-by`
  * [ ] `ais-stats`
  * [ ] `ais-toggle-refinement`
  * [ ] `ais-index`
* docs
  * [ ] `ais-breadcrumb`
  * [ ] `ais-clear-refinements`
  * [x] `ais-configure`
  * [ ] `ais-current-refinements`
  * [ ] `ais-hierarchical-menu`
  * [ ] `ais-highlight`
  * [ ] `ais-hits-per-page`
  * [ ] `ais-hits`
  * [ ] `ais-index`
  * [ ] `ais-infinite-hits`
  * [ ] `ais-menu-select`
  * [ ] `ais-menu`
  * [ ] `ais-numeric-menu`
  * [ ] `ais-numeric-selector`
  * [ ] `ais-pagination`
  * [ ] `ais-panel`
  * [ ] `ais-powered-by`
  * [ ] `ais-range-input`
  * [ ] `ais-range-slider`
  * [ ] `ais-rating-menu`
  * [ ] `ais-refinement-list`
  * [ ] `ais-search-box`
  * [ ] `ais-snippet`
  * [ ] `ais-sort-by`
  * [ ] `ais-stats`
  * [ ] `ais-toggle-refinement`
  * [ ] `ais-index`
* stories
  * [ ] `ais-breadcrumb`
  * [ ] `ais-clear-refinements`
  * [x] `ais-configure`
  * [ ] `ais-current-refinements`
  * [ ] `ais-hierarchical-menu`
  * [ ] `ais-highlight`
  * [ ] `ais-hits-per-page`
  * [ ] `ais-hits`
  * [ ] `ais-index`
  * [ ] `ais-infinite-hits`
  * [ ] `ais-menu-select`
  * [ ] `ais-menu`
  * [ ] `ais-numeric-menu`
  * [ ] `ais-numeric-selector`
  * [ ] `ais-pagination`
  * [ ] `ais-panel`
  * [ ] `ais-powered-by`
  * [ ] `ais-range-input`
  * [ ] `ais-range-slider`
  * [ ] `ais-rating-menu`
  * [ ] `ais-refinement-list`
  * [ ] `ais-search-box`
  * [ ] `ais-snippet`
  * [ ] `ais-sort-by`
  * [ ] `ais-stats`
  * [ ] `ais-toggle-refinement`
  * [ ] `ais-index`
* tests
  * [ ] `ais-breadcrumb`
  * [ ] `ais-clear-refinements`
  * [ ] `ais-configure`
  * [ ] `ais-current-refinements`
  * [ ] `ais-hierarchical-menu`
  * [ ] `ais-highlight`
  * [ ] `ais-hits-per-page`
  * [ ] `ais-hits`
  * [ ] `ais-index`
  * [ ] `ais-infinite-hits`
  * [ ] `ais-menu-select`
  * [ ] `ais-menu`
  * [ ] `ais-numeric-menu`
  * [ ] `ais-numeric-selector`
  * [ ] `ais-pagination`
  * [ ] `ais-panel`
  * [ ] `ais-powered-by`
  * [ ] `ais-range-input`
  * [ ] `ais-range-slider`
  * [ ] `ais-rating-menu`
  * [ ] `ais-refinement-list`
  * [ ] `ais-search-box`
  * [ ] `ais-snippet`
  * [ ] `ais-sort-by`
  * [ ] `ais-stats`
  * [ ] `ais-toggle-refinement`
  * [ ] `ais-index`

# Rounding up work

* [ ] release plan
* [ ] migration guide