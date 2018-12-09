FROM debian:stable-slim

LABEL "name"="sh"
LABEL "maintainer"="GitHub Actions <support+actions@github.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="cURL for GitHub Actions"
LABEL "com.github.actions.description"="Runs cURL in an Action"
LABEL "com.github.actions.icon"="upload"
LABEL "com.github.actions.color"="green"

COPY LICENSE README.md THIRD_PARTY_NOTICE.md /

COPY entrypoint.sh /entrypoint.sh

RUN apt-get update && apt-get install curl -y

ENTRYPOINT ["/entrypoint.sh"]

