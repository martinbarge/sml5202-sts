<h1>HTML and CSS Part 1</h1>
<h2>1. Making Images Clickable</h2>
<p>Sometimes it can be helpful for your page visitors to view images in a larger window. This can be done by adding a <code> &lt;a href=""  </code> tag around the image. This is also useful if you want an image to link to another website or page in your own website.<p>
<p>Here is an example of an image from Wikipedia that is now clickable</p>
<p>
<a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source">
<img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"></a>
</p>
<div class="clearLeft"></div>

<p>Ths code for this is:</p>
<div class="code">
<p>
&lt;a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source"&gt;
<br>
&lt;img  src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"&gt; 
<br>
&lt;/a&gt;
</p>
</div>
<p>Look at the above lines of code carefully. Notice the order in which the tags are placed:</p> 

<ol>
<li>We open the familiar link tag: <code> &lt;a href="" </code> and include the URL of the image source. Notice also that we can add a <code> title= </code> attribute to the tag. The title attribute specifies text that appears over the image when the user hovers their mouse on the image.</li>
<li>Next, we have the familiar image tag: <code> &lt;img src="" </code>. You will notice that in this case the URL to the image is the same as in the href tag.</li>
<li>Finally, we must close the <code> &lt;/a&gt; </code> tag.</li>
</ol>

<h2>2. Changing the size and position of images.</h2>
<h3>2.1: Changing the display size of images.</h3>
<p>Sometimes we might want our image to occupy less space on the page. This can be done by adding a style attribute to the tag.</p>
<p>Here is an example of a simple style attribute added to the image tag that specifies the image to occupy only 70% of the width of the page content area: <code> style="width:70%; </code>.</p>

<p>In the example above, the word <code> width </code> is known as a style <strong style="color:#33cc00;">property</strong>, and the number <code>70%</code> is known as the <strong style="color:#33cc00;">value</strong>. Notice that the property and the value are separated by a colon (:) </p>

<p> The Mozilla Developer Network provides a <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#Keyword_index">full reference for all possible style properties</a>. <b>But you don't need to worry about learning them all! Just a few are useful for our purposes.</b></p>
<p>We can add other properties and values to our style entry. For example: <code> style="width:70%; border:1px solid green; </code>. Adding the 'border' property specifies a border around the image. In this example, the border property is followed by 3 values: <code> 1px solid green </code>. This means the border will be a solid green line, one pixel thick.</p>
<p>Notice that to add a new property to the style, we need to put a semi-colon after the previous property:value pair.</p>
<p>So the full code for our image tag would now look like this:</p>
<code> 
&lt;img style="width:70%; border:1px solid green;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe" &gt;
</code>

<p>And the result is this:</p>
<p>
<a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source">
<img style="width:70%; border:1px solid green;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"></a>
</p>

<h3>2.2: Centering an image on the page.</h3>
<p style="margin-left:15%;">This time, the image is centred.</p>
<a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source">
<img style="width:70%; border:1px solid green; margin-left:15%;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"></a>
<p>To centre the image, it's necessary to make a small calculation. In our example, this is as follows:</p>


<div style="margin-left:1rem; padding:.8rem; background-color:#f6f8fc; font-family: courier;">
<p>page content width = 100% <br>
image width = 70% <br>
  &#8756; remaining content width = 30% </p>

<p>So, to centre the image we need to divide the remaining content width (30%) so that it is equal on both sides of the image: <br>
We know that 30% &#247; 2 = 15% </p>
<p>So we now know we need a space of 15% to the left and 15% to the right of the image.<br> 
Numerically, it looks like this:<br>
left-hand margin width = 15%; <br>
image width = 70% <br>
right-hand margin width = 15%
</p>
</div>

<p>In our image, we specified the width to be 70%. This means the image uses 70% of the 100% content area available. By default, the image is positioned to the left of the content area. This means that to right of the image, 30% of the page width is blank. So, to centre the image, we need to put a space of 15% to the left of the image.</p> 
  
<p>To do this, we use a style property known as <code> margin-left </code> with a value of 15% (half of the blank space).</p>
<p>The <code> margin-left </code> property specifies a distance of x between the left-hand edge of the image and the left-hand edge of the  content area - just like a margin on a paper page.</p> 
<p>So, here is the modified image style code:</p>
<code> 
&lt;img style="width:70%; border:1px solid green; margin-left:15%;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe" &gt;
</code>

<p>Note: in the above example we don't need to specify a margin-right:15% because this is automatically computed by the browser. The browser computes the specified values of 15% + 70% = 85%, and then assigns the remaining 15% to the right-hand margin.</p>

<p>Understanding the way the page width can be divided in this way enables us to position objects on our pages, including blocks of text.</p>

<h2>3. Formating Text with CSS</h2>
<p>A very useful application of CSS is text formatting.</p>
<p>For example, in a language learning website, we might need to set certain classes of words to different colours in order to hightlight textual features for our learners. The following example shows a paragraph with the nouns highlighted in green and the adjectives in purple:</p>
<h3>Ode to Autumn, by John Keats</h3>
<p><span id="noun">SEASON</span> of <span id="noun">mists</span> and <span id="adj">mellow</span> <span id="noun">fruitfulness</span>!<br>	 
<span id="adj">Close</span> <span id="noun">bosom-friend</span> of the maturing <span id="noun">sun</span>;<br> 
Conspiring with him how to load and bless<br>
  With <span id="noun">fruit</span> the <span id="noun">vines</span> that round the <span id="noun">thatch-eaves</span> run;
</p>

<p>To format words and phrases within a paragraph, you can use the familiar &lt;strong&gt; and &lt;em&gt; tags. However, if you want to apply other styles, such as colours, then we use the <code> &lt;span style=""&gt; </code> tag. The span tag combined with style property will modify whatever the tag surroungs. So in the example above, to set the word 'SEASON' to green, the tag looks like this: <code> &lt;span style="color:#00cc00;"&gt; SEASON &lt;/span&gt; </code>. </p>
