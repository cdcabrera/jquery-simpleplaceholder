<h1>jQuery.SimplePlaceholder</h1>
<p>
    Quick jQuery placeholder attribute plugin. Developed specifically for compatibility
    with Internet Explorer 7-9.
</p>
<p>
    Needed a temporary way to allow multiple submit scenarios.
    Thought about assigning an initial jQuery submit event, but yet another scenario popped up where
    I couldn't guarantee a standard form submittal. Hopefully this version of the plugin is
    generic enough to allow for a variety of uses.
</p>

<p>
    Originally, I tried cloning input elements utilizing "outerHTML" and had pretty good success,
    even with handling "password" input elements. Also incorporated the use of removing the "name"
    attribute which seemed to fix multiple fields submitting. Long story short IE, I forget which
    version, had an issue with the removal of the name attribute, ohs well.
</p>



<h2>How it works</h2>
<p>
    The plugin makes use of one off built in methods that shouldn't interfere with standard
    jQuery functions. The built in methods include a:
</p>
<ul>
    <li>serialize method;</li>
    <li>serializeArray method;</li>
    <li>and a blank out method.</li>
</ul>

<p>
    You'll notice a similarity between "serialize" and "serializeArray" from jQuery's method listing. That's
    because the built in methods utilize jQuery's methods with the added benefit of removing placeholder
    values from your fields.
</p>

<p>
    The plugin shouldn't interfere with browsers that actually support the
    attribute, such as Firefox, Chrome, and Opera. All hail the demise of IE < 9.
</p>

<h2>Requirements</h2>
<p>
    General requirements for use:
</p>
<ul>
    <li>
        Use of a version of jQuery 1.7 - 1.9. If you need an older
        version of jQuery you'll have to mod the use of the ".on()" method.
    </li>
</ul>

<h2>Limitations &amp; issues</h2>
<p>
    What you should be aware of:
</p>
<ul>
    <li>
        It's IE, what shouldn't you be aware of. Though it's no Webkit =), thank goodness updated versions of Chrome and Safari
        support placeholders or I think I would have lost my hair. Humor aside, good luck.
    </li>
</ul>

<h2>Browser compatibility</h2>
<p>
    Tested in IE 7-9. And minimally tested to make sure it doesn't interfere with Firefox, Chrome, and Opera.
</p>

<h2>License</h2>
<p>
    Released under the <a href="http://opensource.org/licenses/mit-license.php">MIT License</a>.
</p>