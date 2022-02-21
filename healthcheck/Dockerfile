FROM alpine:3.12.0
//Este fue el cambio del código
RUN apk update && \
    apk add ruby ruby-json ruby-rdoc ruby-irb

RUN gem install awesome_print

COPY healthcheck.rb healthcheck.rb
ENTRYPOINT ["ruby", "healthcheck.rb"]
