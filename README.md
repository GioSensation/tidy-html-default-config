Tidy HTML Default Config
========================

*Tidy Html default config for the modern workflow*

Did you know your Mac has an *html beautifier* built-in? It's called **Tidy** and was built a while ago by a fine guy by the name of [Dave Raggett](http://en.wikipedia.org/wiki/Dave_Raggett). Today you have it pre-installed on your Mac and you can use it via the command line or install it as a service.

If commando is not your style and you are more a gui-guy, you can go [here](http://www.pixelfreak.net/tidy_service/), download the package (by another fine man: Scott Ahten) and copy the `TidyService.service` file onto `~/Library/Services/` (if the folder is not there, go ahead and create it).

If you need more help, you can read the original [Tidy Service readme page](http://www.pixelfreak.net/tidy_service/readme.html).

Three things to note here:

1. the service will not be available for you until you **logout or restart your Mac**;
2. in order for the service to run properly, your Mac needs to be able to run apps by **unidentified developers**. If you receive a warning saying that the app won't run because is from an unknown developer, just go to `Preferences > Security & Privacy > General` and accept apps from everywhere (I am sure someone will have a better solution for this, but I don't; the only hint is you can reenable the security setting after the service has run once -> peace of mind);
3. before using it, you might need to **activate the service** from your Mac's global Preferences: go to Preferences, then Keyboard, then go to the Abbreviations tab and find Services on the left column. From there you can scan through the services and find Tidy Markup. Check that and you are good to go.

Now, every time you have a piece of compressed html, just select it, right click `Services > Tidy Markup`. Boom! Beautified in an instant.

Wait, what! *The output is a mess*: no indentation, a `doctype` added, crazy wrap rules applied.

Here is why I created this repository. Using my config file here you will have a nice, **clean output**, with 4 spaces indentation (Tidy html does not allow to use tabs as far as I know) and no weird things added.

How do you use the file? Simply **copy it in your home folder** (`~` – or if you are a Mac beginner: `/Users/YOUR-USER-NAME-HERE/`). As simple as that.

Of course you can customize it to your heart's content using the options listed on [Tidy's man page](http://tidy.sourceforge.net/docs/tidy_man.html).

Please, note that the config file **also works with the command line version** of the tool.

Hope this helps.
