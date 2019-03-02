# Accessibility Learning Plan for Developers

## Purpose

This learning plan is designed to provide web developers who are accessibility beginners with a plan and actionable goals for the journey of learning. It provides focus and a timeline rather than aimlessly searching tutorials. I've copied the format from [Anton Ball's Typescript Learning Plan](https://medium.com/@antonball/planning-to-learn-225fc7817394).

### What's a learning plan?

Wikipedia does a great job of defining what a [learning plan](https://en.wikipedia.org/wiki/Learning_plan) is.

## Goal

The goal of the learning plan is not to teach accessibility but provide the plan and resources in order to learn. The plan has a clear stopping point - the scope is basic accessible web development skills. This plan does not cover app development, which uses different code and techniques, although the underlying principles are the same. 

When you've completed the plan, you will be able to create basic accessible content and make a well-informed choice when reviewing more advanced plugins and tools which claim to be accessible. 

## Prerequisites

A basic understanding of front-end web development is assumed.

## Resources

These resources will be useful in this learning plan. There are many others which you may prefer. Suggestions welcome!

-   [WCAG 2.1 documentation](https://www.w3.org/TR/WCAG21/)
-   [The A11y Project](https://a11yproject.com/)
-   [WAI tutorials](https://www.w3.org/WAI/tutorials/)

## Tools
-   [Chrome Accessibility Tools (extension)](https://chrome.google.com/webstore/detail/accessibility-developer-t/fpkknkljclfencbdbgkenhalefipecmb?hl=en) and/or [Firefox Accessibility Tool](https://developer.mozilla.org/en-US/docs/Tools/Accessibility_inspector)
-   Lea Verou's [Contrast Ratio tool](https://contrast-ratio.com/) or other contrast checking tool
-   [NVDA](https://www.nvaccess.org/) to be used on Firefox/Windows or VoiceOver on [Safari/iOS](https://www.apple.com/accessibility/iphone/vision/) or [Safari/Mac](https://www.apple.com/accessibility/mac/vision/)

## What is accessibility?

Accessibility is a property of all websites, web apps or software apps. Some are more accessible than others. 

"Being accessible is about making your website, with all of its data and functions, available for anyone, no matter how they have to use your website." - Katie Cunningham, Accessibility Handbook (O’Reilly)

-   [What we mean when we talk about accessibility](https://accessibility.blog.gov.uk/2016/05/16/what-we-mean-when-we-talk-about-accessibility-2/) by Alastair Duggin for Gov.UK
-   [Google's Web Fundamentals: Accessibility Overview](https://developers.google.com/web/fundamentals/accessibility/)
-   [Web Accessibility Initiative at W3C: Introduction to Web Accessibility](https://www.w3.org/WAI/fundamentals/accessibility-intro/)

## Learning Plan

(Times are wild guesstimates)

<table>
	<thead>
		<tr>
			<th>Goal</th>
			<th>Time</th>
			<th>Task/Projects/Activities</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Writing semantic HTML</td>
			<td>One Day</td>
			<td>
        <p>Writing semantic HTML makes all other accessible development techniques much easier. It is the foundation of your ability to write code which can be translated and transformed by the user and their chosen software into a format which works for their needs. </p>
				<ul>
          <li><a href="https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML">Accessible HTML</a> at Mozilla Developer Network (MDN)</li>
					<li><a href="https://developers.google.com/web/fundamentals/accessibility/semantics-builtin/">Semantics built-in</a> at Google's Web Fundamentals</li>
          <li><a href="https://medium.com/@mandy.michael/understanding-why-semantic-html-is-important-as-told-by-typescript-bd71ad41e6c4">Why semantic HTML is important, as told by TypeScript</a> or <a href="https://medium.com/@mandy.michael/building-websites-for-safari-reader-mode-and-other-reading-apps-1562913c86c9">Building websites for Safari Reader Mode and other reading apps</a> by Mandy Michael.</li>
					<li>Web Accessibility Initiative (WAI) tutorial on <a href="https://www.w3.org/WAI/tutorials/page-structure/">Page Structure</a></li>
				</ul>
        <p>Activity: recreate a content-heavy page (try a page from Wikipedia or documentation of a framework you use) using semantic HTML. Use the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element">MDN HTML element reference</a> rather than the articles above if you need to find out what element to use.</p>
			</td>
    </tr>
		<tr>
			<td>Creating accessible styles</td>
			<td>Half day</td>
			<td>
         <p>Accessible designs are out of scope for this learning plan. But we need to know how to implement them using the right techniques.</p> 
				<ul>
          <li><a href="https://www.sitepoint.com/cant-rely-color/">We can't rely on colour</a> by James Edwards for SitePoint</li>
          <li><a href="https://css-tricks.com/focusing-on-focus-styles/">Focusing on focus styles</a> at CSS Tricks</li>
          <li><a href="https://developers.google.com/web/fundamentals/accessibility/accessible-styles">Accessible styles</a> at Google's Web Fundamentals</li>
          <li>In theory, most front-end web developers know how to make responsive designs already. But if you need a refresher or weren't taught it well, <a href="https://bradfrost.github.io/this-is-responsive/resources.html">Brad Frost's Responsive Resources</a> has everything you need.</li>
				</ul>
          <p>Activity: make sure your content page is repsonsive and add focus styles to any links or buttons. Use a contrast ratio tool to check the page and make fixes if needed. Add <pre>body {filter : grayscale(100%);}</pre> to the CSS to check if you have relied on colour alone for any visual indicators, and fix any problems.</p>
			</td>
		</tr>
    <tr>
      <td>Making images accessible</td>
      <td>Two hours</td>
      <td>
        <p>Images often have some of the most useful information on a page. It's important to make sure that information is conveyed to all users, not just those with good vision.</p>
        <ul>
          <li>WAI has an excellent <a href="https://www.w3.org/WAI/tutorials/images/">tutorial about all aspects of image accessibility</a>.</li>
          <li>More detail on the accessibility of <a href="https://www.24a11y.com/2017/svg-icon-fonts-accessibility-case-study/">SVGs and icon fonts</a> at 24 Accessibility</li>
        </ul>
        <p>Activity: find a website with a lot of images in content, like for an art gallery or a band website. Write out the alt text you'd use for each one, and why. Repeat for a web app which uses lots of icons on it's controls, like email or video services.</p>
      </td>
</tr>
        <tr>
			<td>Learn the hiding methods</td>
			<td>One hour</td>
			<td>
                <p>Dynamic sites and common widgets let users show and hide chunks of content. The method you choose for hiding makes a big difference to how accessible your site is to keyboard and screen reader users.</p>
				<ul>
					<li><a href="https://a11yproject.com/posts/how-to-hide-content/">How to hide content</a> at The A11y Project</li>
				</ul>
                <p>Activity: Make a page with chunks of content, some with links or buttons in them. Experiment with HTML and CSS methods of hiding content. Compare the results in the browser, in dev tools, with a keyboard and with a screen reader.</p> 
			</td>
		</tr>
		<tr>
			<td>Build an accessible drop-down menu</td>
			<td>Half day</td>
			<td>
                <p>Site navigation brings together accessibility requirements, so it makes a good practice feature.</p>
				<ul>
					<li>Read the WAI <a href="https://www.w3.org/WAI/tutorials/menus/">Menus tutorial</a></li>
				</ul>
                <p>Activity: create a flyout or dropdown menu. When you are done, compare it to the examples given at <a href="https://codepen.io/svinkle/pen/aEVwWd">The A11y Project</a> or Heydon Pickering's <a href="https://inclusive-components.design/menus-menu-buttons/">Inclusive Components</a>. How would you make yours responsive?</p>
			</td>
		</tr>
		<tr>
			<td>Build an accessible form</td>
			<td>Half day</td>
			<td>
                <p>There's more to accessible forms than choosing semantic elements. We now have to make use of the right attributes, and consider how screen reader software behaves differently inside form elements.</p>
				<ul>
                    <li><a href="https://alistapart.com/article/sensibleforms">Sensible form design</a> at A List Apart</li>
                    <li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/autocomplete">Autocomplete attributes</a> for frequently-typed information are now an essential part of most forms.</li>
					<li><a href="https://24ways.org/2018/inclusive-considerations-when-restyling-form-controls/">Inclusive considerations when styling form controls</a> by Scott O'Hara for 24 Ways</li>
				</ul>
                <p>Activity: Follow pages 1 to 4 of the <a href="https://www.w3.org/WAI/tutorials/forms/">WAI forms tutorial</a> to make a short form using a variety of input types and groups. Make sure they are all labelled correctly, and provide information about required fields and instructions. (Error messaging is the next lesson!)</p>
			</td>
		</tr>
		<tr>
			<td>Providing accessible error messages</td>
			<td>Half day</td>
			<td>
                <p>Giving your users accessible error messages has a number of potential pitfalls to avoid. We want to make it as easy as possible for everyone to recover from their mistake and finish their task.</p>
				<ul>
					<li><a href="https://www.slideshare.net/maxdesign/accessible-hints-and-error-messages">Accessible hints and error messages</a> by Russ Weakley</li>
                    <li><a href="https://www.nngroup.com/articles/errors-forms-design-guidelines/">How to report errors in forms: 10 design guidelines</a> at Nielsen Norman Group</li>
                    <li><a href="https://intopia.digital/articles/default-browser-error-messages/">Don't rely on browser-default error messages</a> by me for Intopia</li>
				</ul>
                <p>Activity: Use <a href="https://www.w3.org/WAI/tutorials/forms/validation/">pages 4 and 5 of the WAI forms tutorial</a> to add validation and error messages to your form from last week. Test it with a screen reader, in high contrast, and on a small screen.</p>
			</td>
		</tr>
<tr>
<td>Quick and dirty testing</td>
<td>Two hours</td>
<td>
  <p>Quick testing is useful to confirm that the information you want to convey to all users is actually available to all users. It cannot replace a full audit by an accessibility specialist, or usability testing by people with disabilities. But you can check that your work is of good-enough quality to hand over for a proper quality assurance process.</p>
  <ul>
    <li><a href="https://a11yproject.com/#Quick-tests">Quick tests</a> from The A11y Project</li>
    <li>Check that all information is present in the accessibility tree using either <a href="https://developer.mozilla.org/en-US/docs/Tools/Accessibility_inspector">Firefox's Accessibility Inspector</a> or <a href="https://developers.google.com/web/tools/chrome-devtools/accessibility/reference#pane">Chrome's Accessibility pane in dev tools</a></li> 
    <li>Lea Verou's [Contrast Ratio tool](https://contrast-ratio.com/) or The Paciello Group's [Colour Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/) can be used to check the colours of your site. Don't forget content which is hidden on page load!</li>
    <li>The A11y Project also has very basic instructions for using <a href="https://a11yproject.com/#Assistive-technology">assistive technology</a> (at the moment, free screen readers). </li>
  </ul>
  <p>Activity: perform these tests on the pages you've made during this learning plan. Use the resources linked in this plan (or Stack Overflow) to find solutions to any problems you come across.</p>
</td>
</tr>
</tbody>
</table>
