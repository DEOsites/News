<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AIニュース</title>

<style>
:root {
  --bg: #f4f6f8;
  --card: #ffffff;
  --text: #111;
  --sub: #666;
  --accent: #2563eb;
}

@media (prefers-color-scheme: dark) {
  :root {
    --bg: #0f172a;
    --card: #1e293b;
    --text: #e5e7eb;
    --sub: #9ca3af;
  }
}

body {
  margin: 0;
  font-family: system-ui, -apple-system, BlinkMacSystemFont;
  background: var(--bg);
  color: var(--text);
}

header {
  padding: 16px;
  background: var(--card);
  box-shadow: 0 2px 6px rgba(0,0,0,.08);
  position: sticky;
  top: 0;
}

header h1 {
  margin: 0;
  font-size: 20px;
}

.container {
  padding: 16px;
  max-width: 700px;
  margin: auto;
}

.news-card {
  background: var(--card);
  border-radius: 16px;
  padding: 16px;
  margin-bottom: 16px;
  box-shadow: 0 6px 16px rgba(0,0,0,.08);
}

.news-card h2 {
  font-size: 17px;
  margin: 0 0 8px;
}

.tag {
  display: inline-block;
  font-size: 11px;
  padding: 4px 8px;
  border-radius: 999px;
  background: var(--accent);
  color: white;
  margin-bottom: 8px;
}

.summary {
  font-size: 14px;
  line-height: 1.6;
  color: var(--text);
}

.meta {
  font-size: 12px;
  color: var(--sub);
  margin-top: 10px;
}

a.source {
  display: inline-block;
  margin-top: 10px;
  font-size: 13px;
  color: var(--accent);
  text-decoration: none;
}

footer {
  text-align: center;
  font-size: 12px;
  color: var(--sub);
  padding: 24px 0;
}
</style>
</head>

<body>

<header>
  <h1>🧠 AIニュース</h1>
</header>

<div class="container">

  <div class="news-card">
    <div class="tag">国際</div>
    <h2>各国が米国との貿易戦略を再調整</h2>
    <p class="summary">
      米国の通商政策を背景に、各国が外交・貿易戦略の見直しを進めている。
      特にアジア・欧州諸国では経済的自立を強める動きが注目されている。
    </p>
    <a class="source" href="#" target="_blank">元記事を見る</a>
    <div class="meta">AI要約・自動生成</div>
  </div>

  <div class="news-card">
    <div class="tag">テクノロジー</div>
    <h2>大手クラウドサービスで一時障害</h2>
    <p class="summary">
      世界的なクラウドサービスで短時間の障害が発生し、
      多数のウェブサービスに影響が出た。
      企業側は再発防止策を公表している。
    </p>
    <a class="source" href="#" target="_blank">元記事を見る</a>
    <div class="meta">AI要約・自動生成</div>
  </div>

</div>

<footer>
  本サイトはAIが公開情報を要約しています
</footer>

</body>
</html>