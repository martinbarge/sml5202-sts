<h1>Section 1:</h1>
<h2>Introduction to HTML</h2>
<p>Paragraph 1: HTML stands for HyperText Markup Language. It's the fundamental structural language of web pages.</p>
<p>Paragraph 2: HTML is quite easy to learn. All you have to remember is to write your code carefully, making sure you open and close tags correctly. Here are two basic tags to get you started:</p>
<p>This tag creates a heading known as H1, or heading level 1: <code>&lt;h1&gt; &lt;/h1&gt;</code>. The words 'Section 1:' at the top of this section are inside the h1 tags.<br>To make a smaller heading, you just change the h1 to h2 in the opening and closing tags. You can go from h1 all the way down to h6, which is the smallest heading size.</p>
<p>Next is the paragraph tag, which looks like this:<code>&lt;p&gt; &lt;/p&gt;</code>. Any text between these tags will appear a single paragraph. You can add new paragraphs easily by opening a new paragraph tag. I have numbered the paragraphs in this section to show you.</p>

<p>However, some tags do not close. E.G. The code for making a single line break is <code>&lt;br&gt;</code>. It looks like<br>this.<br>And this. <br> </p>

<p>Also, the tag for making a horizontal line across the page is: <code>&lt;hr&gt;</code>. The result looks like this:<hr> </p>

<h1>Section 2:</h1> 
<h2>Basic text formatting with HTML</h2>
<p>Other useful formatting tags are:</p>
  <ul>
    <li><code>&lt;strong&gt; &lt;/strong&gt;</code> for creating <strong>bold text</strong></li>
    <li><code>&lt;em&gt; &lt;/em&gt;</code> for creating <em>italic text</em></li>
     <li><code>&lt;u&gt; &lt;/u&gt;</code> for creating <u>underlined text</u>. It is generally used for indicating errors (e.g. <u>rong </u>spelling)</li>
    </ul>
<hr>
<h1>Section 3:</h1> 
<h2>Making lists with HTML</h2>
<p>You will notice that in Section 2 above, I used a bullet list to layout the points.</p>
<p>There are two types of list you can make: unordered lists (bullets), and ordered lists (numbers).</p>
<p>The HTML for unordered lists (bullets) is this:</p>
<p><code>&lt;ul&gt; &lt;li&gt;First item &lt;/li&gt; &lt;li&gt;Second item &lt;/li&gt; &lt;/ul&gt;</code></p>
<p>Here is an example of a to-do list:</p>
<ul>
    <li>Check my email.</li>
    <li>Do some research.</li>
    <li>Do my homework.</li>
    </ul>
    
<p>The HTML for ordered lists (numbers) is this:</p>
<p><code>&lt;ol&gt; &lt;li&gt;First item &lt;/li&gt; &lt;li&gt;Second item &lt;/li&gt; &lt;/ol&gt;</code></p>
<p>Here is an example of my top three favourite books:</p>
<ol>
    <li>A Short History of Tractors in Ukrainian.</li>
    <li>The Curious Incident of the Dog in the Night-Time.</li>
    <li>Sophie's World.</li>
    </ol>
<p>So that's it for lists for now.</p>
<hr>

<h1>Section 4:</h1> 
<h2>Inserting links in your HTML</h2>
<p>It's easy to insert a link. But before you do, it's important to understand the difference between <strong><em>relative</em></strong> and <strong><em>absolute</em></strong> links.</p>
<h3>Absolute Links</h3>
<p>An absolute link uses the full URL address of the page you want to link to. This is necessary if you are linking to a page outside of your own website.</p><p> For example: suppose you want to link to the W3Schools HTML Tutorial. Here is the web address: <code> https://www.w3schools.com/html/html_basic.asp</code>. And I want the link text to read: <code>visit the W3Schools HTML tutorial</code></p>
<p></p>
<p>Here is the code for inserting this link:</p>
<code>&lt;a href="https://www.w3schools.com/html/html_basic.asp"&gt; visit the W3Schools HTML tutorial&lt;/a&gt; </code>
<p>In the above code, you put the URL of the site inside double-inverted commas after href=</p>
<p>You then write the words for the link between the &gt; and the &lt;/a&gt; tags</p>
<p>Here is the result: <a href="https://www.w3schools.com/html/html_basic.asp">visit the W3Schools HTML tutorial</a> 

<h3>Relative Links</h3>
<p>Relative links are used to link to pages or assets (e.g. images and files) that are within the file structure your own website. We won't cover this yet, as it can be slightly complicated.</p> 
<p>So that's a brief introduction to links.</p>
<hr>

<h1>Section 5: Homework</h1> 
<h3>For homework, I'd like you to edit your GitHub page</h3>
    <p>Make three sections using the H1 heading style, as follows:</p>
  <ol>
  <li><strong>Section 1:</strong> Write a paragraph describing yourself (e.g. where you come from, what you are studying, how long you have lived in London. And include a link to your QMplus Hub Page for SML209 (the text for the link should read: 'Visit my QMplus Hub page'.</li>
    <li><strong>Section 2:</strong> Write a bullet list of three things you have to do.</li>
    <li><strong>Section 3:</strong> Write a numbered list of three of your favourite things.</li>
    </ol>
<p>Finally put a horizontal line between each section, like this:</p>
<hr>
<p>When you have finished, post the link to your github website on your QMplus Hub Journal.</p>
<p>Good luck!</p>
<hr>

