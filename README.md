## 自我介紹

我叫彭顯皓，目前正在學習怎麼當一個苦命的資工人，平常的休閒就是玩遊戲跟看youtube。

### 我看youtube最愛看的人:國動
<img src="https://i.imgur.com/D3zmG9m.jpg">

我的偶像，臺灣桃園人，是網路遊戲實況主，為蹦蛙數位娛樂旗下藝人，綽號「國動」，源自於他喜歡看的政論節目《大話新聞》中的常態來賓吳國棟。除此之外，也有「瘋狗動」、「海鮮稽查員」、「改革家」、「鼻地大師」等稱呼。他是另一位實況主「亞洲統神」張嘉航的哥哥。
<br>
他有許多影片在嘴砲他人跟過激反應，但個人認為他的影片相當好笑，推薦大家去看看

### 我看youtube最愛看的團體:反正我很閒
<body>
	<div class="slideshow">
		<ul>
			<li>
				<a href="#">
					<img src="https://i.imgur.com/l0J8D4L.png" title="" alt="" />
				</a>
			</li>
			<li>
				<a href="#">
					<img src="https://i.imgur.com/RE5xc6A.jpg" title="" alt="" />
				</a>
			</li>
			<li>
				<a href="#">
					<img src="https://i.imgur.com/S5F3ADb.jpg" title="" alt="" />
				</a>
			</li>
			<li>
				<a href="#">
					<img src="https://i.imgur.com/kFoFCNP.jpg" title="" alt="" />
				</a>
			</li>
		</ul>
	</div>
</body>

ul, li {
	margin: 0;
	padding: 0;
	list-style: none;
}
.slideshow {
	position: relative;
	height: 160px;
	width: 210px;
	float: left;
	margin: 0 10px;
	border: 3px solid #ddd;
}
.slideshow li {
	position: absolute;
}
.slideshow a img{
	display: block;
	padding: 0;
	margin: 0 auto;
	border: none;
}
.slideshow li a{
	display: block;
}
.slideshowController {
	position: absolute;
	right: 0;
	bottom: 0;
}
.slideshowController a {
	background: transparent url(images/arrows.png) no-repeat left top;
	display: block;
	width: 30px;
	height: 30px;
	position: absolute;
	right: 60px;
	bottom: 0;
	z-index: 9999;
	outline: none;
}
.slideshowController .next{
	background-position: -30px 0;
	right: 0;
}
.slideshowController .play{
	background-position: -60px 0;
	right: 30px;
}
.slideshowController .pause{
	background-position: -90px 0;
}

$(function(){

	var _fadeSpeed = 600;

	$('.slideshow').each(function(){

		var $this = $(this), 
			$ul = $this.find('ul'), 
			$li = $ul.find('li'), 
			$controller = $('<div class="slideshowController"><a href="#"></a><a href="#" class="play"></a><a href="#" class="next"></a></div>').css('opacity', 0), 
			_len = $li.length, 
			_index = 0, timer, _speed = 2000;

		$li.eq(_index).css('z-index', 2).siblings().css('opacity', 0);

		$this.append($controller).hover(function(){
			$controller.stop().animate({
				opacity: 1
			});
		}, function(){
			$controller.stop().animate({
				opacity: 0
			});
		});

		$controller.delegate('a', 'click', function(){

			var $a = $(this), 
				_className = $a.attr('class');

			if(('play pause').indexOf(_className) > -1){

				$a.toggleClass('pause').hasClass('pause') ? timer = setTimeout(autoClickNext, _fadeSpeed + _speed) : clearTimeout(timer);
				return false;
			}
 

			clearTimeout(timer);

			$a.siblings('.pause').removeClass('pause');

			_index = ('next' == _className ? _index + 1 : _index - 1 + _len) % _len;

			show();
 
			return false;
		});

		function autoClickNext() {
			_index = (_index + 1) % _len;
			show();
			timer = setTimeout(autoClickNext, _fadeSpeed + _speed);
		}
 
		function show() {
			$li.eq(_index).animate({
				opacity: 1, 
				zIndex: 2
			}, _fadeSpeed).siblings(':visible').animate({
				opacity: 0, 
				zIndex: 1
			}, _fadeSpeed);
		}
	});
});

反正我很閒是一個YouTube頻道，團隊由鍾佳播、陳奕凱及趙福臨組成。內容以喜劇的方式討論各種主題，含括了社會政治、哲學思考、男女情感、都市傳說等，其中以諷刺資本主義和反抗體制的左膠為最主要特色。鏡頭則是以嘲弄YouTuber慣用的跳接剪輯，刻意粗糙的影像，以及縮放鏡頭的手法呈現。劇中創造了許多如「卑鄙源之助」、「惡魔貓男」、「台北暴徒」等虛構人物和洗腦台詞在網路上蔚為流行，可謂迷因製造機。

### Game

### Apex
<img src="https://i.imgur.com/W2yqfPi.jpg">

遊戲以3人小隊為單位進行遊戲，每局遊戲最多有60人。每位玩家可以從十三位傳奇角色中選擇一位進行遊戲，每位英雄都有其獨特的技能，玩家可以自訂其外觀。隊伍空投落地後需要尋找武器、彈藥及其他裝備，小隊間互相戰鬥至最後存活一隊為勝。遊戲特有復活系統，如有隊友死亡，玩家可以在時限內(90s)取得陣亡隊友的旗幟，並將其攜至重生點即可復活隊友。同時，遊戲也設有較為詳細的標記功能，也可進行隊伍語音。

### LOL

