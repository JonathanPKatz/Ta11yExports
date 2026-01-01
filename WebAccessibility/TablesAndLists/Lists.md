---
title: Lists
description: >-
  Lists group a series of related items. They format text in a way that simplifies the content and lowers the density of text on a page. Lists make it easier for people to quickly scan and understand information.
contributors:
  - en/ellen-liebert
  - en/liz-thomas
  - en/Jonathan-katz-ouziel
sidebar:
  order: 5

---

<h1 id="lists">Lists</h1>
<h2 id="summary">Summary</h2>
<p>Lists group a series of related items. They format text in a way that simplifies the content and lowers the density of text on a page. Lists make it easier for people to quickly scan and understand information.</p>
<h2 id="overview">Overview</h2>
<p>Lists make it easier for people to scan a series of items. The native styling and structure of lists simplifies and organizes content to help people understand information.</p>
<p>Use lists to group a series of three or more related items.</p>
<ul>
<li>Use ordered lists for information that follows a specific order, such as a series of steps to complete a task.</li>
<li>Use unordered lists for related information that does not follow a specific order, such as a shopping list.</li>
<li>Websites may also include menu lists for organizing menus and definition lists to organize glossaries or similar types of content.</li>
</ul>
<p>Basic guidelines for lists include:</p>
<ul>
<li>Use lists for a series of three or more related items.</li>
<li>Keep items in lists concise.</li>
<li>Use the correct document or web formatting to create lists.</li>
<li>Do not use characters like asterisks or dashes to create the appearance of a list with bullets.</li>
<li>Keep to one phrase or sentence per list item if possible.</li>
<li>Avoid nested or multi-level lists if possible.</li>
<li>Limit multi-level lists to two levels if they are used.</li>
<li>Start each list item with the same:
<ul>
<li>word type (such as a noun or a verb)</li>
<li>tense (past, present, or future)</li>
<li>sentence type (such as instructions or a question).</li>
</ul>
</li>
<li>Do not use tables to organize lists. See <strong>Layout Tables (Ta11y)</strong> for more information.</li>
</ul>
<h2 id="who-is-helped">Who is Helped?</h2>
<p>Lists simplify content and make it easier for people to understand information. This can be especially helpful for people with cognitive disabilities such as dyslexia, language-related disabilities, or memory impairment.</p>
<ul>
<li>Bulleted lists simplify sentence structure by replacing nesting clauses with short phrases or sentences.</li>
<li>Numbered lists help to break complex processes into a series of steps.</li>
</ul>
<p>These same techniques also make content easier for people with low vision to scan and understand.</p>
<p>People who use assistive technologies may be able to navigate to lists on a page using keyboard shortcuts or voice commands. Screen readers will also announce the number of items in a list and identify each list item as it is read; knowing the list length helps people who cannot see the list understand what to expect. Correctly formatted lists help these individuals move through content more efficiently and better understand a content’s structure.</p>
<h2 id="guidelines">Guidelines</h2>
<p>Lists must be marked up in the code using the correct semantic HTML for the type of list. The term “semantic” indicates that the HTML element conveys the meaning of its content.</p>
<p>Lists should never use text characters, such as asterisks, dashes, icons, or foreground images, to create the appearance of a list. While this may add visual clues for sighted users, it does not provide the necessary meaning that semantic HTML provides to make lists accessible to assistive technologies.</p>
<p>There are four types of lists used in digital content:</p>
<ul>
<li>Ordered lists</li>
<li>Unordered lists</li>
<li>Menu lists</li>
<li>Description lists</li>
</ul>
<h3 id="ordered-lists-ol">Ordered lists <code>&lt;ol&gt;</code></h3>
<p>Ordered lists are used for information that follows a specific order. For example, a recipe or directions.</p>
<p>These lists are marked up using a  <code>&lt;ol&gt;</code>  parent element and  <code>&lt;li&gt;</code>  child elements.</p>
<p>Code example:</p>
<pre><code>&lt;ol&gt;
	&lt;li&gt;Add milk&lt;/li&gt;
	&lt;li&gt;Add flour&lt;/li&gt;
	&lt;li&gt;Combine all ingredients&lt;/li&gt;
&lt;/ol&gt;
</code></pre>
<h3 id="unordered-lists-ul">Unordered lists <code>&lt;ul&gt;</code></h3>
<p>Unordered lists are used for related information that does not follow a specific order. For example, a shopping list. These lists are marked up using a  <code>&lt;ul&gt;</code>  parent element and  <code>&lt;li&gt;</code>  child elements.</p>
<p>Code example:</p>
<pre><code>&lt;ul&gt;
&lt;li&gt;Tabby&lt;/li&gt;
&lt;li&gt;Scottish fold&lt;/li&gt;
&lt;li&gt;Persian&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<h3 id="menu-menu">Menu <code>&lt;menu&gt;</code></h3>
<p>The  <code>&lt;menu&gt;</code> element is an alternative to an unordered list  <code>&lt;ul&gt;</code>  but is intended for use with interactive items, such as a toolbar. It is exposed to assistive technologies in the same way that an unordered list is. It contains a list of items using the  <code>&lt;li&gt;</code>  element that represents actions or commands.</p>
<p>Code example:</p>
<pre><code>&lt;menu&gt;
	&lt;li&gt;&lt;button id="save"&gt;Save this article&lt;/button&gt;&lt;/li&gt;
	&lt;li&gt;&lt;button id="share"&gt;Share this article&lt;/button&gt;&lt;/li&gt;
