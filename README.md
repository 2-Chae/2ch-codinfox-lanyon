# 2ch-codinfox-lanyon
This is a jekyll template based on [Codinfox-Lanyon](https://github.com/codinfox/codinfox-lanyon). You can see the live demo [here](https://2-chae.github.io/).

If you like my template, please give me a star :)
You can copy this template easily by pressing Fork button.

All the configurations are inside either `_config.yml` or `_config.scss`. The options are fairly straightforward.
You can refer additional explanation on [Codinfox's Github](https://github.com/codinfox/codinfox-lanyon).

Please understand that I am not a web developer so codes are kind of mess. :)

## Category

I just changed an architecture.  
So the most notable difference compared to Codinfox is category.

If you want to create a new category, you have to make a new file in the category directory. (like mycat.md)
The content of the file should start like this..
```
---
layout: category
title:  MyCat
tags : 'tag1,tag2,hihi'
---
```

You can write tags which you want to show on the top of the category page. 

and then you also have to write tags in your post like this.
```
---
layout: post
title: Introducing Lanyon
tags: ['tag1','tag3']
categories: 'MyCat'
---
```

You can understand better when you see an example code I provide.

## Error
If you got the following error message during installing,

```
An error occurred while installing eventmachine (1.2.7), and Bundler cannot continue.
```

Try the code below,
```
gem install eventmachine -- --with-openssl-dir=/usr/local/Cellar/openssl@1.1/1.1.1h
```

Then, try `bundle install` again.

## License
Open sourced under the [MIT license](https://github.com/2-Chae/2ch-codinfox-lanyon/blob/master/LICENSE).
