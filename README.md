
jsdelivr_cdn:
  # If use_cdn is false, this plugin will not work
  use_cdn: true 

  # If deploy_when_generating is true, the assets repository will be pushed to github every time you generate the hexo project using 'hexo g' command. If this flag is set false, the repository will be pushed when deploying. You can manually push the assets repository to github when generating by using 'hexo g cdn' command.
  deploy_when_generating: true

  # cdn_url_prefix is the jsdelivr cdn url of your github repository(the assets repository for static assets rather than the hexo project deployment repository), it should be like: https://cdn.jsdelivr.net/gh/<username for github>/<assets repo name>/
  cdn_url_prefix: <the url of jsdelivr cdn for your github repository>

  # git_repo_url is the url of your new assets repository on github, it should be like git@github.com:<username>/<repo>.git
  git_repo_url: <git repository url>
  
  # you can use github token to push your assets repository. If you don't want to use a token, you can use a empty string '' or comment out this line. We do not recommand that you directly write your token in the _config.yml. We suggest that you read the token from the environment variable by setting token with a prefix '$'. e.g. '$GITHUB_TOKEN'. When you want to use token, you must use http(s) link of your repo. More information about github token can be found in https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line.
  token: <your github auth token, optional>

  # The path of an asset directory in asset_dirs should be the relative path to your hexo project directory, e.g. assets or source/assets or themes/<theme name>/assets. If you only want to use the cdn for the images in your posts, you can leave asset_dirs as empty
  asset_dirs:
    - [assets directory]
    - [another assets directory]
# images
