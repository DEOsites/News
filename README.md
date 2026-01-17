<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title></title>

<style>
/* スマホ専用・横スクロール完全封鎖 */
html, body {
  margin: 0;
  padding: 0;
  width: 100%;
  overflow-x: hidden;
  background: #ffffff;
  font-family: -apple-system, BlinkMacSystemFont,
    "Hiragino Kaku Gothic ProN", "Noto Sans JP", sans-serif;
  color: #111;
}

* {
  box-sizing: border-box;
}

.wrapper {
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}

/* 一覧 */
.item {
  padding: 14px;
  border-bottom: 1px solid #e5e5e5;
}

.item:last-child {
  border-bottom: none;
}

.item-title {
  font-size: 16px;
  font-weight: 600;
  line-height: 1.5;
}

.item-cat {
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
  display: inline-block;
  margin-bottom: 14px;
  font-size: 14px;
  color: #2563eb;
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

<div class="wrapper">

<!-- 一覧 -->
<div id="list">

  <div class="item" onclick="openDetail('n1')">
    <div class="item-title">日米首脳会談 半導体供給網で連携強化</div>
    <div class="item-cat">国際</div>
  </div>

  <div class="item" onclick="openDetail('n2')">
    <div class="item-title">FRB 利下げ時期を巡り市場見方割れる</div>
    <div class="item-cat">経済</div>
  </div>

  <div class="item" onclick="openDetail('n3')">
    <div class="item-title">円相場 一時1ドル＝150円台</div>
    <div class="item-cat">経済</div>
  </div>

  <div class="item" onclick="openDetail('n4')">
    <div class="item-title">生成AI導入 企業で明暗分かれる</div>
    <div class="item-cat">IT</div>
  </div>

  <div class="item" onclick="openDetail('n5')">
    <div class="item-title">能登半島地震 復旧・復興が本格化</div>
    <div class="item-cat">国内</div>
  </div>

  <div class="item" onclick="openDetail('n6')">
    <div class="item-title">ウクライナ情勢 停戦見通し立たず</div>
    <div class="item-cat">国際</div>
  </div>

  <div class="item" onclick="openDetail('n7')">
    <div class="item-title">国内観光需要 回復基調続く</div>
    <div class="item-cat">社会</div>
  </div>

  <div class="item" onclick="openDetail('n8')">
    <div class="item-title">大手IT企業 決算発表で株価変動</div>
    <div class="item-cat">経済</div>
  </div>

</div>

<!-- 詳細 -->
<div id="n1" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">日米首脳会談 半導体供給網で連携強化</div>
  <div class="detail-body">
    日米両政府は首脳会談を行い、半導体や重要物資の供給網について
    協力を強化する方針を確認した。
  </div>
</div>

<div id="n2" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">FRB 利下げ時期を巡り市場見方割れる</div>
  <div class="detail-body">
    インフレ動向を受け、利下げ時期について市場関係者の見方が分かれている。
  </div>
</div>

<div id="n3" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">円相場 一時1ドル＝150円台</div>
  <div class="detail-body">
    為替市場では円安が進行し、家計や企業への影響が注目されている。
  </div>
</div>

<div id="n4" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">生成AI導入 企業で明暗分かれる</div>
  <div class="detail-body">
    業務効率化を進める企業がある一方、リスク管理を重視する動きもある。
  </div>
</div>

<div id="n5" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">能登半島地震 復旧・復興が本格化</div>
  <div class="detail-body">
    被災地ではインフラ復旧や生活再建に向けた取り組みが進んでいる。
  </div>
</div>

<div id="n6" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">ウクライナ情勢 停戦見通し立たず</div>
  <div class="detail-body">
    戦闘の長期化により国際社会では懸念が強まっている。
  </div>
</div>

<div id="n7" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">国内観光需要 回復基調続く</div>
  <div class="detail-body">
    地方を中心に観光客が戻り、宿泊施設の稼働率が改善している。
  </div>
</div>

<div id="n8" class="detail">
  <span class="back" onclick="back()">← 戻る</span>
  <div class="detail-title">大手IT企業 決算発表で株価変動</div>
  <div class="detail-body">
    決算内容を受け、株式市場では関連銘柄が上下した。
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