&lt;/menu&gt;
</code></pre>
<h3 id="description-lists-li">Description lists <code>&lt;li&gt;</code></h3>
<p>Description lists are used for grouping terms and descriptions. For example, a glossary.</p>
<p>These lists are marked up using a  <code>&lt;dl&gt;</code>  parent element and  <code>&lt;dt&gt;</code> (specifying the term) and  <code>&lt;dd&gt;</code>  (specifying the description) child elements.</p>
<p>Code example:</p>
<pre><code>&lt;dl&gt;
	&lt;dt&gt;Fern&lt;/dt&gt;
	&lt;dd&gt;Green flowerless plants with divided leaves that tend to grow in damp, shady areas&lt;/dd&gt;
	&lt;dt&gt;Cactus&lt;/dt&gt;
	&lt;dd&gt;A type of desert plant that has thick, leafless stems covered in prickly spines or sharp spikes&lt;/dd&gt;
&lt;/dl&gt;
</code></pre>
<p><strong>Note</strong>: How description lists are exposed to different screen readers can vary. For this reason, there must be a clear relationship in the text between the term and the description. For more information, see Adrian Roselli’s article on <a href="https://codepen.io/aardrian/full/NzGaKP">how description lists are exposed to assistive technology</a>.</p>
<h3 id="exceptions">Exceptions</h3>
<p>In cases where native HTML cannot be used, the ARIA roles of ‘list’ and ‘listitem’ or ‘menu’ and ‘menuitem’ can be applied to elements to change the semantics. Refer to <strong>Building Elements with ARIA (Ta11y)</strong> for more information.</p>
<h2 id="best-practices">Best Practices</h2>
<h3 id="general-tips">General Tips</h3>
<ul>
<li>Keep lists concise.</li>
<li>Try to keep to one phrase or sentence per list item.</li>
<li>Avoid styling lists to display in-line (unless styling a horizontal menu), as this reduces readability.</li>
</ul>
<h3 id="multi-level-lists">Multi-Level Lists</h3>
<p>Try to avoid multi-level lists, as they can be hard for people to follow. If you do use a multi-level list, try to limit it to two levels and use the same symbol, number, or letter for the same level in each list.</p>
<h3 id="grammatical-structure">Grammatical Structure</h3>
<p>It helps users if lists keep to the same grammatical structure. This means starting each list item with the same:</p>
<ul>
<li>word type (such as a noun or a verb)</li>
<li>tense (past, present, or future)</li>
<li>sentence type (such as instructions or a question).</li>
</ul>
<h2 id="how-to-test">How to Test</h2>
<p>Lists can be checked using the  <a href="https://accessibility-bookmarklets.org/install.html">lists bookmarklet</a>  or an accessibility test tool (browser extension) like WAVE or ANDI.</p>
<ul>
<li>Use the Details panel in  <a href="https://wave.webaim.org/extension/">WAVE</a>  to highlight all lists on a page.</li>
<li>Use the Structures module in  <a href="https://www.ssa.gov/accessibility/andi/help/install.html">ANDI</a>  and select the “lists” option to see all lists on a page. The lists option is only available if there are lists on the page.</li>
</ul>
<p>See  <a href="https://www.ta11y.org/learning/topic?key=test_tool.comprehensive_wave">Wave (Ta11y)</a>  and  <strong>ANDI (Ta11y)</strong>  for more information about using these tools.</p>
<p>![Screenshot of ANDI Table Test Results showing code and list items for the Breadcrumb Links list. Following text provides the full description][/astro/src/assets/images/webaccessibility-tablesandlists-lists-figure1.png]<br>
Figure 1: ANDI Test Results showing Breadcrumb Links List</p>
<p>In an example from this page in <a href="http://ta11y.org/">Ta11y.org</a>, the ANDI output for the Breadcrumb Links list shows the text of the three list items (Home, Learn about Accessibility, and Lists) and identifies the list as an ordered list. Cycling through the list would reveal information about each of the list items in the list.</p>
<p>Developers can check the source code for lists by using the  <strong>Browser Inspect / DevTools (Ta11y)</strong>.</p>
<ul>
<li>Check that everything that looks like a list is correctly coded as a list. Lists can be coded using native HTML elements (preferred) or ARIA. Refer to <strong>Building Elements with ARIA (Ta11y)</strong>  for more information.</li>
</ul>
<h2 id="resources">Resources</h2>
<ul>
<li><a href="https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html">WCAG Success Criterion 1.3.1 Info and Relationships (W3C)</a></li>
<li><a href="https://www.stylemanual.gov.au/structuring-content/lists">Lists (Australian Government Style Manual</a>)</li>
<li><a href="https://www.w3.org/TR/coga-usable/">Making Content Usable for People with Cognitive and Learning Disabilities (W3C)</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Counter_Styles/Using_CSS_counters">Using CSS counters (Mozilla Developer Network)</a></li>
<li><a href="https://webaim.org/techniques/semanticstructure/">Semantic Structure: Regions, Headings, and Lists (WebAIM)</a></li>
<li><a href="https://developers.google.com/tech-writing/one/lists-and-tables">Technical Writing: Lists and Tables (Google for Developers)</a></li>
</ul>

