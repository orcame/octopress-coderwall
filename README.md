octopress-coderwall
==============================

Display coderwall badges on the awesome blog system Octopress 

## Octopress Aside Plugin For Coderwall

A plugin of [Octopress](http://octopress.org/) used for display your badges on coderwall.

### Installation

Get the plugin
```bash
git clone git@github.com:orcame/octopress-coderwall.git
cd octopress-coderwall
cp coderwall.html /root_of_your_blog/source/_includes/asides/
cp coderwall.js /root_of_your_blog/source/javascript/
```

Config your  ```_config.yml``` file.

1. add `asides/coderwall.html` to your default_asides array. 
2. add the following configuration to the end of your ```_config.yml``` file.

```yaml

# Display coderwall badges
coderwall_user: your_coderwall_user_name
coderwall_show_profile_link: true #show your profile link on coderwall.

```

Preview and deploy(if you want)
```bash
rake generate
rake preview # after this, access http://localhost:4000 to view your blog
rake deploy

``` 
**Notice:** This plugin is worked fine on my theme(based on bootstrap), maybe you need adjust some class value or other code on your own theme. You can just reference this code.


