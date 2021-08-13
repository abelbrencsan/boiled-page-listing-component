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
`listing-item-meta` | Applies a meta list inside listing item. | `<ul class="listing-item-meta-list"></ul>`
`listing-item-meta-list-item--wide` | Sets meta list item wider. | `<li class="isting-item-meta-list-item isting-item-meta-list-item--wide"></li>`
`isting-item-meta-list-item--narrow` | Sets meta list item narrower. | `<li class="isting-item-meta-list-item isting-item-meta-list-item--narrow"></li>`
`listing-item-meta-key` | Applies a key inside meta list item. | `<span class="listing-item-meta-key"></span>`
`listing-item-meta-value` | Applies a value inside meta list item. | `<span class="listing-item-meta-value"></span>`
`listing-item-action-list` | Applies a list of actions inside listing item. Use grid component for alignment. | `<ul class="listing-item-action-list grid"></ul>`

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
    <ul class="listing-item-meta-list">
      <li>
        <span class="listing-item-meta-key">Price</span>
        <span class="listing-item-meta-value">$5.69</span>
      </li>
      <li>
        <span class="listing-item-meta-key">Condition</span>
        <span class="listing-item-meta-value">Very Good</span>
      </li>
    </ul>
    <ul class="listing-item-action-list button-group-list grid">
      <li class="grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="grid-col grid-col--small--fit">
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
    <ul class="listing-item-meta-list">
      <li>
        <span class="listing-item-meta-key">Price</span>
        <span class="listing-item-meta-value">$8.59</span>
      </li>
      <li>
        <span class="listing-item-meta-key">Condition</span>
        <span class="listing-item-meta-value">Like New</span>
      </li>
    </ul>
    <ul class="listing-item-action-list button-group-list grid">
      <li class="grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="grid-col grid-col--small--fit">
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
    <ul class="listing-item-meta-list">
      <li>
        <span class="listing-item-meta-key">Price</span>
        <span class="listing-item-meta-value">$4.69</span>
      </li>
      <li>
        <span class="listing-item-meta-key">Condition</span>
        <span class="listing-item-meta-value">Very Good</span>
      </li>
    </ul>
    <ul class="listing-item-action-list button-group-list grid">
      <li class="grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="grid-col grid-col--small--fit">
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
    <ul class="listing-item-meta-list">
      <li>
        <span class="listing-item-meta-key">Price</span>
        <span class="listing-item-meta-value">$6.79</span>
      </li>
      <li>
        <span class="listing-item-meta-key">Condition</span>
        <span class="listing-item-meta-value">Good</span>
      </li>
    </ul>
    <ul class="listing-item-action-list button-group-list grid">
      <li class="grid-col grid-col--small--fit">
        <button type="button" class="button button--fit">Edit</button>
      </li>
      <li class="grid-col grid-col--small--fit">
        <button type="button" class="button button--fit button--badge">Delete</button>
      </li>
    </ul>
  </li>
</ul>
```
