---
layout: posts
title: "Getting Started with Jekyll in Windows OS"
date: 2019-04-03
---

## Installing Ruby and Jekyll

1. Download and Install a **Ruby+Devkit** version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
2. Run the ```ridk install``` after ruby installation wizard. Install all 3 components because this is needed for installing gems with native extensions base from [**Ruby Installer Documentation**](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system).
3. To check which ruby and gem version installed in your computer, open command prompt and type ```ruby -v``` and ```gem -v```.
    +  If ```ruby``` is not recognized in your computer, go to Ruby bin folder and copy the directory path. By default it's directory path should be like this ```C:\Ruby26-x64\bin```.
    + Next step, go to ```Control Panel\System and Security\System``` and open **Advanced System Settings**. Click on **Environment Variables** and double-click ```Path``` under **System Variables** to edit it.
    + Then add the **ruby path directory** by clicking **New** and pasting the copied ruby bin directory. Then click OK and apply changes to run ```ruby``` command.
4. Then open command prompt to install Jekyll and Bundler via: ```gem installer jekyll bundler```. The following text will be displayed during installation.

```plaintext
C:\Users\IAmCarl>gem install jekyll bundler
Fetching em-websocket-0.5.1.gem
Fetching http_parser.rb-0.6.0.gem
Fetching eventmachine-1.2.7-x64-mingw32.gem
Fetching sassc-2.2.1-x64-mingw32.gem
Fetching jekyll-watch-2.2.1.gem
Fetching jekyll-sass-converter-2.1.0.gem
Fetching listen-3.2.1.gem
Fetching kramdown-2.1.0.gem
Fetching kramdown-parser-gfm-1.1.0.gem
Fetching liquid-4.0.3.gem
Fetching mercenary-0.3.6.gem
Fetching forwardable-extended-2.6.0.gem
Fetching pathutil-0.16.2.gem
Fetching rouge-3.17.0.gem
Fetching safe_yaml-1.0.5.gem
Fetching unicode-display_width-1.7.0.gem
Fetching jekyll-4.0.0.gem
Fetching terminal-table-1.8.0.gem
Successfully installed colorator-1.1.0
Temporarily enhancing PATH for MSYS/MINGW...
Building native extensions. This could take a while...
Successfully installed http_parser.rb-0.6.0
Successfully installed eventmachine-1.2.7-x64-mingw32
Successfully installed em-websocket-0.5.1
Successfully installed sassc-2.2.1-x64-mingw32
Successfully installed jekyll-sass-converter-2.1.0
Successfully installed listen-3.2.1
Successfully installed jekyll-watch-2.2.1
Successfully installed kramdown-2.1.0
Successfully installed kramdown-parser-gfm-1.1.0
Successfully installed liquid-4.0.3
Successfully installed mercenary-0.3.6
Successfully installed forwardable-extended-2.6.0
Successfully installed pathutil-0.16.2
Successfully installed rouge-3.17.0
Successfully installed safe_yaml-1.0.5
Successfully installed unicode-display_width-1.7.0
Successfully installed terminal-table-1.8.0
-------------------------------------------------------------------------------------
Jekyll 4.0 comes with some major changes, notably:

  * Our `link` tag now comes with the `relative_url` filter incorporated into it.
    You should no longer prepend  site.baseurl to foo.md
    For further details: https://github.com/jekyll/jekyll/pull/6727

  * Our `post_url` tag now comes with the `relative_url` filter incorporated into it.
    You shouldn't prepend  site.baseurl to post_url 2019-03-27-hello
    For further details: https://github.com/jekyll/jekyll/pull/7589

  * Support for deprecated configuration options has been removed. We will no longer
    output a warning and gracefully assign their values to the newer counterparts
    internally.
-------------------------------------------------------------------------------------
Successfully installed jekyll-4.0.0
Parsing documentation for colorator-1.1.0
Installing ri documentation for colorator-1.1.0
Parsing documentation for http_parser.rb-0.6.0
unknown encoding name "chunked\r\n\r\n25" for ext/ruby_http_parser/vendor/http-parser-java/tools/parse_tests.rb, skipping
Installing ri documentation for http_parser.rb-0.6.0
Parsing documentation for eventmachine-1.2.7-x64-mingw32
Installing ri documentation for eventmachine-1.2.7-x64-mingw32
Parsing documentation for em-websocket-0.5.1
Installing ri documentation for em-websocket-0.5.1
Parsing documentation for sassc-2.2.1-x64-mingw32
Installing ri documentation for sassc-2.2.1-x64-mingw32
Parsing documentation for jekyll-sass-converter-2.1.0
Installing ri documentation for jekyll-sass-converter-2.1.0
Parsing documentation for listen-3.2.1
Installing ri documentation for listen-3.2.1
Parsing documentation for jekyll-watch-2.2.1
Installing ri documentation for jekyll-watch-2.2.1
Parsing documentation for kramdown-2.1.0
Installing ri documentation for kramdown-2.1.0
Parsing documentation for kramdown-parser-gfm-1.1.0
Installing ri documentation for kramdown-parser-gfm-1.1.0
Parsing documentation for liquid-4.0.3
Installing ri documentation for liquid-4.0.3
Parsing documentation for mercenary-0.3.6
Installing ri documentation for mercenary-0.3.6
Parsing documentation for forwardable-extended-2.6.0
Installing ri documentation for forwardable-extended-2.6.0
Parsing documentation for pathutil-0.16.2
Installing ri documentation for pathutil-0.16.2
Parsing documentation for rouge-3.17.0
Installing ri documentation for rouge-3.17.0
Parsing documentation for safe_yaml-1.0.5
Installing ri documentation for safe_yaml-1.0.5
Parsing documentation for unicode-display_width-1.7.0
Installing ri documentation for unicode-display_width-1.7.0
Parsing documentation for terminal-table-1.8.0
Installing ri documentation for terminal-table-1.8.0
Parsing documentation for jekyll-4.0.0
Installing ri documentation for jekyll-4.0.0
Done installing documentation for colorator, http_parser.rb, eventmachine, em-websocket, sassc, jekyll-sass-converter, listen, jekyll-watch, kramdown, kramdown-parser-gfm, liquid, mercenary, forwardable-extended, pathutil, rouge, safe_yaml, unicode-display_width, terminal-table, jekyll after 108 seconds
Fetching bundler-2.1.4.gem
Successfully installed bundler-2.1.4
Parsing documentation for bundler-2.1.4
Installing ri documentation for bundler-2.1.4
Done installing documentation for bundler after 45 seconds
20 gems installed

C:\Users\IAmCarl>jekyll -v
jekyll 4.0.0

C:\Users\IAmCarl>
``` 
5. Check if Jekyll installed properly: ```jekyll -v```

