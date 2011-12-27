# jQuery hanzi2pinyin
fast [hanzi](http://en.wikipedia.org/wiki/Hanzi) to [pinyin](http://en.wikipedia.org/wiki/Pinyin) conversion
## Examples
### DOM
	// Hanzi in $('#hanzi') will convert to pinyin and put to $('#pinyin')
	$('#hanzi').hanzi2pinyin({target:'#pinyin'});
### String
	// This brings the same effect as above:
	$('#pinyin').val($('#hanzi').val().hanzi2pinyin());
	
	// HanZi
	alert('汉字'.hanzi2pinyin({'case':'proper',hyphen:''}));
## Options
* **target** - selectors will contain the results
* **hyphen** - the hyphens between pinyins
* **'case'** - can be *lower*, *upper* or *proper* (*title*) case *(Note: adding quotes around case is necessary for IE browsers)*
* **punctuation_marks** - you can *remove* or *ignore* the Chinese punctuation marks or even *replace* them with corresponding English punctuation marks