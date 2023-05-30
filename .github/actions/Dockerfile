FROM ubuntu:focal

LABEL "com.github.actions.name"="Send Webex Message to Room"
LABEL "com.github.actions.description"="Send a message to the given room on Webex"
LABEL "com.github.actions.icon"="message-circle"
LABEL "com.github.actions.color"="orange"

LABEL "repository"="http://github.com/roddyd94/swm-gha-workshop-beginners"
LABEL "homepage"="http://github.com/roddyd94"
LABEL "maintainer"="Gyeongyong Park <pky941129@gmail.com>"

# Install curl
RUN apt-get update && apt-get install -y \
    sudo \
    curl \
 && rm -rf /var/lib/apt/lists/*

ADD entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]