That’s it, you’re ready to use Jekyll!

## Create a New Site

It’s time to create a site!

1. Create a new directory for your site, you can name it whatever you’d like. 
2. Then add your first file, for example create ```index.html```.

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
</head>
<body>
	<h1>Hello World From Jekyll!</h1>
</body>
</html>
```     
3. Then **build** the site to output static site to a directory called ```_site```.

```plaintext
D:\Jekyll_Sites\firstsite>jekyll build

Configuration file: none
            Source: D:/Jekyll_Sites/firstsite
       Destination: D:/Jekyll_Sites/firstsite/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 0.094 seconds.
 Auto-regeneration: disabled. Use --watch to enable.
 ``` 

4. Then run local web server, be default jekyll web server run in port **4000**, in order to browse the site go to **[http://localhost:4000/](http://localhost:4000/)**.

```plaintext
D:\Jekyll_Sites\firstsite>jekyll serve
Configuration file: none
            Source: D:/Jekyll_Sites/firstsite
       Destination: D:/Jekyll_Sites/firstsite/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 0.13 seconds.
  Please add the following to your Gemfile to avoid polling for changes:
    gem 'wdm', '>= 0.1.0' if Gem.win_platform?
 Auto-regeneration: enabled for 'D:/Jekyll_Sites/firstsite'
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```
> **Note:** To run Jekyll in different port use  ```jekyll serve --port 4001 --host my_hostname_or_ip``` or put ```port:4001``` in your **_config.yml**.

That’s it, you’re site is running via Jekyll!

**References:**

[https://jekyllrb.com/docs/installation/windows/](https://jekyllrb.com/docs/installation/windows/)  
[https://jekyllrb.com/docs/step-by-step/01-setup/](https://jekyllrb.com/docs/step-by-step/01-setup/)    
[https://jekyllrb.com/docs/configuration/options/#serve-command-options](https://jekyllrb.com/docs/configuration/options/#serve-command-options)    
[https://stackoverflow.com/questions/25650749/is-it-possible-to-serve-multiple-jekyll-sites-locally](https://stackoverflow.com/questions/25650749/is-it-possible-to-serve-multiple-jekyll-sites-locally)