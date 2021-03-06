---
layout: "simulator"
page_title: "Convergence Simulator"
sidebar_current: "docs-internals-simulator"
---

<h1>Serf Convergence Simulator</h1>

<p>
The graph below shows the expected time to reach various states of convergence
depending on the settings which are tunable below the graph. Below the graph,
the estimated maximum bandwidth usage is shown per node in <em>kilobits</em>
per second.
</p>
<p>
The default values in the boxes are also the default values that Serf
is configured with, where applicable.
</p>

<div class="row">
    <div id="graph"></div>
</div>
<div class="row">
	<div class="col-md-12">
		<h4>Estimated max bandwidth: <span id="bytes">0</span> kbps/node</h4>
	</div>
</div>
<div class="row">
	<div class="col-md-6">
		<h5>Gossip Interval</h5>
		<p>The gossip interval controls how often messages are gossiped to other nodes</p>
		<input type="text" id="interval" value="0.2"> seconds
	</div>
	<div class="col-md-6">
		<h5>Gossip Fanout</h5>
		<p>The gossip fanout controls how many nodes we gossip with</p>
		<input type="text" id="fanout" value="3"> nodes
	</div>
</div>
<div class="row">
	<div class="col-md-6">
		<h5>Nodes</h5>
		<p>This controls how many simulated nodes are in the cluster</p>
		<input type="text" id="nodes" value="30">
	</div>
	<div class="col-md-6">
		<h5>Packet Loss</h5>
		<p>This controls the amount of simulated packet loss [0, 100)</p>
		<input type="text" id="packetloss" value="0"> % lost packets
	</div>
</div>
<div class="row">
	<div class="col-md-6">
		<h5>Node failures</h5>
		<p>This controls what percent of simulated nodes are failed</p>
		<input type="text" id="failed" value="0"> % failed
	</div>
	<div class="col-md-6">
	</div>
</div>
