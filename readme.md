LineChart.js

Creates a single-line D3 line chart. 

Get Started:

 - *Data Format:*
	 - **VARIABLE NAMING**: LineChart.js requires data to have 2 properties: "x" and "y". When preparing your data, make sure your x-axis and y-axis variables are renamed accordingly. 
		Example: Values for each year for a given country.
		 `chartData = data.map(function (d) {
                return {
                    x: d[year],
                    y: d[value],
                    id: d['country_area']
                };
            });`
		 
	 - **DATA NESTING**: LineChart.js requires (x, y) value pairs to be nested according to what they aim to represent as a line. In our previous example, it would be nested by 'country_area'.
 - *Chart Properties:* there are many details that can be changed for your line graph. All properties will be updated in the following manner: `LineChart().title('GDP Australia');`

	Modifiable chart properties include:
	 
	 - Chart Title: takes in a string of chars and modifies the chart's title. ` title('GDP Australia')`
	 - X-Axis Title: takes in a string of chars and modifies the chart's X-Axis Label. `xTitle('Year')`
	 - Y-Axis Title: takes in a string of chars and modifies the chart's Y-Axis Label. `yTitle('Value')`
	 - X-Axis Scale: takes in a string indicating 'linear' or 'log' scale. `xScaleType('linear')`
	 - Y-Axis Scale:takes in a string indicating 'linear' or 'log' scale. `yScaleType('linear')`
	 - Width: takes in an int and modifies the chart's width. `width(500)`
	 - Height: takes in an int and modifies the chart's height. `height(500)`
	 - Line Stroke: takes in a float and modifies the chart's line's width. `strokeWidth(4.0)`
	 - Line Color: takes in a string of chars and modifies the chart's line color. `stroke('yellow')`
	 - Transition Duration: takes in an int and modifies the duration of enter, update and remove transitions. Duration for transitions for axes is half of the number of provided.`duration(3000)`
