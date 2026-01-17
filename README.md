<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title></title>

<style>
body {
  margin: 0;
  background: #f5f5f5;
  font-family: -apple-system, BlinkMacSystemFont, "Hiragino Kaku Gothic ProN", "Noto Sans JP", sans-serif;
  color: #111;
}

a {
  text-decoration: none;
  color: inherit;
}

.container {
  max-width: 600px;
  margin: 0 auto;
  background: #fff;
}

/* 一覧 */
.news-item {
  padding: 14px;
  border-bottom: 1px solid #e5e5e5;
}

.news-item:last-child {
  border-bottom: none;
}

.title {
  font-size: 16px;
  font-weight: 600;
  line-height: 1.45;
}

.meta {
  margin-top: 6px;
  font-size: 12px;
  color: #777;
}

/* 詳細 */
.detail {
  display: none;
  padding: 16px;
}

.back {
  font-size: 14px;
  color: #2563eb;
  margin-bottom: 12px;
  display: inline-block;
}

.detail-title {
  font-size: 20px;
  font-weight: 700;
  margin-bottom: 14px;
}

.detail-body {
  font-size: 15px;
  line-height: 1.7;
}
</style>
</head>

<body>

<div class="container">

  <!-- 一覧 -->
  <div id="list">

    <div class="news-item" onclick="openDetail('n1')">
      <div class="title">日米首脳会談 経済安全保障で連携強化へ</div>
      <div class="meta">国際</div>
    </div>

    <div class="news-item" onclick="openDetail('n2')">
      <div class="title">米FRB 利下げ時期を慎重に判断との見方</div>
      <div class="meta">経済</div>
    </div>

    <div class="news-item" onclick="openDetail('n3')">
      <div class="title">生成AIの利用拡大 企業の対応分かれる</div>
      <div class="meta">IT</div>
    </div>

    <div class="news-item" onclick="openDetail('n4')">
      <div class="title">国内観光需要 回復基調が続く</div>
      <div class="meta">社会</div>
    </div>

    <div class="news-item" onclick="openDetail('n5')">
      <div class="title">中東情勢 緊張長期化への懸念強まる</div>
      <div class="meta">国際</div>
    </div>

  </div>

  <!-- 詳細 -->
  <div id="n1" class="detail">
    <span class="back" onclick="back()">← 戻る</span>
    <div class="detail-title">日米首脳会談 経済安全保障で連携強化へ</div>
    <div class="detail-body">
      日米両首脳は会談を行い、半導体や重要資源の供給網を中心に
      経済安全保障分野での協力を一段と強化する方針を確認した。
      今後は民間企業との連携も含めた枠組みづくりが進められる見通し。
    </div>
  </div>

  <div id="n2" class="detail">
    <span class="back" onclick="back()">← 戻る</span>
    <div class="detail-title">米FRB 利下げ時期を慎重に判断との見方</div>
    <div class="detail-body">
      米国の金融政策を巡り、FRBはインフレ動向を見極めながら
      利下げのタイミングを慎重に判断するとの見方が広がっている。
      市場では早期利下げへの期待と警戒感が交錯している。
    </div>
  </div>

  <div id="n3" class="detail">
    <span class="back" onclick="back()">← 戻る</span>
    <div class="detail-title">生成AIの利用拡大 企業の対応分かれる</div>
    <div class="detail-body">
      生成AIの活用が急速に進む中、業務効率化を進める企業がある一方で、
      情報管理や著作権への懸念から導入に慎重な姿勢を示す企業もある。
    </div>
  </div>

  <div id="n4" class="detail">
    <span class="back" onclick="back()">← 戻る</span>
    <div class="detail-title">国内観光需要 回復基調が続く</div>
    <div class="detail-body">
      国内旅行の需要は引き続き回復傾向にあり、
      地方都市でも宿泊予約が増加している。
      観光業界では人手不足への対応が課題となっている。
    </div>
  </div>

  <div id="n5" class="detail">
    <span class="back" onclick="back()">← 戻る</span>
    <div class="detail-title">中東情勢 緊張長期化への懸念強まる</div>
    <div class="detail-body">
      中東地域では緊張状態が続いており、
      国際社会では事態の長期化を懸念する声が強まっている。
      各国は外交的解決を模索している。
    </div>
  </div>

</div>

<script>
function openDetail(id) {
  document.getElementById("list").style.display = "none";
  document.querySelectorAll(".detail").forEach(d => d.style.display = "none");
  document.getElementById(id).style.display = "block";
}

function back() {
  document.getElementById("list").style.display = "block";
  document.querySelectorAll(".detail").forEach(d => d.style.display = "none");
}
</script>

</body>
</html>
