---
layout: default
title: Home
---

# Sun & Moon Web Pages

## 시간 정보

<div id="seoul"></div>
<div id="newyork"></div>

<script>
function updateTime() {
  document.getElementById('seoul').textContent =
    'Seoul: ' + new Date().toLocaleString('ko-KR', {
      timeZone: 'Asia/Seoul'
    });

  document.getElementById('newyork').textContent =
    'New York: ' + new Date().toLocaleString('en-US', {
      timeZone: 'America/New_York'
    });
}

updateTime();
setInterval(updateTime, 1000);
</script>
