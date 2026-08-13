<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GTQ 자기소개서 초안 도구 | 그린컴퓨터아카데미</title>
<style>
  :root{
    --deep-green:#1B5E42;
    --mint-bg:#E8F5E9;
    --mint-line:#81C784;
    --amber:#F4A020;
    --paper:#F4F6F4;
    --ink:#1F2A24;
    --ink-soft:#5B6B62;
    --before:#C0392B;
    --before-bg:#FDEDEC;
    --before-line:#F1B3AC;
    --after:#1B5E42;
    --after-bg:#E8F5E9;
    --after-line:#81C784;
    --white:#FFFFFF;
    --radius:14px;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    background:var(--paper);
    color:var(--ink);
    font-family:'Pretendard','Apple SD Gothic Neo','Malgun Gothic',sans-serif;
    line-height:1.55;
  }
  .topbar{
    background:var(--deep-green);
    color:#fff;
    padding:28px 24px;
  }
  .topbar-inner{
    max-width:960px;
    margin:0 auto;
  }
  .eyebrow{
    font-size:13px;
    letter-spacing:.08em;
    color:#B2DFCA;
    font-weight:700;
    text-transform:uppercase;
  }
  h1{
    margin:6px 0 4px;
    font-size:26px;
    font-weight:800;
  }
  .sub{
    font-style:italic;
    color:#CDE9DA;
    font-size:14px;
    margin:0;
  }
  main{
    max-width:960px;
    margin:0 auto;
    padding:28px 24px 80px;
  }
  .panel{
    background:var(--white);
    border-radius:var(--radius);
    border:1px solid #E1E7E3;
    padding:24px;
    margin-bottom:20px;
    box-shadow:0 1px 3px rgba(27,94,66,.05);
  }
  .panel h2{
    font-size:16px;
    margin:0 0 4px;
    color:var(--deep-green);
    display:flex;
    align-items:center;
    gap:8px;
  }
  .panel h2 .num{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    width:22px;height:22px;
    border-radius:50%;
    background:var(--deep-green);
    color:#fff;
    font-size:12px;
    font-weight:700;
  }
  .panel .hint{
    font-size:13px;
    color:var(--ink-soft);
    margin:0 0 16px;
  }
  label{
    display:block;
    font-size:13px;
    font-weight:700;
    color:var(--ink);
    margin-bottom:6px;
  }
  .field{margin-bottom:16px;}
  .field:last-child{margin-bottom:0;}
  input[type=text], textarea, select{
    width:100%;
    padding:10px 12px;
    border-radius:8px;
    border:1px solid #D7DED9;
    font-size:14px;
    font-family:inherit;
    background:#FBFCFB;
    color:var(--ink);
  }
  input[type=text]:focus, textarea:focus, select:focus{
    outline:2px solid var(--mint-line);
    outline-offset:1px;
    background:#fff;
  }
  textarea{resize:vertical; min-height:64px;}
  .grid2{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:16px;
  }
  @media (max-width:640px){ .grid2{grid-template-columns:1fr;} }
  .toolrow{display:flex; gap:10px; flex-wrap:wrap;}
  .chip{
    padding:8px 14px;
    border-radius:999px;
    border:1px solid #D7DED9;
    background:#FBFCFB;
    font-size:13px;
    cursor:pointer;
    user-select:none;
  }
  .chip.active{
    background:var(--mint-bg);
    border-color:var(--mint-line);
    color:var(--deep-green);
    font-weight:700;
  }
  .generate-bar{
    position:sticky;
    bottom:0;
    background:linear-gradient(180deg, rgba(244,246,244,0) 0%, var(--paper) 30%);
    padding:16px 0 4px;
    text-align:center;
  }
  button.generate{
    background:var(--deep-green);
    color:#fff;
    border:none;
    padding:14px 32px;
    font-size:15px;
    font-weight:700;
    border-radius:999px;
    cursor:pointer;
    box-shadow:0 4px 14px rgba(27,94,66,.28);
  }
  button.generate:hover{background:#164A35;}
  .result-section{display:none;}
  .result-section.show{display:block;}
  .warn-box{
    background:#FFF8E1;
    border:1px solid #F4D98A;
    border-radius:10px;
    padding:14px 16px;
    font-size:13px;
    font-weight:700;
    color:#5B4A16;
    margin-bottom:20px;
    text-align:center;
  }
  .draft-card{
    background:var(--white);
    border-radius:var(--radius);
    border:1px solid #E1E7E3;
    margin-bottom:16px;
    overflow:hidden;
  }
  .draft-head{
    background:var(--mint-bg);
    border-bottom:1px solid var(--mint-line);
    padding:12px 18px;
    display:flex;
    align-items:center;
    justify-content:space-between;
  }
  .draft-head h3{
    margin:0;
    font-size:15px;
    color:var(--deep-green);
  }
  .copy-btn{
    background:#fff;
    border:1px solid var(--mint-line);
    color:var(--deep-green);
    font-size:12px;
    font-weight:700;
    padding:6px 12px;
    border-radius:999px;
    cursor:pointer;
  }
  .copy-btn:hover{background:var(--mint-bg);}
  .draft-body{
    padding:18px;
    font-size:14.5px;
    white-space:pre-wrap;
  }
  .principles{
    background:var(--after-bg);
    border:1px solid var(--after-line);
    border-radius:var(--radius);
    padding:20px 22px;
    margin-bottom:20px;
  }
  .principles h3{
    margin:0 0 10px;
    color:var(--deep-green);
    font-size:15px;
  }
  .principles ol{
    margin:0;
    padding-left:20px;
    font-size:13.5px;
    color:var(--ink);
  }
  .principles li{margin-bottom:6px;}
  .principles .example{
    color:var(--ink-soft);
    font-style:italic;
    font-size:12.5px;
  }
  footer{
    text-align:center;
    color:var(--ink-soft);
    font-size:12px;
    padding:20px 0 0;
  }
  .empty-state{
    text-align:center;
    color:var(--ink-soft);
    font-size:13px;
    padding:30px 0;
  }
</style>
</head>
<body>

<div class="topbar">
  <div class="topbar-inner">
    <div class="eyebrow">그린컴퓨터아카데미 강남캠퍼스 · 취업지원실</div>
    <h1>GTQ 자기소개서 초안 도구</h1>
    <p class="sub">Photoshop·Illustrator 실습 경험을 자기소개서 초안으로 — 초안 확인 후 반드시 내 말투로 수정하세요</p>
  </div>
</div>

<main>

  <div class="panel">
    <h2><span class="num">1</span> 기본 정보</h2>
    <p class="hint">지원하는 회사와 직무를 입력하세요. 초안 곳곳에 자동으로 반영됩니다.</p>
    <div class="grid2">
      <div class="field">
        <label for="company">지원 회사명</label>
        <input type="text" id="company" placeholder="예: OO디자인스튜디오">
      </div>
      <div class="field">
        <label for="job">지원 직무</label>
        <input type="text" id="job" placeholder="예: 콘텐츠 디자이너">
      </div>
    </div>
  </div>

  <div class="panel">
    <h2><span class="num">2</span> 관심의 시작 — 계기 에피소드</h2>
    <p class="hint">디자인·이미지 편집에 관심을 갖게 된 구체적인 경험을 짧게 적어주세요. (아르바이트, 동아리, SNS 운영 등)</p>
    <div class="field">
      <textarea id="motiveStory" placeholder="예: 카페 아르바이트 당시 SNS 홍보 게시물을 제작하는 업무를 맡으며, 이미지 한 장이 매장 방문에 영향을 준다는 것을 느꼈다"></textarea>
    </div>
  </div>

  <div class="panel">
    <h2><span class="num">3</span> GTQ 과정에서 쌓은 역량</h2>
    <p class="hint">사용한 도구와 결과물, 가능하면 수치를 함께 적어주세요.</p>
    <div class="toolrow" id="toolChips" style="margin-bottom:16px;">
      <span class="chip active" data-tool="Photoshop">Photoshop</span>
      <span class="chip active" data-tool="Illustrator">Illustrator</span>
      <span class="chip" data-tool="InDesign">InDesign</span>
      <span class="chip" data-tool="프리미어프로">프리미어 프로</span>
    </div>
    <div class="field">
      <label for="output">대표 결과물 (구체적으로)</label>
      <input type="text" id="output" placeholder="예: 카드뉴스 6종, 상세페이지 3종, 포스터 2종">
    </div>
    <div class="field">
      <label for="skillDetail">실습 과정에서 익힌 것</label>
      <textarea id="skillDetail" placeholder="예: 정보 위계와 톤앤매너를 통일하는 실습을 반복하며 실무 활용 능력을 갖춤"></textarea>
    </div>
  </div>

  <div class="panel">
    <h2><span class="num">4</span> 성격 장점 · 단점</h2>
    <div class="grid2">
      <div class="field">
        <label for="strength">장점 키워드</label>
        <select id="strength">
          <option value="꼼꼼함">꼼꼼함</option>
          <option value="성실함">성실함</option>
          <option value="주도성">주도성</option>
          <option value="협업 능력">협업 능력</option>
          <option value="트렌드 감각">트렌드 감각</option>
        </select>
      </div>
      <div class="field">
        <label for="weakness">보완 중인 점</label>
        <select id="weakness">
          <option value="완벽을 추구하다 보니 작업 속도가 다소 느려지는 것">완벽 추구 → 속도 저하</option>
          <option value="새로운 툴 적응에 시간이 걸리는 것">새 툴 적응 시간</option>
          <option value="혼자 판단하고 진행하려는 경향">혼자 판단하려는 경향</option>
        </select>
      </div>
    </div>
    <div class="field">
      <label for="strengthStory">장점을 보여주는 에피소드</label>
      <textarea id="strengthStory" placeholder="예: 카드뉴스 제작 과정에서 정보 위계와 색상 규칙이 맞는지 다시 확인하며 오류를 줄이려 노력함"></textarea>
    </div>
  </div>

  <div class="panel">
    <h2><span class="num">5</span> 입사 후 포부</h2>
    <div class="field">
      <label for="goal">단기 목표 (입사 초기)</label>
      <input type="text" id="goal" placeholder="예: 사내 디자인 가이드와 작업 흐름 빠르게 파악">
    </div>
  </div>

  <div class="generate-bar">
    <button class="generate" onclick="generateDraft()">자기소개서 초안 생성하기</button>
  </div>

  <div class="result-section" id="resultSection">

    <div class="warn-box">⚠️ 주의! AI는 초안 생성기입니다 — 없는 경험 지어내기 절대 금지 · 반드시 내 말투로 수정 · 복붙 제출 금지!</div>

    <div class="draft-card">
      <div class="draft-head"><h3>① 지원동기</h3><button class="copy-btn" onclick="copyText('draft1')">복사</button></div>
      <div class="draft-body" id="draft1"></div>
    </div>

    <div class="draft-card">
      <div class="draft-head"><h3>② 성격의 장점 및 단점</h3><button class="copy-btn" onclick="copyText('draft2')">복사</button></div>
      <div class="draft-body" id="draft2"></div>
    </div>

    <div class="draft-card">
      <div class="draft-head"><h3>③ 직무경험 및 역량</h3><button class="copy-btn" onclick="copyText('draft3')">복사</button></div>
      <div class="draft-body" id="draft3"></div>
    </div>

    <div class="draft-card">
      <div class="draft-head"><h3>④ 입사 후 포부</h3><button class="copy-btn" onclick="copyText('draft4')">복사</button></div>
      <div class="draft-body" id="draft4"></div>
    </div>

    <div class="principles">
      <h3>초안 확인 후 — 이렇게 수정하세요</h3>
      <ol>
        <li><b>내 경험이 맞는지 확인</b> — 없는 내용은 삭제하세요</li>
        <li><b>AI 말투 → 내 말투로 바꾸기</b></li>
        <li><b>수치·도구명 구체적으로 추가</b>
          <div class="example">예) "이미지를 편집했습니다" → "Photoshop으로 카드뉴스 6종 제작"</div>
        </li>
        <li><b>지원 회사명·직무명 맞게 수정</b></li>
        <li><b>한 번만 쓰고 복붙 금지! 회사마다 다르게</b></li>
      </ol>
    </div>

  </div>

  <div class="empty-state" id="emptyState">
    ↑ 항목을 입력하고 "자기소개서 초안 생성하기"를 눌러주세요
  </div>

