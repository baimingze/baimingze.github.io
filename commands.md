
### new article(need to added posts attr mannually)
bundle exec middleman article "Launching my blog"


### publish all with gh-pages
bundle exec rake publish   ALLOW_DIRTY=true BRANCH_NAME=master

### publish one article
bundle exec rake publish source/posts/2015-06-07-are-you-ready-for-the-open-science.html.markdown  ALLOW_DIRTY=true BRANCH_NAME=master
