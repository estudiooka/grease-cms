GREASE CMS
=====

Just code and dance.  
A fast and simple markdown file-based CMS developed with Silex and Symfony Components and templating with twig.

# GREASE 1.0 DOCUMENTATION

### Cache

Grease will cache all the rendered pages and server the straight on.
Disable the cache editing config/settigns.yml or renaming the file /sites/*/content/cache.md to something else.
Clean all cache renaming the cache.md file to clean.md.

### Twig Filters

```
placeholder     
css_tag     
js_tag"       
image_tag      
lorem      
```

### Twig Functions
- region($url)
- stream($url)
- getPage($url)


### Twig Page Variables

```
[page] => Array
    (
        [url] => default
        [file_path] => 1.default/
        [slug] => default
        [permlink] => http://grease.cms/default
        [has_children] => 1
        [children] => Array
            (
                [subpage] => 1.default/1.subpage
            )
        [data] => Array
            (
                [content] => markdown
                [layout] => default
                [title] => Default
                [description] => This description will go in the meta description tag
                [custom] => Custom Variable
                [anothercustom] => Another custom Variable
            )
        [files] => Array
            (
                [index.md] => http://grease.cms/sites/default/content/pages/1.default/index.md
            )
        [images] => Array
            (
            )                
        [videos] => Array
            (
            )
    )
[theme] => Array
    (
        [url] => http://grease.cms/sites/default/themes/
        [path] => /Volumes/SATA/Sites/_apps/grease/sites/default/themes/
        [css] => http://grease.cms/sites/default/assets/css/
        [js] => http://grease.cms/sites/default/assets/js/
        [img] => http://grease.cms/sites/default/assets/img/
    )
```


### Avaliable Events ( for plugin develpment)

- before_twig_options
- after_load_plugins
- after_url
- before_vars
- on_vars
- before_render
- after_render
- before_cache
- before_output
- after_output


## Libraries

- Silex
- Twig
- Pimple
- Symfony Components
- Moust Cache
- PHP Markdown & Extra

## Credits
- Fabio Luis
- Estúdio OKA