</main>

<footer>취업지원실 신수지 · 010-7547-9780 · green_job@nate.com</footer>

<script>
document.querySelectorAll('#toolChips .chip').forEach(chip=>{
  chip.addEventListener('click', ()=> chip.classList.toggle('active'));
});

function val(id, fallback){
  const v = document.getElementById(id).value.trim();
  return v || fallback;
}

function selectedTools(){
  const chips = [...document.querySelectorAll('#toolChips .chip.active')].map(c=>c.dataset.tool);
  return chips.length ? chips.join('·') : 'Photoshop·Illustrator';
}

function generateDraft(){
  const company = val('company', '귀사');
  const job = val('job', '콘텐츠 디자인');
  const motiveStory = val('motiveStory', '카페 아르바이트 당시 SNS 홍보 게시물을 제작하는 업무를 맡으며, 이미지 한 장이 매장 방문에 직접적인 영향을 준다는 것을 경험했습니다');
  const tools = selectedTools();
  const output = val('output', '카드뉴스 6종');
  const skillDetail = val('skillDetail', '정보 위계와 톤앤매너를 통일하는 실습을 반복하며 실무 활용 능력을 갖추었습니다');
  const strength = val('strength', '꼼꼼함');
  const weakness = val('weakness', '완벽을 추구하다 보니 작업 속도가 다소 느려지는 것');
  const strengthStory = val('strengthStory', '카드뉴스 제작 과정에서 정보 위계와 색상 규칙이 맞는지 다시 확인하며 오류를 줄이고자 노력했습니다');
  const goal = val('goal', '사내 디자인 가이드와 작업 흐름을 빠르게 파악하는 것');

  const draft1 =
`[관심의 시작]
${motiveStory}. 이를 통해 ${job} 업무에 흥미를 가지게 되었습니다.

[현재 노력]
GTQ 취득 과정에서 ${tools}를 활용해 ${output}을 제작하고, ${skillDetail}

[미래 기여]
입사 후에는 디자인 툴을 활용해 ${company}의 콘텐츠를 효율적으로 제작하고, 통일된 톤앤매너로 콘텐츠의 신뢰도를 높이는 데 기여하겠습니다.`;

  const draft2 =
`[장점: 직무와 연결된 강점]
저의 가장 큰 장점은 결과물의 완성도를 끝까지 확인하는 ${strength}입니다.
${strengthStory} 그 결과 제작 과정에서 발생하는 실수를 줄이고, 보다 안정적으로 작업을 수행할 수 있었습니다.
이러한 습관은 GTQ 과정에서도 이어져, 실습 파일 제출 전 레이어와 색상값을 다시 검토하는 것을 기본 원칙으로 삼고 있습니다.

[단점 및 보완 노력]
반면, ${weakness}이 있었습니다.
이를 보완하기 위해 작업 전 우선순위를 정리하고, 시간 기준을 설정하여 일정 내에 시안을 마무리하는 연습을 하고 있습니다.`;

  const draft3 =
`[직무경험 및 역량]
GTQ 과정에서 ${output} 제작을 담당하며 콘텐츠 결과물의 완성도를 개선한 경험이 있습니다.

[문제인식]
작업 진행 과정에서 시안마다 폰트와 색상 규칙이 통일되지 않아 확인과 수정에 시간이 반복적으로 소요되는 문제를 발견했습니다.

[해결 행동]
이에 자주 사용하는 요소를 기준으로 디자인 가이드를 정리하고, ${tools}를 활용해 폰트·색상을 통일하여 시안 제작과 검토 과정을 개선했습니다.

[성과]
그 결과 시안 제작 시 불필요한 수정 과정을 줄이고, ${output}을 통일된 톤앤매너로 완성할 수 있었습니다.`;

  const draft4 =
`[단기 목표: 업무 적응]
입사 초기에는 ${goal}, ${tools}를 활용한 콘텐츠 제작 업무를 정확하게 수행하겠습니다.

[중기 목표: 업무 효율 개선]
반복되는 작업을 보다 효율적으로 처리할 수 있는 방법을 고민하며, 디자인 툴과 사내 시스템 활용 능력을 함께 향상시키겠습니다.

[장기 목표: 신뢰 기반 업무 수행]
정확성과 감각을 바탕으로 맡은 작업을 안정적으로 수행하며, ${company}에서 신뢰받는 ${job}(으)로 성장하겠습니다.`;

  document.getElementById('draft1').textContent = draft1;
  document.getElementById('draft2').textContent = draft2;
  document.getElementById('draft3').textContent = draft3;
  document.getElementById('draft4').textContent = draft4;

  document.getElementById('resultSection').classList.add('show');
  document.getElementById('emptyState').style.display = 'none';
  document.getElementById('resultSection').scrollIntoView({behavior:'smooth', block:'start'});
}

function copyText(id){
  const text = document.getElementById(id).textContent;
  navigator.clipboard.writeText(text).then(()=>{
    event.target.textContent = '복사됨!';
    setTimeout(()=>{ event.target.textContent = '복사'; }, 1500);
  });
}
</script>

</body>
</html>
