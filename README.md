# image-query-and-display

A Polymer Element that builds and runs an elasticsearch aggregation query, shows the transformed image results in a paginated image gallery,
and shows a double bar chart with optional selectable behavior.

### Example
```html
<image-query-and-display
  aggregation-field="myAggregationField"
  query-fields='"myQueryField"'
  query-values='"myQueryValue"'
  client="[[client]]"
  index-name="myIndexName"
  index-types='["myIndexType"]'
  filter-list="[[filterList]]"
  transform-config="{}"
  transform-function="[[myTransformFunction]]"
  show-checkboxes
  hovering="{{hovering}}"
  images="{{images}}"
  loaded-images="{{loadedImages}}"
  selected="{{selected}}">
</image-query-and-display>
```

### Styling

`<image-query-and-display>` provides the following custom properties and mixins for styling:

Custom property                                          | Description                                                         | Default
---------------------------------------------------------|---------------------------------------------------------------------|--------
`--image-query-and-display-hovering-color`               | The background color of the hovering images.                        | none
`--image-query-and-display-loading-spinner`              | Mixin applied to the loading-spinner.                               | none
`--image-query-and-display-max-height`                   | Maximum height of the gallery.                                      | 160px
`--image-query-and-display-scroll-threshold`             | Mixin applied to the iron-scroll-threshold.                         | none
`--image-query-and-display-selected-color`               | The background color of the selected images.                        | none
`--image-query-and-display-show-more-button`             | Mixin applied to the show more button.                              | none
`--image-query-and-display-bar-color`                    | The color of the single or left bars.                               | --paper-grey-400
`--image-query-and-display-bar-count-color`              | The color of the single or left count labels.                       | --paper-grey-900
`--image-query-and-display-bar-height`                   | The height of the single or left bars.                              | 20px
`--image-query-and-display-bar-title-color`              | The color of the single or left title labels.                       | --paper-grey-900
`--image-query-and-display-bar-title-hover-color`        | The color of the single or left title labels on hover (if a link).  | --paper-grey-700
`--image-query-and-display-second-bar-color`             | The color of the right (second) bars.                               | --paper-grey-400
`--image-query-and-display-second-bar-count-color`       | The color of the right (second) count labels.                       | --paper-grey-900
`--image-query-and-display-second-bar-height`            | The height of the right (second) bars.                              | 20px
`--image-query-and-display-second-bar-title-color`       | The color of the right (second) title labels.                       | --paper-grey-900
`--image-query-and-display-second-bar-title-hover-color` | The color of the right (second) title labels on hover (if a link).  | --paper-grey-700

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

