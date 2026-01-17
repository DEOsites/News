<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title></title>
<style>
body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, "Hiragino Kaku Gothic ProN", "Noto Sans JP", sans-serif;
  background: #f5f5f5;
  color: #111;
}
a { text-decoration: none; color: inherit; }
.container { max-width: 600px; margin: auto; }

/* 一覧 */
.news-list { background: #fff; }
.news-item {
  display: flex;
  gap: 12px;
  padding: 12px;
  border-bottom: 1px solid #e5e5e5;
}
.news-item:last-child { border-bottom: none; }
.thumb {
  width: 96px; height: 72px;
  background: #ddd;
  border-radius: 4px;
  flex-shrink: 0;
}
.content {}
.title { font-size: 16px; font-weight: 600; margin-bottom: 4px; }
.meta { font-size: 12px; color: #777; }

/* 詳細 */
.detail-page { padding: 16px; background: #fff; display: none; }
.detail-title { font-size: 20px; font-weight: bold; margin-bottom: 12px; }
.detail-body { font-size: 15px; line-height: 1.6; margin-bottom: 16px; }
.back-btn {
  font-size: 14px;
  color: #2563eb;
  margin-bottom: 12px;
  display: inline-block;
}
</style>
</head>
<body>

<div class="container">

  <!-- ニュース一覧 -->
  <div id="list" class="news-list">

    <a class="news-item" href="#"
       onclick="showDetail('d1')">
      <div class="thumb"></div>
      <div class="content">
        <div class="title">日伊首脳 経済安全保障協力を強化一致</div>
        <div class="meta">国際ニュース</div>
      </div>
    </a>

    <a class="news-item" href="#"
       onclick="showDetail('d2')">
      <div class="thumb"></div>
      <div class="content">
        <div class="title">トランプ政権1年目 半数が「失敗」評価</div>
        <div class="meta">国際政治</div>
      </div>
    </a>

    <a class="news-item" href="#"
       onclick="showDetail('d3')">
      <div class="thumb"></div>
      <div class="content">
        <div class="title">米市場：テック株が反発し株価安定</div>
        <div class="meta">経済ニュース</div>
      </div>
    </a>

    <a class="news-item" href="#"
       onclick="showDetail('d4')">
      <div class="thumb"></div>
      <div class="content">
        <div class="title">不動産市場の選別、次の段階へ</div>
        <div class="meta">社会ニュース</div>
      </div>
    </a>

  </div>

  <!-- 詳細ページテンプレ -->
  <div id="d1" class="detail-page">
    <a class="back-btn" href="#" onclick="backToList()">← 一覧に戻る</a>
    <div class="detail-title">日伊首脳 経済安全保障協力を強化一致</div>
    <div class="detail-body">
      高市総理はイタリアのメローニ首相と会談し、
      サプライチェーンや宇宙分野での協力強化に合意した。  
      これは経済安全保障の枠組みを拡大する重要な一歩となる。  
      出典: NHKニュース おはよう日本（TVでた蔵） 0
    </div>
  </div>

  <div id="d2" class="detail-page">
    <a class="back-btn" href="#" onclick="backToList()">← 一覧に戻る</a>
    <div class="detail-title">トランプ政権1年目 半数が「失敗」評価</div>
    <div class="detail-body">
      トランプ大統領の1年目を評価するCNNの調査では、
      半数以上が経済政策に否定的な見方をしている。  
      とくに物価高対策について「不十分」と答えた割合が高い。  
      出典: テレビ朝日ニュース 1
    </div>
  </div>

  <div id="d3" class="detail-page">
    <a class="back-btn" href="#" onclick="backToList()">← 一覧に戻る</a>
    <div class="detail-title">米市場：テック株が反発し株価安定</div>
    <div class="detail-body">
      米国株式市場では大型テクノロジー株が反発し、
      S&P500指数が安定した動きを見せた。  
      一方、原油価格が大きく下落したことも市場心理に影響している。  
      出典: Times of India（AP通信） 2
    </div>
  </div>

  <div id="d4" class="detail-page">
    <a class="back-btn" href="#" onclick="backToList()">← 一覧に戻る</a>
    <div class="detail-title">不動産市場の選別、次の段階へ</div>
    <div class="detail-body">
      不動産価格や取引の「選別」が進み、
      市場は新たなフェーズに入っているとの分析が出ている。  
      出典: ライブドアニュース 3
    </div>
  </div>

</div>


<script>
// 詳細表示
function showDetail(id) {
  document.getElementById("list").style.display = "none";
  document.getElementById(id).style.display = "block";
}
// 一覧に戻る
function backToList() {
  document.getElementById("list").style.display = "block";
  document.querySelectorAll('.detail-page').forEach(div =>{
    div.style.display = "none";
  });
}
</script>

</body>
</html>
