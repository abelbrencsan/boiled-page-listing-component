# Boiled Page listing component

Listing SCSS component for Boiled Page frontend framework. It is intended to create responsive listings with a thumbnail, a heading with a subheading, a list of key-value pairs, and a list of action buttons.

## Install

Place `_listing.scss` file to `/assets/css/components` directory, and add its path to components block in `assets/css/app.scss` file. You will also need to add button component for properly working buttons.

- Button component: <https://www.github.com/abelbrencsan/boiled-page-button-component>

## Usage

### Classes

Class name | Description | Example
---------- | ----------- | -------
`listing` | Applies a listing. | `<ul class="listing"></ul>`
`listing-item` | Applies an item inside listing. | `<li class="listing-item"></li>`
`listing-item-thumbnail` | Applies a thumbnail inside listing item. You can place a keypoint or a image into a thumbnail. | `<div class="listing-item-thumbnail"></div>`
`listing-item-header` | Applies a header with a heading and a subheading inside listing item. | `<header class="listing-item-header"></header>`
`listing-item-header--wide` | Sets listing item header wider. | `<header class="listing-item-header listing-item-header--wide"></header>`
`listing-item-header--narrow` | Sets listing item header narrower. | `<header class="listing-item-header listing-item-header--narrow"></header>`
`listing-item-meta` | Applies a meta list inside listing item. | `<ul class="listing-item-meta"></ul>`
`listing-item-meta-col` | Applies a column inside meta list. | `<li class="listing-item-meta-col"></li>`
`listing-item-meta-col--wide` | Sets meta list column wider. | `<li class="listing-item-meta-col listing-item-meta-col--wide"></li>`
`listing-item-meta-col--narrow` | Sets meta list column narrower. | `<li class="listing-item-meta-col listing-item-meta-col--narrow"></li>`
`listing-item-meta-col-key` | Applies a key inside meta list column. | `<span class="listing-item-meta-col-key"></span>`
`listing-item-meta-col-value` | Applies a value inside meta list column. | `<span class="listing-item-meta-col-value"></span>`
`listing-item-actions` | Applies a list of actions inside listing item. | `<ul class="listing-item-actions"></ul>`

### Examples

#### Example 1

The following example shows a listing with keypoints inside thumbnails.

```html
<ul class="listing">
  <li class="listing-item">
    <div class="listing-item-thumbnail">
      <div class="keypoint keypoint--small">86</div>
    </div>
    <header class="listing-item-header">
      <h3>Animal Farm</h3>
      <p>Book by George Orwell</p>
    </header>
    <ul class="listing-item-meta">
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Price</span>
        <span class="listing-item-meta-col-value">$5.69</span>
      </li>
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Condition</span>
        <span class="listing-item-meta-col-value">Very Good</span>
      </li>
    </ul>
    <ul class="listing-item-actions button-group-list grid">
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit button--badge">Delete</button>
      </li>
    </ul>
  </li>
  <li class="listing-item">
    <div class="listing-item-thumbnail">
      <div class="keypoint keypoint--small">72</div>
    </div>
    <header class="listing-item-header">
      <h3>Of Mice and Men</h3>
      <p>Book by John Steinbeck</p>
    </header>
    <ul class="listing-item-meta">
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Price</span>
        <span class="listing-item-meta-col-value">$8.59</span>
      </li>
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Condition</span>
        <span class="listing-item-meta-col-value">Like New</span>
      </li>
    </ul>
    <ul class="listing-item-actions button-group-list grid">
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit button--badge">Delete</button>
      </li>
    </ul>
  </li>
  <li class="listing-item">
    <div class="listing-item-thumbnail">
      <div class="keypoint keypoint--small">68</div>
    </div>
    <header class="listing-item-header">
      <h3>Goodnight Moon</h3>
      <p>Book by Margaret Wise Brown</p>
    </header>
    <ul class="listing-item-meta">
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Price</span>
        <span class="listing-item-meta-col-value">$4.69</span>
      </li>
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Condition</span>
        <span class="listing-item-meta-col-value">Very Good</span>
      </li>
    </ul>
    <ul class="listing-item-actions button-group-list grid">
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit button--badge">Delete</button>
      </li>
    </ul>
  </li>
  <li class="listing-item">
    <div class="listing-item-thumbnail">
      <div class="keypoint keypoint--small">65</div>
    </div>
    <header class="listing-item-header">
      <h3>Green Eggs and Ham</h3>
      <p>Book by Dr. Seuss</p>
    </header>
    <ul class="listing-item-meta">
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Price</span>
        <span class="listing-item-meta-col-value">$6.79</span>
      </li>
      <li class="listing-item-meta-col">
        <span class="listing-item-meta-col-key">Condition</span>
        <span class="listing-item-meta-col-value">Good</span>
      </li>
    </ul>
    <ul class="listing-item-actions button-group-list grid">
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="button-group-list-item grid-col grid-col--small--fit">
        <button type="button" class="button button--fit button--badge">Delete</button>
      </li>
    </ul>
  </li>
</ul>
```
