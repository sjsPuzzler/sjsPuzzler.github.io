<!DOCTYPE html>
<html lang="en">
<head>
	<title>Events</title>
	<link rel="stylesheet" href="styles.css">
	<meta charset="UTF-8">
	<meta name="keywords" content="event, plan, Meetup, Ottawa, visualization, data">
	<meta name="description" content="A Visualization tool to help you plan your next Meetup event.">
	<meta name="author" content="Planner Hats">
</head>
<body>
<!-- Load d3.js -->
<script src="https://d3js.org/d3.v4.js"></script>

<!-- Create a div where the graph will take place -->
<div id="my_dataviz"></div>

<!-- Load color palettes -->
<script src="https://d3js.org/d3-scale-chromatic.v1.min.js"></script>
<script>

// set the dimensions and margins of the graph
var margin = {top: 80, right: 25, bottom: 30, left: 40},
  width = 600 - margin.left - margin.right,
  height = 600 - margin.top - margin.bottom;

// append the svg object to the body of the page
var svg = d3.select("#my_dataviz")
.append("svg")
  .attr("width", width + margin.left + margin.right)
  .attr("height", height + margin.top + margin.bottom)
.append("g")
  .attr("transform",
        "translate(" + margin.left + "," + margin.top + ")");

//Read the data
d3.csv("https://raw.githubusercontent.com/sjsPuzzler/Meetup/main/csvFile.csv", function(data) {

  // Labels of row and columns -> unique identifier of the column called 'day' and 'week'
  var mydays = d3.map(data, function(d){return d.day;}).keys()
  var myVars = d3.map(data, function(d){return d.week;}).keys()

  // Build X scales and axis:
  var x = d3.scaleBand()
    .range([ 0, width ])
    .domain(mydays);
  svg.append("g")
    .style("font-size", 15)
    .attr("transform", "translate(0," + height + ")")
    .call(d3.axisBottom(x).tickSize(0))

  // Build Y scales and axis:
  var y = d3.scaleBand()
    .range([0,height])
    .domain(myVars);
  svg.append("g")
    .style("font-size", 15)
    .call(d3.axisLeft(y).tickSize(0))

  // Build color scale
  var myColor = d3.scaleSequential()
    .interpolator(d3.interpolateGreys)
    .domain([1,100])

  // create a tooltip
  var tooltip = d3.select("#my_dataviz")
    .append("div")
    .style("opacity", 0)
    .attr("class", "tooltip")
    .style("background-color", "white")
    .style("border", "solid")
    .style("border-width", "2px")
    .style("border-radius", "5px")
    .style("padding", "5px")

  // Three function that change the tooltip when user hover / move / leave a cell
  var mouseover = function(d) {
    tooltip
      .style("opacity", 1)
    d3.select(this)
      .style("stroke-width", 3)
      .style("stroke", "black")
      .style("opacity", 1)
  }
  var mousemove = function(d) {
    tooltip
      .html("RSVP count:" + d.rsvp)
      .style("left", (d3.mouse(this)[0]+70) + "px")
      .style("top", (d3.mouse(this)[1]) + "px")
  }
  var mouseleave = function(d) {
    tooltip
      .style("opacity", 0)
    d3.select(this)
      .style("stroke-width", 1)
      .style("stroke", "black")
      .style("opacity", 0.8)
  }

  // add the squares
  svg.selectAll()
    .data(data, function(d) {return d.day+':'+d.week;})
    .enter()
    .append("rect")
      .attr("x", function(d) { return x(d.day) })
      .attr("y", function(d) { return y(d.week) })
      .attr("width", x.bandwidth() )
      .attr("height", y.bandwidth() )
      .style("fill", function(d) { return myColor(d.rsvp)} )
      .style("stroke-width", 1)
      .style("stroke", "black")
      .style("opacity", 0.8)
    .on("mouseover", mouseover)
    .on("mousemove", mousemove)
    .on("mouseleave", mouseleave)
})

// Add title to graph
svg.append("text")
        .attr("x", 0)
        .attr("y", -50)
        .attr("text-anchor", "left")
        .style("font-size", "22px")
        .text("Number of Daily Tech RSVPs");

// Add subtitle to graph
svg.append("text")
        .attr("x", 0)
        .attr("y", -20)
        .attr("text-anchor", "left")
        .style("font-size", "14px")
        .style("fill", "grey")
        .style("max-width", 400)
        .text("Edited code: https://www.d3-graph-gallery.com/graph/heatmap_style.html");


</script>

<select>
  <option value="o1">Option 1</option>
  <option value="o2">Option 2</option>
  <option value="o3">Option 3</option>
  <option value="o4">Whatever</option>
</select>

</body>
</html>
