####
#docker run --rm -p 127.0.0.1:4567:4567 --name gollum -v /home/seb/depots_git/gollum/:/home/gollum -d   gollum:latest

FROM ruby:2.7
RUN apt-get -y update && apt-get -y install libicu-dev cmake git && rm -rf /var/lib/apt/lists/*
RUN gem install github-linguist
RUN gem install gollum
RUN gem install org-ruby  # optional
WORKDIR /wiki
ENTRYPOINT ["gollum","--port","4567","--base-path","/"]
EXPOSE 4567
