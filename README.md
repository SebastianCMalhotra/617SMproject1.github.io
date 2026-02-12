# 617SMproject1.github.io


---
layout: default
title: 617 Dear Data Redux
---

<div id="viz-container"></div>

<script src="https://d3js.org/d3.v6.min.js"></script>

<script>
  const data = [10, 20, 30, 40, 50];
  const svg = d3.select("#viz-container")
    .append("svg")
    .attr("width", 400)
    .attr("height", 100);

  svg.selectAll("rect")
    .data(data)
    .enter()
    .append("rect")
    .attr("x", (d, i) => i * 70)
    .attr("y", d => 100 - d)
    .attr("width", 50)
    .attr("height", d => d)
    .fill("steelblue");
</script>
