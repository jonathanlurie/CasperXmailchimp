# CasperXmailchimp

A fork of the default Casper theme (made at v1.2.8), with Mailchimp subscription form.  
The form are displayed at two places:  

**The index page:**  

![](https://raw.githubusercontent.com/jonathanlurie/CasperXmailchimp/master/snapIndex.jpg)

**The tag page:**  

![](https://raw.githubusercontent.com/jonathanlurie/CasperXmailchimp/master/snapTag.jpg)

# Usage

The user just need to type his/her email address and press `Enter`. Then, the regular Mailchimp page opens to warn the user will have to confirm his subscription from an email that was just sent.

# Setup

Based on the *naked form* generated by Mailchimp, you need to replace the form and user ID within the page `index.hbs` and `tag.hbs`.  

Here is what a *naked form* looks like when freshly generated by Mailchimp:  

```html
<!-- Begin MailChimp Signup Form -->
<div id="mc_embed_signup">
<form action="//XXXX.XXXX.list-manage.com/subscribe/post?u=XXXXXXXXXXXXXX&amp;id=XXXXXXXXXXXX" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
    <div id="mc_embed_signup_scroll">

<div class="mc-field-group">
	<label for="mce-EMAIL">Email Address </label>
	<input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
</div>
	<div id="mce-responses" class="clear">
		<div class="response" id="mce-error-response" style="display:none"></div>
		<div class="response" id="mce-success-response" style="display:none"></div>
	</div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
    <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_181cdcb2cc1de5c3cc04be835_27649f5188" tabindex="-1" value=""></div>
    <div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
    </div>
</form>
</div>

<!--End mc_embed_signup-->
```

You need to use the `action` attribute of `form`:  
```html
<form action="//XXXX.XXXX.list-manage.com/subscribe/post?u=XXXXXXXXXXXXXX&amp;id=XXXXXXXXXXXX" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
```

and replace replace the *XXXX* values from `index.hbs` and `tag.hbs`, respectively line **20** and **25**.


## Copyright & License

Copyright (c) 2013-2016 Ghost Foundation - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
