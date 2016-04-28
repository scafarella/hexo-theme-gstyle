# hexo-theme-gstyle
a googl style hexo theme.

##features
### smooth page transition
all pages are loaded async by using [smoothsate](http://smoothstate.com/).
and pages are preloaded before you visit them, super fast!
no blank between page switch!

### responsive
totaly responsive, mobile first.
no bootstrap, using modern css3 flex!
![hexo-theme-gstyle responsive screenshot]()

### impressing navigation
full screen morphing navigation on mobile
![full screen navigation menu with morphing animation](https://raw.githubusercontent.com/wayou/hexo-theme-gstyle/master/source/img/nav.gif)

### graceful table of content module
auto generated table of content with transition animation when expanding and collapsing.
![full screen navigation menu with morphing animation](https://raw.githubusercontent.com/wayou/hexo-theme-gstyle/master/source/img/toc.gif)

## how to use
- `git clone https://github.com/wayou/hexo-theme-gstyle.git themes/gstyle`
- config site `_config.yml` `theme: gstyle`

## using relative assets path in your post
- enable `post_asset_folder` in your hexo site config file `_config.yml`
- install `hexo-filter-pathfix` to fix the path of assets `npm install --save hexo-filter-pathfix`
- then you can using relative path when writing posts like `![image title](image_name.jpg)`.

## config

### comments
implemented 2 comments vendor, choose one you like.
``` yml
duoshuo_shortname: #your duoshuo shortname goes here
disqus_shortname: #your disqus shortname goes here
```

### site analytics
the `baidu_analytics` is mainly for mainland users. you can get the baidu analytics id from the admin page of baidu analytics code installing page.
![where to get the baidu analytics id](https://raw.githubusercontent.com/wayou/hexo-theme-gstyle/master/source/img/baidu_analytics.png)
``` yml
google_analytics:  
baidu_analytics: 
```

### image title
to enable image caption for iamges, install `hexo-image-caption` plugin by using this command:
```bash
npm i --save hexo-image-caption
```
and enable it in your hexo site config file `_config.yml` (not the theme config file).
```yml
image_caption: true
```

### sliding navigation indicator
whether to show an indicator for the active navigation menu item
```yml
active_nav: false
```

### known issues

- images may be empty after imagemin optimized. my suggestion is not to enable it at present
- enable page transition with smoothstate will cause the code in the post cannot scroll horizonally
