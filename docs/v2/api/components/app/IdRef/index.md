---
layout: "v2_fluid/docs_base"
version: "nightly"
versionHref: "/docs/v2"
path: ""
category: api
id: "{{IdRef | slugify}}"
title: "IdRef"
header_sub_title: "Class in module "
doc: "IdRef"
docType: "class"

---




<div class="improve-docs">
  <a href='http://github.com/driftyco/ionic2/tree/master/ionic/components/app/id.ts#L2'>
    View Source
  </a>
  &nbsp;
  <a href='http://github.com/driftyco/ionic2/edit/master/ionic/components/app/id.ts#L2'>
    Improve this doc
  </a>

</div>




<h1 class="api-title">


IdRef






</h1>






<h2>Description</h2>

<p>IdRef is an easy way to identify unique components in an app and access them
no matter where in the UI heirarchy you are. For example, this makes toggling
a global side menu feasible from any place in the application.</p>
<p>See the <a href="http://ionicframework.com/docs/v2/components/#menus">Menu section</a> of
the Component docs for an example of how Menus rely on ID&#39;s.</p>
<p>To give any component an ID, simply set its <code>id</code> property:</p>
<pre><code class="lang-html">&lt;ion-checkbox id=&quot;myCheckbox&quot;&gt;&lt;/ion-checkbox&gt;
</code></pre>
<p>To get a reference to the registered component, inject the <a href="../app/IonicApp/">IonicApp</a>
service:</p>
<pre><code class="lang-ts">constructor(app: IonicApp) {
  var checkbox = app.getComponent(&quot;myCheckbox&quot;);
  if (checkbox.checked) console.log(&#39;checkbox is checked&#39;);
}
</code></pre>
<p><em>NOTE:</em> It is not recommended to use ID&#39;s across Pages, as there is often no
guarantee that the registered component has not been destroyed if its Page
has been navigated away from.</p>


<h2>Directive</h2>
<h3>selector: <code>[id]</code></h3>





<h2>Methods</h2>

<div id="app"></div>

<h3>
<code>app()</code>

</h3>












<div id="elementRef"></div>

<h3>
<code>elementRef()</code>

</h3>












<div id="appViewManager"></div>

<h3>
<code>appViewManager()</code>

</h3>










<!-- end content block -->


<!-- end body block -->

