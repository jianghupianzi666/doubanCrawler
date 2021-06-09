# doubanCrawler
1. 这个repo就是把这个repo的代码https://github.com/Captain-F/DoubanHahahaScraper clone下来，然后把不能compile的code fix了，让他可以compile. (感谢大神分享代码，我只是代码的搬运工，不妥联系我我马上删)
2. patches did:
	1) 加了code去install没有install的lib
	2) In doubanScraper.ipynb, 变量count一开始没有定义，导致code不能编译, fix加了count的定义
	3) 少了一个import tqdm的statement, 加上了
	4) 原代码assume发帖日期格式是xxxx-xx-xx, 但是实际上日期格式有两种 a) 06-09 10:31, b) 2018-04-02, 当日期格式是a)的时候，代码不能编译。把这个修复了。
	5) 多加了几个stopwords的来源，原包里的stopwords只有英文，“的”，“你”这种词都没有过滤掉
	6) 增加了一个图: 回复的词云
