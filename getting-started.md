---
layout: detail-with-left-sidebar
title: Getting started
permalink: /getting-started/
---



<h1 class="page-detail-heading">Getting started</h1>
<p class="page-sub-paragraph">The simplest way to use a visualization created in CARTO on an external site is as follows.</p>
<figure class="highlight">
	<pre><code class="language-html" data-lang="html"><span class="nt">&lt;link</span> <span class="na">rel=</span><span class="s">"stylesheet"</span><span class="na">href=</span><span class="s">"http://libs.cartocdn.com/cartodb.js/v3/3.15/themes/css/cartodb.css"</span> <span class="nt">/&gt;</span>
...
<span class="nt">&lt;div</span><span class="na">id=</span><span class="s">"map"</span><span class="nt">&gt;&lt;/div&gt;</span>
...
<span class="nt">&lt;script </span><span class="na">src=</span> <span class="s">"http://libs.cartocdn.com/cartodb.js/v3/3.15/cartodb.js"</span> <span class="nt">&gt;&lt;/script&gt;</span> <span class="nt">&lt;script&gt;</span> 
<span class="c1">// get the viz.json url from the CARTO Editor</span> 
<span class="c1">// - click on visualize</span> 
<span class="c1">// - create new visualization</span> 
<span class="c1">// - make visualization public</span> 
<span class="c1">// - click on publish</span> 
<span class="c1">// - go to API tab</span>
			
<span class="nb">window</span><span class="p">.</span><span class="nx">onload</span> <span class="o">=</span> <span class="kd">function</span><span class="p">()</span> <span class="p">{</span>
<span class="nx">cartodb</span><span class="p">.</span><span class="nx">createVis</span><span class="p">(</span><span class="s1">'map'</span><span class="p">,</span> <span class="s1">'http://documentation.carto.com/api/v2/viz/2b13c956-e7c1-11e2-806b-5404a6a683d5/viz.json'</span><span class="p">);</span>
<span class="p">}</span>
<span class="nt">&lt;/script&gt;</span>
		</code></pre>
</figure>

<p class="page-sub-paragraph"><a href="#">Here is the complete example source code</a></p>

<h2 class="page-detail-sub-heading">Using the CARTO.js Library</h2>

<p class="page-sub-paragraph">CARTO.js can be used to embed a visualization you have designed using CARTO’s user interface, or to dynamically create visualizations from scratch, using your data. If you want to create new maps on your webpage, jump to Creating a visualization from scratch. If you already have maps on your webpage and want to add CARTO visualizations to them, read Adding CARTO layers to an existing map.</p>
<p class="page-sub-paragraph">You can also use the CARTO APIs to create visualizations programmatically. This can be useful when the visualizations react to user interactions. To read more about it, jump to Creating visualizations at runtime.</p>

<table>
	<tr>
		<th>Arguments</th>
		<th>Description</th>
	</tr>

	<tr>
		<td>map_id</td>
		<td>a DOM object</td>
	</tr>
	<tr>
		<td>vizjson_url</td>
		<td>url of the vizjson object.</td>
	</tr>
	<tr>
		<td>callback(vis, layers)</td>
		<td>if a function is specified, it is called once the visualization is created.</td>
	</tr>
</table>

<h3>Other Mapping Libraries</h3>
<p class="page-sub-paragraph">We have also made it easy for you to build maps using the mapping library of your choice. Whether you are using Leaflet or something else, our CARTO.js code remains the same. This makes our API documentation simple and straightforward. It also makes it easy for you to consistently develop, or maintain, multiple maps online.</p>

<div class="alert alert-success" role="alert">
<p class="page-sub-paragraph">CARTO.js automatically includes dependencies from other mapping libraries (such as Leaflet, jQuery, Mustache, Underscore, and so on). You do not have to manually include these libraries, or worry about other mapping library version control, when you are using CARTO.js. If you need to see which version of other mapping libraries are included, view the vendor folder for each CARTO.js release.</p>
</div>

<h2 class="page-detail-sub-heading">Creating a Visualization from Scratch</h2>
<p class="page-sub-paragraph">This is the easiest way to quickly get a CARTO map onto your webpage. Use this method when there is no map in your application, and you want to add the visualization to hack over it. CARTO.js handles all the details of loading a map interface, basemap, and your CARTO visualization.</p>
<p class="page-sub-paragraph">You can start by giving CARTO.js the DIV ID from your HTML where you want to place your map, and the viz.json URL of your visualization (which you can get from the Publish your map options).</p>

<h2 class="page-detail-sub-heading">Next steps</h2>
<p class="page-sub-paragraph">Once the form, with the stored payment token, is submitted to your server, you'll want to use the payment details just collected. Usually this means one of three actions:</p>

<h2 class="page-detail-sub-heading">Questions?</h2>
<p class="page-sub-paragraph">We're always happy to help with code or other questions you might have! Search our site for more information or <a href="mailto:loremipsum@loremmail.com">send us an email</a>!</p>
