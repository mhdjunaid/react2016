# React HighCharts

Render HighCharts with React.js using JSON data.  This is a basic, working template of a bar chart with React that anyone can pull and start working on.

![alt text](https://github.com/jasonganub/react-highcharts/blob/master/screenshots/HighChartsScreenshot.PNG "Screenshot of a HighCharts example")

## Examples

```javascript
var chartInstance = new Highcharts.Chart(chartOptions);
this.setState({
  chartInstance: chartInstance
});
```

```javascript
var chart = React.render(
  React.createElement(Chart, {
    seriesModel: seriesObject,
    chartModel: chartObject}),
  document.getElementById('example')
);
```

```javascript
var seriesObject = [{
      name: 'Year 1800',
      data: [107, 31, 635, 203, 2]
  }, {
      name: 'Year 1900',
      data: [133, 156, 947, 408, 6]
  }, {
      name: 'Year 2008',
      data: [973, 914, 4054, 732, 34]
}];
```

## Installation

Download the full directory as a zip to use it as a template.

## Usage

The JSON data is modifiable within src/chart.js in the seriesObject array.

JSX users: src/chart.js

JavaScript users: build/chart.js

###### Note for JSX users:

Be sure to transform your JSX file into a JavaScript file.
ex: src/chart.js -> build/chart.js

## History

1.0.0 Initial release

## Credits

With the help of Justin Woo's Mori implementation, I minimized the solution to a working basic template.  If you would like a resizable chart, view his implementation at this link.  https://github.com/justinwoo/highcharts-mori-test

## License

React is BSD licensed.
Highcharts is free for a personal or non-profit project under the Creative Commons Attribution-NonCommercial 3.0 License.
