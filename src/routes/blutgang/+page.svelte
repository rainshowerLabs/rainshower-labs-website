<svelte:head>
	<title>Blutgang</title>
	<meta name="description" content="Blutgang, a blazing fast load balancer" />
</svelte:head>

<script>
   import Blutgang from "$lib/images/blutgang.jpg"
   import bench0 from "$lib/images/Figure_1.png"
   import bench1 from "$lib/images/Figure_2.png"
</script>

<div class="text-column">
	<p>
		<img style="width: 100%;" src={Blutgang} alt="Blutgang logo">
	</p>
	
	<h1>Blutgang - the wd40 of alpha ethereum load balancers</h1>

	<p>
		Blutgang is a <i>blazing fast</i>, caching, minimalistic load balancer designed with Ethereum's json-rpc in mind.<br><br>

		Blutgang's industry leading advantage, lies in the speed of its cache. Historical RPC querries are cached in a local database, bypassing the need for slow, repeating calls to your nodes.
	</p>
	<h1>Load Balancing</h1>
		<p>
			Blutgang is designed to be used in front of a cluster of Ethereum RPC nodes, distributing the load between them. By default, the load is balanced in a weighted round-robin configuration. Thanks to its modularity, the load balancing algorithm can be customized to support any load balancing schema.
		</p>
	<h1>Benchmarks</h1>
		<p>
			<img style="width: 100%;" src={bench0} alt="Benchmarks">
			<img style="width: 100%;" src={bench1} alt="Benchmarks">
		</p>
	<h1>Commercial licensing</h1>
	<p>
		Blutgang is libre software licensed under the AGPL-3.0 license. In practice, this means that if you use blutgang for non-personal use, <b>you are required by law to disclose the source code of blutgang, or any works based on or that use the licensed software in any way.</b> This includes MEV bots. Blutgang respects the freedom of it's users and will *always* be free for non-commerical use.   
	</p>
	<p>
		If you want to use blutgang <b>in a comercial setting without disclosing any source code, please reach out</b> via our contact page.
	</p>
</div>
