# jQuery hanzi2pinyin
fast [hanzi](http://en.wikipedia.org/wiki/Hanzi) to [pinyin](http://en.wikipedia.org/wiki/Pinyin) conversion

[Demo](http://www.caiguanhao.com/hanzi2pinyin/demo.html), where you can customize hanzi2pinyin

## Versions
### jquery-hanzi2pinyin.all.js (~102KB)
contains simplified and traditional Chinese characters and pinyins with [tones](http://en.wikipedia.org/wiki/Pinyin#Tones).

### jquery-hanzi2pinyin.simp.js (~24KB)
contains only simplified Chinese characters and pinyins without tones (suitable for users in mainland China).

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

### target
selectors which will contain the results

### hyphen
the hyphens between pinyins

### 'case'
can be ***lower***, ***upper*** or ***proper*** (***title***) case

*(Note: adding quotes around case is necessary for IE browsers)*

### punctuation_marks
you can ***remove***, ***ignore*** the Chinese punctuation marks or ***replace*** them with corresponding English punctuation marks ([?](http://en.wikipedia.org/wiki/Chinese_punctuation))

### fullwidth_chars
you can ***remove***, ***ignore*** the fullwidth characters or ***replace*** them with corresponding halfwidth characters ([?](http://en.wikipedia.org/wiki/Halfwidth_and_fullwidth_forms))

### tones
displays tones in ***simple*** (han-zi), ***standard*** (hàn-zì) or ***numeric*** (han4-zi4) mode