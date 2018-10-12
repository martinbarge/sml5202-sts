<h1>HTML Part 2: More text layouts</h1>
<h2>Images</h2>
<p>You can reference images from other web hosts, or you can upload an image to your GitHub repository and reference that.<p>
<p>First we will reference an image hosted on Wikipedia</p>
<img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe">
<p>The code for inserting images is: <code>&lt;img src="URL OF IMAGE" alt="DESCRIPTION OF IMAGE" &gt;</code></p>
<p>In the example above, the image src is <code> https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg </code></p>
<p>You will notice that the image fills the width of the content area. This is okay for this exercise. Later we will look at how to modify the width settings of the image.</p>

<hr>

<h2>2. Description lists</h2>
<p>Description lists are good for giving definitions</p>
<dl>
  <dt>soliloquy</dt>
  <dd>In drama, where a character speaks to themselves, representing their inner thoughts or feelings and in the process relaying them to the audience (but not to other characters.)</dd>
  <dt>monologue</dt>
  <dd>In drama, where a character speaks their thoughts out loud to share them with the audience and any other characters present.</dd>
  <dt>aside</dt>
  <dd>In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought, or piece of additional background information.</dd>
</dl>
<p>The code for inserting description lists is similar to that for ordered and unordered lists. But it uses three tags: <code>&lt;dl&gt; ... &lt;/dl&gt;</code>, which opens and closes the list. Then <code>&lt;dt&gt;...&lt;/dt&gt;</code>, which inserts the description term. Inside the dt tag you insert the description definition tag to provide the description: <code>&lt;dd&gt;...&lt;/dd&gt;</code></p>
<p>To get the code for this, <a href="https://www.w3schools.com/tags/tag_dl.asp">visit the W3Schools entry for description lists</a>.</p>

<hr>
<h2>3. Tables</h2>
<p>Tables are an orderly way to present information.</p>
<p>Here is an example of a simple verb table:</p>
<table>
  <tr><th>Infinitive</th><th>Past simple</th><th>Past participle</th></tr>
  <tr>
    <td>to go</td><td>went</td><td>gone/been</td>
  </tr>
   <tr>
    <td>to have</td><td>had</td><td>had</td>
  </tr>
  <tr>
    <td>to come</td><td>came</td><td>come</td>
  </tr>
  </table>
  
<p>The code for inserting tables is similar to that for description lists. But tables include three tags: <code>&lt;table&gt; ... &lt;/table&gt;</code>, which opens and closes the table. Then <code>&lt;tr&gt;...&lt;/tr&gt;</code>, which inserts a row into the table. Inside the <em>first</em> <b>tr</b> tag (i.e. The first table row) you insert the table header tag which will display the head for each column: <code>&lt;th&gt;...&lt;/th&gt;</code>. The humber of th tags you include determines the number of columns your table has.</p>
  
<p><b>For example:</b> In the first two columns of the table above, the first row code is like this: <code>&lt;tr&gt;&lt;th&gt;Infinitive&lt;/th&gt;&lt;th&gt;Past simple&lt;/th&gt;&lt;/tr&gt;</code></p>
<p>To insert another row, use <code>&lt;tr&gt;</code>.<br>
Then, insert cells into the row using the <code>&lt;td&gt;</code> tag, which means <b>table data</b>.<br>
So, in our two column table above, we would add: <code>&lt;tr&gt;&lt;td&gt;to go&lt;/td&gt;&lt;th&gt;went&lt;/td&gt;&lt;/tr&gt;</code></p>
<p>This may seem very complicated, so the best place to get the basic table code is, <a href="https://www.w3schools.com/tags/tag_table.asp">visit the W3Schools entry for tables</a>. Copy the code there and experiment.</p>

<hr>

<h2>4. Superscript</h2>
<p>Now for something easier. The superscript tag is useful for formatting the date.</p>
<p><b>Example:</b> My birthday is on the 25<sup>th</sup> of May 2001.</p>
<p>To make the 'th' a superscript (i.e. half the size of the numbers 25 and floating at the top of the 5), simply place <code>&lt;sup&gt; ... &lt;/sup&gt;</code> around the 'th'</p>
<hr>

<h2>5. Accented and Non-Latin Characters</h2>
<p>GitHub pages use the UTF-8 Character set. This means you can type accented letters directly into your page and it will display correctly</p>
<p>Examples:</p>
<ul>
    <li lang="pl">jabłko</li>
    <li lang="ru">Доброе утро</li>
    <li lang="zh-Hans">你好</li>
</ul>
<p>However, if you recall, in order for screen reading software to pronounce the words correctly, you need to add the &lt;lang="X"&gt; attribute to the tag, where X is the abbreviated language code.<br>
  <b>For example:</b> In the list above, the tag for the Polish word is <code>&lt;li lang="pl"&gt;</code>, where pl is the abbreviated language code for Polish. The language code for the Russian word is "ru" and for the Chinese word "zh-Hans". A full listing of the language codes is provided on the <a href="https://www.w3schools.com/tags/ref_language_codes.asp">W3Schools Website</a>.
</p>
<hr>

