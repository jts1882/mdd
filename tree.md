---
layout: default
title: Tree view of Taxonomy
---
<script type="text/javascript" src="js/papaparse.min.js"></script>
<script src="js/filter.js"></script>
<script src="js/mammals.js"></script>
<script>document.addEventListener("DOMContentLoaded", createMDDOrderList())</script>

<ul class="header-ul">
<li><a href="/index.html">Home</a></li>
<li><a href="assets/data/MDD.zip">Download the Database</a></li>
<li><a href="taxa.html">Explore Taxonomy</a></li>
<li><a href="tree.html">Treeview</a></li>
<li><a href="explore.html">Search Species</a></li>
<li style="float:right"><a href="about.html">About</a></li>
</ul>
<p>
    <h2>
    Treeview of Mammalian Taxonomy Hierarchy
    </h2>
    Click on symbols to expand collapse the tree to explore taxa families, genera, and species. Use the info icons to get the species details.
</p>
<div style="float:right;font-size:small;text-align:left;width:200px;padding:10px;margin:10px;border:1px solid #000088;border-radius:5px";>
                 <input id="check-MDD"     type="checkbox" name="load" onchange="onChangeOrderList(event)" checked >Treeview of MDD v1.31
            <br/><input id="check-MSW3"    type="checkbox" name="load" onchange="onChangeOrderList(event)"         >Treeview of MSW3
            <br/><input id="check-details" type="checkbox" name="load" onchange="onChangeOrderList(event)" checked >Species details pane
</div> 
<div style="clear:both;"></div>
<div id="content-details" > <!-- used by fillSpeciesInfo() --> </div>
<div id="content">
   <div id="content-MDD" class="interactive"></div>
   <div id="content-MSW3" class="interactive"></div>
</div>
