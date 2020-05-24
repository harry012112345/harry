## 自我介紹

我叫彭顯皓，目前正在學習怎麼當一個苦命的資工人，平常的休閒就是玩遊戲跟看youtube。

### 我看youtube最愛看的人:國動
<img src="https://i.imgur.com/D3zmG9m.jpg">

我的偶像，臺灣桃園人，是網路遊戲實況主，為蹦蛙數位娛樂旗下藝人，綽號「國動」，源自於他喜歡看的政論節目《大話新聞》中的常態來賓吳國棟。除此之外，也有「瘋狗動」、「海鮮稽查員」、「改革家」、「鼻地大師」等稱呼。他是另一位實況主「亞洲統神」張嘉航的哥哥。
<br>
他有許多影片在嘴砲他人跟過激反應，但個人認為他的影片相當好笑，推薦大家去看看

### 我看youtube最愛看的團體:反正我很閒

<body>
	<div class="abgne-block-20110423">
		<ul>
			<li><a href="#"><img src="images/1s.jpg" /></a></li>
			<li><a href="#"><img src="images/2s.jpg" /></a></li>
			<li><a href="#"><img src="images/3s.jpg" /></a></li>
			<li><a href="#"><img src="images/4s.jpg" /></a></li>
		</ul>
	</div>
</body>
ul, li {
	margin: 0;
	padding: 0;
	list-style: none;
}
a img {
	border: none;
}
.abgne-block-20110423 {
	overflow: hidden;
	margin: 10px;
	width: 100px;	/* 圖片的寬 */
	height: 100px;	/* 圖片的高 */
	border: 1px solid #525252;
	border-radius: 10px;
}
.abgne-block-20110423 ul {
	position: relative;
}
.abgne-block-20110423 ul li {
	position: absolute;
}
 
.abgne-block-20110423 ul li a {
	display: block;
	width: 100px;	/* 圖片的寬 */
}
.abgne-block-20110423 ul li a img {
	border-radius: 10px;
}	
$(function(){
	// 取得全部要處理的區塊元素
	$('.abgne-block-20110423').each(function(){
		// 取得必要的元素並用 jQuery 包裝
		// 再來取得 $li 的寬度及設定動畫時間
		var $block = $(this),  
			$ul = $block.find('ul'),
			$li = $ul.find('li'), 
			_left = $block.offset().left,
			_width = $li.find('a').width(), 
			_ratio = Math.ceil(_width / $li.length);
 
		// 除了第一張圖之外, 其它的都先隱藏
		$li.eq(0).siblings().hide();
 
		// 當滑鼠在 $block 上移動時
		$block.mousemove(function(e){
 
			// 計算要顯示那一張圖片
			var index = Math.floor((e.pageX - _left)/_ratio);
 
			$li.eq(index).show().siblings().hide();
		})
	}).find('a').focus(function(){
		this.blur();
	});
});	
	
反正我很閒是一個YouTube頻道，團隊由鍾佳播、陳奕凱及趙福臨組成。內容以喜劇的方式討論各種主題，含括了社會政治、哲學思考、男女情感、都市傳說等，其中以諷刺資本主義和反抗體制的左膠為最主要特色。鏡頭則是以嘲弄YouTuber慣用的跳接剪輯，刻意粗糙的影像，以及縮放鏡頭的手法呈現。劇中創造了許多如「卑鄙源之助」、「惡魔貓男」、「台北暴徒」等虛構人物和洗腦台詞在網路上蔚為流行，可謂迷因製造機。

### Game

### Apex
<img src="https://i.imgur.com/W2yqfPi.jpg">

遊戲以3人小隊為單位進行遊戲，每局遊戲最多有60人。每位玩家可以從十三位傳奇角色中選擇一位進行遊戲，每位英雄都有其獨特的技能，玩家可以自訂其外觀。隊伍空投落地後需要尋找武器、彈藥及其他裝備，小隊間互相戰鬥至最後存活一隊為勝。遊戲特有復活系統，如有隊友死亡，玩家可以在時限內(90s)取得陣亡隊友的旗幟，並將其攜至重生點即可復活隊友。同時，遊戲也設有較為詳細的標記功能，也可進行隊伍語音。

### LOL

