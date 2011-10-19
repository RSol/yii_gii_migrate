<h3>Gii migrate</h3>

<h4>Instalation</h4>

<ol>
<li>Copy migrate folder into your protected/gii folder.</li>
<li>
Configure your application:
	<pre>
	'modules'=>array(
	  // uncomment the following to enable the Gii tool
	  'gii'=>array(
	   'class'=>'system.gii.GiiModule',
	   'password'=>'password',
		// If removed, Gii defaults to localhost only. Edit carefully to taste.
	   'ipFilters'=>array('127.0.0.1','::1'),
	   'generatorPaths'=>array(
		'application.gii',
	   ),
	   ...
	  ),
	</pre>
</li>
</ol>

This extention can:

<ul>
<li>generate migration code;</li>
<li>flush cache (checkbox);</li>
<li>clear assets (checkbox).</li>
</ul>

<i>Note: For flush cache and clear assets future you need to configure you console configuration to using assetManager and cache components.</i>