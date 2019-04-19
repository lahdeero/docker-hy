FROM ubuntu:18.04

RUN apt-get update && apt-get install -y curl 
CMD sh -c 'echo "Input website:"; read website; echo "Searching.."; website=${website%$'\r'}; sleep 1; curl $website;'


