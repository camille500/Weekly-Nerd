# Developing for the blind
Bram Duvigneau is an accessibility researcher and web developer whom gave one of our weekly nerd sessions. It’s not just a developer, Bram is a blind developer and a good one.
After his talk, I became more interested in the web for blind people. This article will teach you more about what is important when developing for this specific target audience.

## How blind people use the web
It’s pretty obvious that blind people can’t read and see the content that’s on your website. For us, the seeing, it’s natural to just open a website and get good structured content. But for the blind that is a different story. They can’t see, so they have to listen to what is on your website. To make this possible, most of them use a screen reader and more often than not a so-called braille display. But when you build your last project, did you take this into account? There is a chance you didn’t, then this is a perfect article for you. Why? Because there are an estimated 285 million visually impaired people on the planet, from which around 39 million totally blind (World Health Organization, 2014).

As read above, most of the blind people surfing the internet are using a screen reader. A screen reader is a software application that enables people with visual impairments to use the web. The software works together with the users Operation System and other software to give them information about for example images, menus, content on a website and buttons (Watson, 2015).

## How developers can help the visually impaired

Screen readers start with the language of the webpage. This can be set using the language attribute. This attribute can say something about a part of the website, for example in a section element ```<section lang=”en”> .. </section> ```, but is commonly used for the whole website inside the HTML tag ```<html lang=”en”> .. </html>```.

Users with screen readers use the Tab key to navigate through your website. It is important that all content is well organized. Your menu items need to be in a logic order and the user should get the option to skip the whole navigation or parts of it.

The next thing you should take into consideration are the headings of the webpage. People with a screen reader get the option to navigate from header to header. It’s really important to make sure that your headers are in the right order. In that way people can easily hear what are all the headlines so they can skip to the part that is most interesting for them without going through all the in-between content.

## What about images?
It’s easy to say that blind people can’t see any of the images on your website. But how can you make them interesting for people with a screen reader? Just use the alt attribute. By giving a short description about the image within the context of a website, blind or visually impaired people can still understand the meaning of it.
There is another way to do this as well, the aria-label. This is an attribute you can add to almost all HTML elements on a page. Let’s say you have three buttons below a field. One of them is used to delete the form, the other to edit the form’s content and the last one to send the form’s content to the server. If you have no description of what these buttons do, the screen reader will just tell you it’s a button. But by using the aria-label attribute you can declare what these buttons are for.

Now we’ve added an aria-label to the button for sending the form. The aria-label is like this: ```<input type=”submit” aria-label=”Send the application”>```. If you tab trough the buttons right now, the user will hear what the button can be used for!

# Sources

- Watson, L. (2015, 11 22). What is a Screen Reader? Retrieved 06 2017, 27, from Nomensa: https://www.nomensa.com/blog/2005/what-screen-reader
- World Health Organization. (2014, 08). Visual impairment and blindness. Retrieved 06 28, 2017, from World Health Organization: http://www.who.int/mediacentre/factsheets/fs282/en/
