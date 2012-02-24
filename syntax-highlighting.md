
## TESTING SYNTAX HIGHLIGHTING ##

The syntax could be:

````c#;[2,3]
	int a = 7;
	int b = 8;
	var result = a + b;
	return result;
````

The Output in GitHub will be:

<pre><code class="c#;[3,4]">    var a = 7;
	int b = 8;
	var result = a + b;
	return result;
</code></pre>

And the output after out tooling executes the post-processing could be:

<pre><code class="c#">    var a = 7;
    <strong style='background-color: lightBlue'>int b = 8;</strong>
    <strong style='background-color: lightBlue'>var result = a + b;</strong>
	return result;
</code></pre>