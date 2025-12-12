# mygooglesite
<html>
<head>
<meta charset="UTF-8">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial;
}

/* Tabs */
.tabs {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 10px;
  border-bottom: 2px solid #ccc;
}

.tab {
  padding: 10px 16px;
  cursor: pointer;
  background: #eee;
  margin-right: 5px;
  border-radius: 6px 6px 0 0;
}

input { display:none; }

.content {
  padding: 15px;
  border: 1px solid #ccc;
}

#A:checked ~ .content .A,
#B:checked ~ .content .B {
  display: block;
}

.A, .B {
  display: none;
}
</style>
</head>
<body>

<label class="tab" for="A">A</label>
<label class="tab" for="B">B</label>

<input type="radio" id="A" name="x" checked>
<input type="radio" id="B" name="x">

<div class="content">
  <div class="A"><h3>A內容</h3><p>內容很多也沒關係。</p></div>
  <div class="B"><h3>B內容</h3><p>內容自然往下，不會有捲動。</p></div>
</div>

</body>
</html>
