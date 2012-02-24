
## TESTING SYNTAX HIGHLIGHTING ##

The syntax could be:

````c#;[3,4]
	var a = 7;
	var b = 8;
	var result = a+b;
algo````

The Output in GitHub will be:

<pre><code class="c#;[3,4]">    var a = 7;
    var b = 8;
    var result = a+b;
</code></pre>

And the output after out tooling executes the post-processing could be:

<pre><code class="c#">    var a = 7;
    <strong style='background-color: lightBlue'>var b = 8;</strong>
    <strong style='background-color: lightBlue'>var result = a+b;</strong>
</code></pre>