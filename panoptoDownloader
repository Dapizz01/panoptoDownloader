#!/bin/bash
while IFS= read -r line
do
	link=$(curl $line | pup 'meta[name="twitter:player:stream"] attr{content}')
	title=$(curl $line | pup 'meta[property="og:title"] attr{content}')
	$(wget -O $2/"$title" $link)
done < "$1"
