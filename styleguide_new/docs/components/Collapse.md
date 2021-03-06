# Collapse

## Installation & Usage

#### React
`npm install babel-loader react-svg-loader --save-dev`

`npm install pui-react-collapse --save`

`import {BaseCollapse, AltCollapse, Collapse} from 'pui-react-collapse';`

#### CSS Only
`npm install pui-css-collapse --save`

## Description
Collapse description goes here.

Collapse components are implementations of the [Accordion][accordion] style. In
all `Collapse` component variations, the `header` prop describes the text
of the clickable region to toggle the expand/collapse states. You can pass `defaultExpanded`
as a prop to the `Collapse` and it will start expanded when the page loads.

This is a basic collapse with no additional styles.

## Examples

```jsx
::title=Basic Example
<BaseCollapse header="Panel 1">
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
  <p>Panel 1 content</p>
</BaseCollapse>
```

```jsx
::title=Without Arrows Example
::description=This is a basic collapse with an +/- icon in the clickable region
<AltCollapse header="Without Arrows">
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
</AltCollapse>
```

```jsx
::title=Arrow Icon Example
::description=This is a basic collapse with an arrow icon in the clickable region
<Collapse header="With Arrows">
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
</Collapse>
```

```jsx
::title=Divider Example
::description=To add a divider between the clickable region and the expanded content region, simply set the `divider` property to be true
<Collapse header="With Divider" divider>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
  <p>Content!</p>
</Collapse>
```

## Props

Property | Required | Type | Default | Description
---------|----------|------|---------|------------
divider         | no  | Boolean |       | Specifying this property adds a divider between the clickable region and the expanded content region
header          | yes | Node    |       | The text of the clickable region to toggle the expand/collapse states
defaultExpanded | no  | Boolean | false | Setting this to true will make the component start expanded when the page loads
