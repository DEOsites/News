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

/* ニュース一覧 */
.news-list {
  max-width: 600px;
  margin: auto;
  background: #fff;
}

/* 1記事 */
.news-item {
  display: flex;
  gap: 12px;
  padding: 14px;
  border-bottom: 1px solid #e5e5e5;
}

.news-item:last-child {
  border-bottom: none;
}

/* サムネ */
.thumb {
  width: 96px;
  height: 72px;
  background: #ddd;
  border-radius: 4px;
  flex-shrink: 0;
}

/* テキスト */
.content {
  flex: 1;
}

.title {
  font-size: 16px;
  font-weight: 600;
  line-height: 1.4;
  margin-bottom: 6px;
}

.meta {
  font-size: 12px;
  color: #777;
}

.tag {
  color: #2563eb;
  margin-right: 6px;
}
</style>
</head>

<body>

<div class="news-list">

  <div class="news-item">
    <div class="thumb"></div>
    <div class="content">
      <div class="title">
        各国が米国の通商政策を受け戦略見直しへ
      </div>
      <div class="meta">
        <span class="tag">国際</span>
        AI要約・1時間前
      </div>
    </div>
  </div>

  <div class="news-item">
    <div class="thumb"></div>
    <div class="content">
      <div class="title">
        大手クラウドサービスで一時的な障害発生
      </div>
      <div class="meta">
        <span class="tag">IT</span>
        AI要約・3時間前
      </div>
    </div>
  </div>

  <div class="news-item">
    <div class="thumb"></div>
    <div class="content">
      <div class="title">
        観光業界で国内旅行需要が回復傾向に
      </div>
      <div class="meta">
        <span class="tag">経済</span>
        AI要約・昨日
      </div>
    </div>
  </div>

</div>

</body>
</html>
