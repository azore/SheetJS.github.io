.PHONY: index.html
index.html:
	echo "<meta charset='utf-8'>" > $@
	echo "<ul>" >> $@
	git ls-files | while read x; do y=$$(node -pe 'encodeURIComponent("'"$$x"'")'); echo "<li><a href='$$y'>$$x</a></li>"; done >> $@ 
	echo "</ul>" >> $@
