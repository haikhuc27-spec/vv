<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>VYVY HAIRCARE 2025</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:Arial;background:#0f172a;color:#e2e8f0;padding:20px}
h1{text-align:center;color:#38bdf8;font-size:22px;padding-bottom:4px}
.sub{text-align:center;color:#64748b;font-size:11px;margin-bottom:20px}
.kpi{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:20px}
.k{background:#1e293b;border-radius:10px;padding:14px;text-align:center;border:1px solid #334155}
.v{font-size:17px;font-weight:bold;word-break:break-all}
.l{font-size:10px;color:#94a3b8;margin-top:4px}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.box{background:#1e293b;border-radius:10px;padding:16px;border:1px solid #334155}
.full{grid-column:1/-1}
.ct{font-size:10px;font-weight:bold;color:#38bdf8;text-transform:uppercase;letter-spacing:1px;margin-bottom:3px}
.cd{font-size:9px;color:#64748b;font-style:italic;margin-bottom:10px}
.ins{font-size:10px;padding:7px 10px;border-radius:4px;margin-top:8px;line-height:1.5}
.b{background:#0f2744;border-left:3px solid #38bdf8}
.r{background:#2d1515;border-left:3px solid #ef4444}
.g{background:#0f2d1a;border-left:3px solid #4ade80}
.y{background:#2d2000;border-left:3px solid #fbbf24}
table{width:100%;border-collapse:collapse;font-size:11px;margin-top:8px}
th{background:#334155;color:#94a3b8;padding:7px 8px;text-align:right;font-weight:normal;font-size:10px}
th:first-child{text-align:left}
td{padding:6px 8px;border-bottom:1px solid #1e293b;text-align:right}
td:first-child{text-align:left;color:#38bdf8;font-weight:bold}
.up{color:#4ade80}
.dn{color:#ef4444}
.nt{color:#fbbf24}
.row-low{background:#2d1515}
.row-high{background:#0f2d1a}
.row-sum{background:#1e3a5f;font-weight:bold}
</style>
</head>
<body>

<h1>DASHBOARD DOANH SO 2025 — VYVY HAIRCARE</h1>
<p class="sub">Tong 22,422,074,189 VND | Shopee + TikTok + Facebook | 01/01/2025 - 31/12/2025</p>

<div class="kpi">
  <div class="k"><div class="v" style="color:#38bdf8">22.42 ty</div><div class="l">Tong doanh so 2025</div></div>
  <div class="k"><div class="v" style="color:#4ade80">3.87 ty</div><div class="l">Dinh nam T12/2025</div></div>
  <div class="k"><div class="v" style="color:#f87171">944.9 tr</div><div class="l">Day nam T9/2025</div></div>
  <div class="k"><div class="v" style="color:#fbbf24">4.45 ty</div><div class="l">Du bao ATH T1/2026</div></div>
  <div class="k"><div class="v" style="color:#10b981">8.91 ty</div><div class="l">Facebook 39.7%</div></div>
  <div class="k"><div class="v" style="color:#3b82f6">8.41 ty</div><div class="l">Shopee 37.5%</div></div>
  <div class="k"><div class="v" style="color:#8b5cf6">5.07 ty</div><div class="l">TikTok 22.6%</div></div>
  <div class="k"><div class="v" style="color:#fbbf24">1.87 ty</div><div class="l">Trung binh thang</div></div>
</div>

<div class="grid">

  <div class="box full">
    <div class="ct">1. DOANH SO TONG THEO THANG (Line Chart)</div>
    <div class="cd">Line Chart: xu huong theo thoi gian. 3 giai doan: Tang T1-T5 → Day T6-T9 → Bung no T10-T12</div>
    <canvas id="c1" height="55"></canvas>
    <div class="ins b">T1-T5: +46.9% | T6-T9: -49.4%, day T9 = 944.9M | T10-T12: +310%, dinh T12 = 3.87 ty</div>
  </div>

  <div class="box">
    <div class="ct">2. CO CAU THEO KENH (Doughnut)</div>
    <div class="cd">Ty trong 3 kenh. Facebook dan dau nhung TikTok tang nhanh nhat.</div>
    <canvas id="c2"></canvas>
    <div class="ins r">RUI RO: Facebook + Shopee chiem 77.2% — phu thuoc 2 kenh chinh</div>
  </div>

  <div class="box">
    <div class="ct">3. SO SANH 3 KENH THEO THANG (Grouped Bar)</div>
    <div class="cd">Dong gop tung kenh moi thang. TikTok bung no T10-T12.</div>
    <canvas id="c3" height="90"></canvas>
    <div class="ins g">TikTok: 94.9M (T9) → 1,582.5M (T12) = +1,568% trong 3 thang</div>
  </div>

  <div class="box full">
    <div class="ct">4. TANG TRUONG % THEO THANG — MA MAU (Color Bar)</div>
    <div class="cd">Xanh = tang manh, Vang = on dinh, Do = giam. 1 bieu do noi 2 thong tin.</div>
    <canvas id="c4" height="50"></canvas>
    <div class="ins r">T9: -43.5% — Day nam soc nhat. Can phan tich nguyen nhan phong tranh T9/2026.</div>
    <div class="ins g">T10: +141.7% Breakout | T12: +47.0% Dinh nam. TikTok la dong luc chinh.</div>
  </div>

  <div class="box full">
    <div class="ct">5. AREA CHART — DONG GOP TUNG KENH</div>
    <div class="cd">Area Chart: the hien dong gop tich luy. TikTok dao nguoc ngoan muc cuoi nam.</div>
    <canvas id="c5" height="55"></canvas>
    <div class="ins b">Facebook on dinh lon nhat. Shopee on dinh tang cham. TikTok thap dau nam bung no cuoi nam.</div>
  </div>

  <div class="box">
    <div class="ct">6. DU BAO T1-T2/2026 (Bar)</div>
    <div class="cd">ATH T1/2026 = 4.45 ty. Dieu chinh T2/2026 do chu ky + Tet.</div>
    <canvas id="c6"></canvas>
    <div class="ins g">T1/2026: 4,451,284,937 VND — Ky luc moi. TikTok lan dau dan dau 1.88 ty.</div>
    <div class="ins y">T2/2026: 1,141,024,067 VND — Giam 74.4% chu ky binh thuong.</div>
  </div>

  <div class="box">
    <div class="ct">7. TONG DOANH SO CA NAM TUNG KENH (Bar)</div>
    <div class="cd">So sanh tong dong gop ca nam 2025 tung kenh.</div>
    <canvas id="c7"></canvas>
    <div class="ins b">Facebook vuot Shopee 498.6 trieu. TikTok con cach xa nhung tang nhanh nhat.</div>
  </div>

  <div class="box full">
    <div class="ct">8. BANG DU LIEU GOC — 12 THANG 2025</div>
    <div class="cd">Du lieu goc chinh xac 100% tu JSON. Don vi: VND.</div>
    <table>
      <tr>
        <th>Thang</th>
        <th>Shopee</th>
        <th>TikTok</th>
        <th>TikTok Cha</th>
        <th>Facebook</th>
        <th>Tong thang</th>
        <th>%</th>
        <th>Nhan xet</th>
      </tr>
      <tr><td>T01</td><td>617,118,053</td><td>212,601,772</td><td>1,130,000</td><td>466,637,550</td><td>1,297,487,375</td><td class="nt">+6%</td><td>Moc co so</td></tr>
      <tr><td>T02</td><td>579,267,851</td><td>304,421,834</td><td>6,716,000</td><td>336,129,500</td><td>1,226,535,185</td><td class="dn">-5.5%</td><td>Giam nhe Tet</td></tr>
      <tr><td>T03</td><td>729,190,908</td><td>361,098,331</td><td>7,303,000</td><td>460,993,850</td><td>1,558,586,089</td><td class="up">+27.1%</td><td>Phuc hoi manh</td></tr>
      <tr><td>T04</td><td>642,543,517</td><td>354,079,326</td><td>3,452,000</td><td>744,968,650</td><td>1,745,043,493</td><td class="up">+12.0%</td><td>Duy tri tang</td></tr>
      <tr><td>T05</td><td>661,237,692</td><td>335,554,688</td><td>1,801,000</td><td>907,734,200</td><td>1,906,327,580</td><td class="up">+9.2%</td><td>Tiep tuc tang</td></tr>
      <tr><td>T06</td><td>739,407,379</td><td>290,659,162</td><td>2,206,000</td><td>834,616,251</td><td>1,866,888,792</td><td class="dn">-2.1%</td><td>Di ngang</td></tr>
      <tr><td>T07</td><td>666,691,072</td><td>244,015,830</td><td>2,638,000</td><td>828,988,900</td><td>1,742,333,802</td><td class="dn">-6.7%</td><td>Dieu chinh</td></tr>
      <tr><td>T08</td><td>682,952,815</td><td>209,087,386</td><td>0</td><td>780,133,900</td><td>1,672,174,101</td><td class="dn">-4.0%</td><td>On dinh</td></tr>
      <tr class="row-low"><td>T09</td><td>486,581,486</td><td>94,869,041</td><td>0</td><td>363,451,300</td><td>944,901,827</td><td class="dn">-43.5%</td><td>DAY NAM</td></tr>
      <tr><td>T10</td><td>656,386,606</td><td>460,225,682</td><td>0</td><td>1,167,117,000</td><td>2,283,729,288</td><td class="up">+141.7%</td><td>Breakout</td></tr>
      <tr><td>T11</td><td>760,198,175</td><td>658,317,863</td><td>0</td><td>1,218,764,500</td><td>2,637,280,538</td><td class="up">+15.5%</td><td>Hung phan</td></tr>
      <tr class="row-high"><td>T12</td><td>1,190,568,288</td><td>1,582,533,596</td><td>0</td><td>1,101,474,100</td><td>3,874,575,984</td><td class="up">+47.0%</td><td>DINH NAM</td></tr>
      <tr class="row-sum"><td>TONG</td><td>8,412,353,977</td><td>5,073,464,511</td><td>25,246,000</td><td>8,911,009,701</td><td>22,422,074,189</td><td>—</td><td>22.42 ty VND</td></tr>
    </table>
  </div>

</div>

<p style="text-align:center;color:#334155;font-size:10px;margin-top:20px">VYVY HAIRCARE — Dashboard 2025 | Powered by Zapier AI | 07/06/2026</p>

<script>
Chart.defaults.color = '#94a3b8';
Chart.defaults.borderColor = '#334155';

var M = ['T1','T2','T3','T4','T5','T6','T7','T8','T9','T10','T11','T12'];

var SP = [617118053,579267851,729190908,642543517,661237692,739407379,666691072,682952815,486581486,656386606,760198175,1190568288];
var TK = [212601772,304421834,361098331,354079326,335554688,290659162,244015830,209087386,94869041,460225682,658317863,1582533596];
var FB = [466637550,336129500,460993850,744968650,907734200,834616251,828988900,780133900,363451300,1167117000,1218764500,1101474100];
var TOT = [1297487375,1226535185,1558586089,1745043493,1906327580,1866888792,1742333802,1672174101,944901827,2283729288,2637280538,3874575984];

function m(a){ return a.map(function(v){ return Math.round(v/1000000); }); }

// C1 Line
new Chart(document.getElementById('c1'),{
  type:'line',
  data:{
    labels:M,
    datasets:[
      {label:'Tong',data:m(TOT),borderColor:'#38bdf8',backgroundColor:'rgba(56,189,248,0.07)',fill:true,tension:0.4,pointRadius:m(TOT).map(function(v,i){return i===8||i===11?6:3;}),pointBackgroundColor:m(TOT).map(function(v,i){return i===8?'#ef4444':i===11?'#4ade80':'#38bdf8';}),borderWidth:2},
      {label:'Shopee',data:m(SP),borderColor:'#3b82f6',tension:0.4,pointRadius:2,borderWidth:1.5,borderDash:[4,2]},
      {label:'TikTok',data:m(TK),borderColor:'#8b5cf6',tension:0.4,pointRadius:2,borderWidth:1.5,borderDash:[4,2]},
      {label:'Facebook',data:m(FB),borderColor:'#10b981',tension:0.4,pointRadius:2,borderWidth:1.5,borderDash:[4,2]}
    ]
  },
  options:{responsive:true,plugins:{legend:{position:'top',labels:{font:{size:9}}}},scales:{y:{ticks:{callback:function(v){return v+'M';}}}}}
});

// C2 Doughnut
new Chart(document.getElementById('c2'),{
  type:'doughnut',
  data:{
    labels:['Facebook 39.7%','Shopee 37.5%','TikTok 22.6%','TikTok Cha 0.1%'],
    datasets:[{data:[8911009701,8412353977,5073464511,25246000],backgroundColor:['#10b981','#3b82f6','#8b5cf6','#6366f1'],borderWidth:2,borderColor:'#0f172a'}]
  },
  options:{responsive:true,plugins:{legend:{position:'bottom',labels:{font:{size:10}}}}}
});

// C3 Grouped Bar
new Chart(document.getElementById('c3'),{
  type:'bar',
  data:{
    labels:M,
    datasets:[
      {label:'Shopee',data:m(SP),backgroundColor:'#3b82f6',borderRadius:3},
      {label:'TikTok',data:m(TK),backgroundColor:'#8b5cf6',borderRadius:3},
      {label:'Facebook',data:m(FB),backgroundColor:'#10b981',borderRadius:3}
    ]
  },
  options:{responsive:true,plugins:{legend:{position:'top',labels:{font:{size:9}}}},scales:{y:{ticks:{callback:function(v){return v+'M';}}}}}
});

// C4 Color Bar tang truong
var GR = [6,-5.5,27.1,12.0,9.2,-2.1,-6.7,-4.0,-43.5,141.7,15.5,47.0];
new Chart(document.getElementById('c4'),{
  type:'bar',
  data:{
    labels:M,
    datasets:[{
      data:GR,
      backgroundColor:GR.map(function(v){return v>=20?'#4ade80':v>=0?'#fbbf24':'#ef4444';}),
      borderRadius:4
    }]
  },
  options:{responsive:true,plugins:{legend:{display:false}},scales:{y:{ticks:{callback:function(v){return v+'%';}}}}}
});

// C5 Area
new Chart(document.getElementById('c5'),{
  type:'line',
  data:{
    labels:M,
    datasets:[
      {label:'Facebook',data:m(FB),borderColor:'#10b981',backgroundColor:'rgba(16,185,129,0.15)',fill:true,tension:0.4,pointRadius:2},
      {label:'Shopee',data:m(SP),borderColor:'#3b82f6',backgroundColor:'rgba(59,130,246,0.15)',fill:true,tension:0.4,pointRadius:2},
      {label:'TikTok',data:m(TK),borderColor:'#8b5cf6',backgroundColor:'rgba(139,92,246,0.15)',fill:true,tension:0.4,pointRadius:2}
    ]
  },
  options:{responsive:true,plugins:{legend:{position:'top',labels:{font:{size:9}}}},scales:{y:{ticks:{callback:function(v){return v+'M';}}}}}
});

// C6 Du bao
new Chart(document.getElementById('c6'),{
  type:'bar',
  data:{
    labels:['T10/25','T11/25','T12/25','T1/26','T2/26'],
    datasets:[
      {label:'Thuc te 2025',data:[2283.7,2637.3,3874.6,null,null],backgroundColor:'#3b82f6',borderRadius:4},
      {label:'Du bao 2026',data:[null,null,null,4451.3,1141.0],backgroundColor:'#f59e0b',borderRadius:4}
    ]
  },
  options:{responsive:true,plugins:{legend:{position:'top',labels:{font:{size:9}}}},scales:{y:{ticks:{callback:function(v){return v+'M';}}}}}
});

// C7 Tong kenh
new Chart(document.getElementById('c7'),{
  type:'bar',
  data:{
    labels:['Facebook','Shopee','TikTok','TikTok Cha'],
    datasets:[{
      data:[8.91,8.41,5.07,0.025],
      backgroundColor:['#10b981','#3b82f6','#8b5cf6','#6366f1'],
      borderRadius:6
    }]
  },
  options:{responsive:true,plugins:{legend:{display:false}},scales:{y:{ticks:{callback:function(v){return v+' ty';}}}}}
});
</script>
</body>
</html>
