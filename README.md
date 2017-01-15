#Subbscribe

### Requirements

I tried to keep it as light as possible. The only thing you need to is `jQuery` and a MailChimp or CampaignMonitor form with  the default name and email fields.

### How to use

It's really easy to get started. First you need to include the required libraries at the bottom of your HTML page:

```
<script src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
<script src="subbscribe.min.js"></script>
```

And the CSS file at the head:

```
<link rel="stylesheet" href="subbscribe.css" />
```

Then, you can initialise the plugin using the document’s body as the container, passing your list and form url parameters.

```
$('body').subbscribe({
    list: "MailChimp",
    url : "//1bytebeta.us9.list-manage.com/subscribe/post?u=1c261e60d8259c0c636801494&amp;id=7fa99bf359"
});
```

The list and form’s URL are **required**. The plugin will log an error if they are not provided.

### Options

`list` - 'MailChimp' or 'CampaignMonitor'

`delay` - Dispatch the slide in after X number of seconds

`url` - Your MailChimp/CampaignMonitor form URL. You can get it from the form embed script under the action attribute.

`title` - The window title.

`text ` - The text that will show up above the form when a user click to subscribe.

`name` - The name that will show up next to the thumbnail. This could be a link to a Twitter handle.

`color` - The color of the button.

`thumbnail` - A path to the thumbnail you wish to include. Make sure it’s a square as the plugin will scale it down to 40x40px

`emailonly` - If set to true, the name field will not be included in the opt-in form.

`cm_mail_field` - If CampaignMonitor is used as client, a CM mail field should be provided.

### Callbacks

`onClose` - Called when someone close the pop-up without subscribing.

`onSubbscribe` - Called when someone completed his subscription.

### License

The MIT License

Copyright (c) 2012-2015 1Byte Beta hello@1bytebeta.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
