FROM node:lts

LABEL "com.github.actions.name"="Sync Glitch GitHub"
LABEL "com.github.actions.description"="Sync changes in your GitHub repository to glitch.com"
LABEL "com.github.actions.icon"="box"
LABEL "com.github.actions.color"="purple"

LABEL "repository"="https://github.com/glitch-tools/sync-glitch-github-action"
LABEL "homepage"="https://github.com/glitch-tools/sync-glitch-github-action"
LABEL "maintainer"="Sam Yamashita <1587053+sotayamashita@users.noreply.github.com>"

ADD entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
