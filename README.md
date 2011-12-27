# jQuery hanzi2pinyin
fast [hanzi](http://en.wikipedia.org/wiki/Hanzi) to [pinyin](http://en.wikipedia.org/wiki/Pinyin) conversion
## Examples
### DOM
	// Hanzi in $('#hanzi') will convert to pinyin and put to $('#pinyin')
	$('#hanzi').hanzi2pinyin({target:'#pinyin'});
### String
	// This brings the same effect as above:
	$('#pinyin').val($('#hanzi').val().hanzi2pinyin());