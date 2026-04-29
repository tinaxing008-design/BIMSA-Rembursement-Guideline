<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>BIMSA Reimbursement | Travel & Labor Service Fee</title>
  <!-- Google Fonts for clean typography -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;400;500;600;700&display=swap" rel="stylesheet">
  <!-- Font Awesome 6 -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', sans-serif;
      background: #f4f7fc;
      color: #1a2c3e;
      line-height: 1.5;
    }
    .app {
      max-width: 1400px;
      margin: 0 auto;
      padding: 2rem 1.5rem 3rem;
    }
    /* Cover section */
    .cover {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 85vh;
      text-align: center;
    }
    .logo-area {
      margin-bottom: 2rem;
    }
    .logo-area h2 {
      font-weight: 500;
      font-size: 1.5rem;
      letter-spacing: -0.3px;
      color: #2c6e9e;
      border-bottom: 2px solid #cbdde9;
      display: inline-block;
      padding-bottom: 0.25rem;
    }
    .cover h1 {
      font-size: 3.2rem;
      font-weight: 600;
      margin-bottom: 0.75rem;
      color: #0a2942;
      letter-spacing: -0.02em;
    }
    .subhead {
      font-size: 1.2rem;
      color: #4a627a;
      margin-bottom: 3rem;
      max-width: 550px;
    }
    .card-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
      margin-top: 1rem;
    }
    .reim-card {
      background: white;
      border-radius: 2rem;
      padding: 2.5rem 3rem;
      width: 280px;
      cursor: pointer;
      transition: all 0.25s ease;
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.05), 0 0 0 1px rgba(0, 0, 0, 0.02);
      text-align: center;
    }
    .reim-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 25px 40px rgba(0, 0, 0, 0.1);
    }
    .card-icon {
      font-size: 3rem;
      color: #2c6e9e;
      margin-bottom: 1.2rem;
    }
    .reim-card h3 {
      font-size: 2rem;
      font-weight: 600;
      margin-bottom: 0.5rem;
      color: #1a2c3e;
    }
    .reim-card p {
      color: #5e7e9c;
      font-size: 0.95rem;
    }
    /* Detail pages */
    .detail-page {
      display: none;
      animation: fadeIn 0.3s ease;
    }
    .detail-page.active-page {
      display: block;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(8px);}
      to { opacity: 1; transform: translateY(0);}
    }
    .back-btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: white;
      border: none;
      padding: 0.6rem 1.2rem;
      font-size: 0.9rem;
      font-weight: 500;
      border-radius: 40px;
      cursor: pointer;
      margin-bottom: 1.8rem;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
      transition: 0.2s;
      font-family: inherit;
      color: #2c6e9e;
    }
    .back-btn:hover {
      background: #e9f0f5;
      transform: translateX(-3px);
    }
    .page-header {
      margin-bottom: 2rem;
      border-left: 5px solid #2c6e9e;
      padding-left: 1.2rem;
    }
    .page-header h1 {
      font-size: 2.2rem;
      font-weight: 600;
      color: #0f3b5c;
    }
    .page-header p {
      color: #5a6e82;
      margin-top: 0.3rem;
    }
    /* travel sub-nav */
    .travel-subnav, .labor-subnav {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-bottom: 2rem;
      border-bottom: 1px solid #d4e2ec;
      padding-bottom: 0.5rem;
    }
    .travel-subnav button, .labor-subnav button {
      background: none;
      border: none;
      font-size: 1rem;
      font-weight: 600;
      padding: 0.5rem 1.2rem;
      border-radius: 30px;
      cursor: pointer;
      transition: 0.2s;
      font-family: inherit;
      color: #5a6e82;
    }
    .travel-subnav button.active-tab, .labor-subnav button.active-tab {
      background: #2c6e9e;
      color: white;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    .travel-subnav button:not(.active-tab):hover, .labor-subnav button:not(.active-tab):hover {
      background: #e9f0f5;
      color: #1f496e;
    }
    .travel-tab-content, .labor-tab-content {
      display: none;
    }
    .travel-tab-content.active-tab-content, .labor-tab-content.active-tab-content {
      display: block;
      animation: fadeIn 0.2s ease;
    }
    .doc-section {
      background: white;
      border-radius: 1.5rem;
      padding: 1.8rem 2rem;
      margin-bottom: 2rem;
      box-shadow: 0 5px 18px rgba(0, 0, 0, 0.03), 0 0 0 1px #e2edf2;
    }
    .doc-section h2 {
      font-size: 1.5rem;
      font-weight: 600;
      margin-bottom: 1rem;
      display: flex;
      align-items: center;
      gap: 0.6rem;
      color: #1f496e;
    }
    .doc-section h2 i {
      font-size: 1.4rem;
      color: #3b82b6;
    }
    .doc-list {
      list-style: none;
      padding-left: 0.2rem;
    }
    .doc-list li {
      margin-bottom: 0.75rem;
      padding-left: 1.5rem;
      position: relative;
      font-size: 0.98rem;
      color: #2d3e53;
    }
    .doc-list li:before {
      content: "📄";
      position: absolute;
      left: -0.2rem;
      top: 0;
      font-size: 0.85rem;
      opacity: 0.8;
    }
    .vertical-transport-list {
      list-style: none;
      margin-top: 0.5rem;
    }
    .vertical-transport-list li {
      margin-bottom: 1rem;
      padding-left: 1.6rem;
      position: relative;
    }
    .vertical-transport-list li strong {
      color: #1f6e9c;
      display: inline-block;
      min-width: 100px;
    }
    .vertical-transport-list li:before {
      content: "✈️";
      position: absolute;
      left: 0;
      top: 0;
      font-size: 0.9rem;
    }
    .vertical-transport-list li.train-item:before {
      content: "🚆";
    }
    .vertical-transport-list li.car-item:before {
      content: "🚗";
    }
    .sub-note {
      background-color: #f0f6fa;
      border-left: 3px solid #6c9ebf;
      padding: 0.8rem 1.2rem;
      margin-top: 1rem;
      border-radius: 12px;
      font-size: 0.85rem;
      color: #2c5a7a;
    }
    .standard-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      margin-top: 1rem;
    }
    .std-card {
      background: #f9fdfe;
      border-radius: 1rem;
      padding: 1rem 1.2rem;
      flex: 1 1 200px;
      border: 1px solid #dce7ef;
    }
    .std-card strong {
      color: #1f6e9c;
      display: block;
      margin-bottom: 0.3rem;
    }
     /* Per diem counting table */
    .perdiem-table {
      width: 100%;
      border-collapse: collapse;
      margin: 1rem 0 0.5rem;
      background: #fefefe;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 1px 2px rgba(0,0,0,0.03);
    }
    .perdiem-table th, .perdiem-table td {
      border: 1px solid #dce5ec;
      padding: 0.9rem 1rem;
      text-align: left;
      vertical-align: top;
      font-size: 0.95rem;
    }
    .perdiem-table th {
      background-color: #e9f2f7;
      font-weight: 600;
      color: #1f496e;
    }
    .perdiem-table td {
      color: #2c3e50;
    }
    .perdiem-note {
      margin-top: 0.75rem;
      font-size: 0.85rem;
      color: #4f6f8f;
      background: #f9fcfd;
      padding: 0.5rem 1rem;
      border-radius: 12px;
    }
    hr {
      margin: 1rem 0;
      border: none;
      border-top: 1px solid #d4e2ec;
    }
    @media (max-width: 700px) {
      .app { padding: 1rem; }
      .reim-card { padding: 1.8rem 1.5rem; width: 240px; }
      .doc-section { padding: 1.2rem; }
      .cover h1 { font-size: 2.2rem; }
    }
  </style>
</head>
<body>
<div class="app" id="app">
  <!-- ==================== COVER SECTION ==================== -->
  <div id="coverSection" class="cover">
    <div class="logo-area"><h2>BIMSA</h2></div>
    <h1>Reimbursement Guidelines</h1>
    <div class="subhead">Select a category to view required documents & policies</div>
    <div class="card-grid">
      <div class="reim-card" data-page="travel">
        <div class="card-icon"><i class="fas fa-plane-departure"></i></div>
        <h3>Travel</h3>
        <p>Domestic & International · Transport · Accommodation · Per diem</p>
      </div>
      <div class="reim-card" data-page="labor">
        <div class="card-icon"><i class="fas fa-file-invoice-dollar"></i></div>
        <h3>Labor service fee</h3>
        <p>Honoraria, Stipend for visitors · Invoicing & standards</p>
      </div>
    </div>
    <div style="margin-top: 3rem; font-size: 0.75rem; color: #8aa0b5;">BIMSA Finance · Please review latest policies</div>
  </div>

  <!-- ==================== TRAVEL DETAIL PAGE ==================== -->
  <div id="travelPage" class="detail-page">
    <button class="back-btn" data-back="cover"><i class="fas fa-arrow-left"></i> Back to categories</button>
    <div class="page-header">
      <h1><i class="fas fa-globe-asia"></i> Travel reimbursement</h1>
      <p>Domestic & international travel · required documents & policies</p>
    </div>
    <!-- travel sub-nav: domestic / international / Trip.com invoice (separate link) -->
    <div class="travel-subnav">
      <button id="domesticTabBtn" class="active-tab">Domestic Travel</button>
      <button id="internationalTabBtn">🌍 International Travel</button>
      <button id="tripcomTabBtn">🧾 How to issue invoice from Trip.com</button>
    </div>
    <div id="domesticContent" class="travel-tab-content active-tab-content">
      <div class="doc-section">
       <h2>Domestic travel – Documents checklist</h2>
        <ul class="doc-list">
          <li>Leave Application form (<span style="color: crimson;">THE grant used for the reimbursement should be the same as mentioned in your leave application form)</span></li>
          <li>Invitation letter or conference notification (会议通知)</li>
          <li><strong>For invited visitors:</strong> If support provided, obtain VP's consent screenshot (required by finance)</li></ul>
        <h3>Flight:</h3>
          <ul class="doc-list">
          <li>Boarding passes (photo or original)</li>
          <li>Chinese VAT invoice (note in the remark: itinerary, passenger info)</li>
          <li>Online order page or booking confirmation email (showing price breakdown, passenger & itinerary)</li>
          <li>Payment proof (if>10k RMB)</li></ul>
          <h3>Train:</h3>
          <ul class="doc-list"><li>Online order page (if online booking)</li>
          <li>Train ticket invoice (only via official China Railway app 12306 or station ticketing counter) <a href="https://www.12306.cn/en/index.html" target="_blank" style="color:#2c6e9e;">12306 website</a> | <a href="http://www.china-railway.com.cn/english/businesses/passenger/202411/t20241115_139137.html" target="_blank" style="color:#2c6e9e;">Guide on invoice issurance from 12306 app</a></li>
          <h3>Car ride to/from airport:</h3>
          <ul class="doc-list">
          <li>Electronic itinerary</li>
          <li>Chinese VAT invoice</li></ul>
      </div>
      <div class="doc-section">
        <h2><i class="fas fa-chart-line"></i> Transport & accommodation (China)</h2>
        <div class="standard-grid">
          <div class="std-card"><strong>✈️ Transport Standard</strong> Professors are eligible for <span style="color: crimson;">Business class</span> Flight and <span style="color: crimson;">First-class</span> Train. <br> Please refer to  p.15 <a href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf"><i>Financial Handbook</i></a> for more information</div>
          <div class="std-card"><strong>🏨 Accommodation Standard</strong> Upper Limit for Hotel in Beijing/Shanghai: <br>1080 RMB per night for <span style="color: crimson;">Professors</span>  and 990 RMB per night for others. <br>Please refer to  p.15-25 <a href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf"><i>Financial Handbook</i></a> for more information.</div> Beijing: academic exchanges within Beijing → not business trip; regular hotel stays due to teaching (excl. Qiuzhen credit course) require VP approval in advance; one-night stay → prior approval required.</div>
        </div>
      <div class="doc-section">
        <h2>Per diem allowance (meals & local transport)</h2>
        <ul class="doc-list">
          <li><strong>Rate:</strong> Meal 100 RMB/day + Local transport 80 RMB/day.</li></ul>
           <h3 style="margin: 1rem 0 0.5rem 0; font-size: 1.15rem;">📅 Per diem counting rules</h3>
           <table class="perdiem-table">
            <thead>
            <tr><th>Trip duration (days)</th><th>Allowance calculation</th></tr>
            </thead>
            <tbody>
            <tr><td>≤ 10 days</td><td>Full allowance for all days (meal + local transport).</td></tr>
            <tr><td>10–15 days</td><td>10 days full allowance + extra days at half rate.</td></tr>
            <tr><td>≥ 15 days</td><td>10 days full + 5 days half allowance (remaining days no per diem).</td></tr>
            </tbody>
           </table>
           <li><strong>Prerequisite:</strong> "No meals or local transport provided by host". Invitation must explicitly state no support for meals/transport.</li>
        <div class="sub-note"><i class="fas fa-info-circle"></i> Per diem claimable only if traveler bears own meals & local transit.</div>
      </div></div>
    <div id="internationalContent" class="travel-tab-content">
      <div class="doc-section">
        <h2><i class="fas fa-passport"></i> International travel – documents checklist</h2>
        <ul class="doc-list">
          <li>Leave application form</li>
          <li>Invitation Email</li>
          <li>Photo of passport photopage (if not provided yet)</li>
          <li>Bank detail and expected currency (for visitors who has not provided it yet)</li>
          <h3>Flight:</h3>
          <ul class="doc-list"></ul> 
          <li>Boarding passes (photo/original)</li>
          <li>The electronic copy of flight invoice/receipt; if bought via Chinese websites (including Trip.com), Chinese VAT invoice (fapiao) is required as well</li> 
          <li>Online booking confirmation email showing price breakdown, passenger and itinerary information</li>
          <li>The electronic copy of payment proof i.e. bank statement or credit card statement record showing the purchase of the flight</li></ul>
          <h3>Hotel:</h3> 
          <ul class="doc-list">
          <li>The electronic copy of hotel invoice/receipt; if booked via Chinese websites (including Trip.com), Chinese VAT invoice (fapiao) is required as well</li>
          <li>The electronic copy of the stamped hotel folio showinng price breakdown, check-in/out dates, and guest information</li>
          <li> Online order or booking confirmation email if booked online</li></ul>
          <h3>Car ride to/from airport:</h3> 
          <ul class="doc-list">
          <li>itinerary</li> 
          <li>Chinese VAT invoice</li></ul>
          <div>Invited visitors support:</strong> VP’s consent screenshot required in advance.</div>  
      </div>
      <div class="doc-section">
        <h2><i class="fas fa-plane"></i> Transport and Accommodation (international)</h2>
        <div class="standard-grid">
          <div class="std-card"><strong>Transport Standard</strong>Professors are eligible for <span style="color: crimson;">Business Class</span> Flight. <br>Please refer to p.27 <a href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf"><i>Financial Handbook（First Edition）</i></a> for more information.</div>
          <div class="std-card"><strong>Accommodation Standard</strong> Please refer to p.29-30 <a href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf"><i>Financial Handbook（First Edition）</i></a> for more information.</div>
        </div>
      </div>
      <div class="doc-section">
        <h2><i class="fas fa-hotel"></i>Per diem allowance (meals and local transport)</h2>
        <ul class="doc-list">
          <li>For BIMSA people, per diem is calculated based on the days on your leave application form</li>
          <li>For visitors, BIMSA does not provide per diem</li>
          <li>The per diem standard for international trips varies according to the destination.<br> Please refer to p.29-30 <a href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf"><i>Financial Handbook（First Edition</i>）</a> for the information.</li>
        </ul>
        <h3 style="margin: 1rem 0 0.5rem 0; font-size: 1.15rem;">📅 Per diem counting rules</h3>
        <table class="perdiem-table">
          <thead>
            <tr><th>Trip duration (days)</th><th>Allowance calculation</th></tr>
          </thead>
          <tbody>
            <tr><td>≤ 10 days</td><td>Full allowance for all days (meal + local transport)</td></tr>
            <tr><td>10-15 days</td><td>10 days full allowance + extra days at half rate</td></tr>
            <tr><td>≥ 15 days</td><td>10 days full + 5 days half allowance (remaining days no per diem)</td></tr>
          </tbody></table> 
      </div>
    </div>
    <div id="tripcomContent" class="travel-tab-content">
      <div class="doc-section">
        <h2><i class="fab fa-tripadvisor"></i> How to issue Chinese VAT invoice from Trip.com</h2>
        <ul class="doc-list" style="margin-bottom: 1rem;">
          <li>Step 1 → Go to <strong>My bookings</strong></li>
          <li>Step 2 → Choose your hotel or flight booking</li>
          <li>Step 3 → Go to <strong>Service Chat</strong> and select <strong>Chinese VAT invoice</strong></li>
          <li>Step 4 → Provide the tax number and the Chinese name of BIMSA in the chatbox:</li>
        </ul>
        <div style="background:#eef3f9; padding: 1rem; border-radius: 14px; margin: 0.5rem 0 1rem;">
          <strong>Chinese Name:</strong> 北京雁栖湖应用数学研究院<br/>
          <strong>Tax Number:</strong> 52110000MJ0166456X
        </div>
        <div class="sub-note"><i class="fas fa-receipt"></i> This VAT invoice process applies for both domestic & international bookings made via Trip.com. Ensure you request the invoice before closing the booking.</div>
      </div>
    </div>
  </div>
  <div id="laborPage" class="detail-page">
    <button class="back-btn" data-back="cover"><i class="fas fa-arrow-left"></i> Back to categories</button>
    <div class="page-header">
      <h1><i class="fas fa-hand-holding-usd"></i> Labor service fee & stipends</h1>
      <p>Honoraria, visitor stipends · required documents, standards & invoicing</p>
    </div>
    <div class="labor-subnav">
      <button id="honorariaTabBtn" class="active-tab">🏆 Honoraria for talks</button>
      <button id="stipendTabBtn">🎓 Stipend for visitors</button>
      <button id="notesTabBtn">📌 Notes</button>
    </div>
    <div id="honorariaContent" class="labor-tab-content active-tab-content">
      <div class="doc-section">
        <h2><i class="fas fa-chalkboard-teacher"></i> Honoraria for talks</h2>
        <ul class="doc-list">
          <li><strong>Standard:</strong><br/>
            - 2000 RMB per engagement for guests from <strong>outside Beijing</strong><br/>
            - 1000 RMB per engagement for guests <strong>from other institutes in Beijing</strong><br/>
            - 500 RMB per engagement for guests <strong>from Tsinghua University</strong>
          </li>
          <li><strong>Documents needed:</strong>
            <ul style="margin-top: 8px; margin-left: 1.5rem; list-style: circle;">
              <li>Printed webpage with talk description (date, time, abstract)</li>
              <li>Photocopy of recipient’s passport or Chinese ID card</li>
              <li>Bank details & phone number of recipient</li>
              <li><strong>Labor service fee invoice</strong> (required when amount ≥ 1,000 RMB)</li>
            </ul>
          </li>
          <li><strong>Important note:</strong> The payee must get the invoice on their own via the Tax Bureau App. For foreign nationals first signing up: need a <strong>registration code</strong> obtained from the Tax Hall in person (valid 7 days).</li>
        </ul>
        <div class="sub-note"><i class="fas fa-exclamation-triangle"></i> Invoice required for amounts ≥1000 RMB. Instruction on self-issuing labor service fee invoice available from finance (Word document).</div>
      </div>
    </div>
    <div id="stipendContent" class="labor-tab-content">
      <div class="doc-section">
        <h2><i class="fas fa-user-graduate"></i> Stipend for visitors (students)</h2>
        <ul class="doc-list">
          <li><strong>Standard:</strong> Up to <strong>9900 RMB per month</strong> for students.</li>
          <li><strong>Documents needed:</strong>
            <ul style="margin-top: 8px; margin-left: 1.5rem; list-style: circle;">
              <li>Short-term visitor application form + CV</li>
              <li>Photocopy of recipient’s passport or Chinese ID card</li>
              <li>Bank details & phone number of recipient</li>
              <li><strong>Labor service fee invoice</strong> (if amount ≥ 1,000 RMB)</li></ul>
        </ul>
      </div>
    </div>
    <div id="notesContent" class="labor-tab-content">
      <div class="doc-section">
        <h2><i class="fas fa-file-invoice"></i> Tax & invoicing guidance</h2>
        <p><strong>Chinese VAT invoice for labor service fee:</strong> Individuals must self-issue via official National Tax Bureau app. Foreign nationals: obtain 7-day registration code at local Tax Hall in person. BIMSA tax info for reference:</p>
        <div style="background:#eef3f9; padding: 0.8rem; border-radius: 14px; margin-top: 10px;">
          <strong>Chinese Name:</strong> 北京雁栖湖应用数学研究院 &nbsp;|&nbsp; <strong>Tax Number:</strong> 52110000MJ0166456X
        </div>
        <hr/>
        <p><i class="fas fa-clock"></i> <strong>Timing:</strong> For foreign nationals without Chinese tax app registration, please visit Tax Hall ahead of time for registration code.</p>
      </div>
      <div class="doc-section">
        <h2><i class="fas fa-clipboard-check"></i> Essential reminders</h2>
        <p>Always attach photocopy of ID/passport, bank details, and phone number. For honoraria, the printed webpage with date/time/abstract is mandatory. Invoices must be issued according to the threshold rules above.</p>
      </div>
    </div>
  </div>
</div>
<script>
  const coverDiv = document.getElementById('coverSection');
  const travelPage = document.getElementById('travelPage');
  const laborPage = document.getElementById('laborPage');
  function showCover() {
    coverDiv.style.display = 'flex';
    travelPage.classList.remove('active-page');
    laborPage.classList.remove('active-page');
    travelPage.style.display = 'none';
    laborPage.style.display = 'none';
    coverDiv.style.display = 'flex';
  }
  function showTravel() {
    coverDiv.style.display = 'none';
    travelPage.style.display = 'block';
    laborPage.style.display = 'none';
    travelPage.classList.add('active-page');
    laborPage.classList.remove('active-page');
    // default to domestic tab inside travel
    setActiveTravelTab('domestic');
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  function showLabor() {
    coverDiv.style.display = 'none';
    travelPage.style.display = 'none';
    laborPage.style.display = 'block';
    laborPage.classList.add('active-page');
    travelPage.classList.remove('active-page');
    setActiveLaborTab('honoraria');
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  
  // Travel tabs: domestic, international, tripcom
  const domesticTabBtn = document.getElementById('domesticTabBtn');
  const internationalTabBtn = document.getElementById('internationalTabBtn');
  const tripcomTabBtn = document.getElementById('tripcomTabBtn');
  const domesticContent = document.getElementById('domesticContent');
  const internationalContent = document.getElementById('internationalContent');
  const tripcomContent = document.getElementById('tripcomContent');

  function setActiveTravelTab(tab) {
    domesticContent.classList.remove('active-tab-content');
    internationalContent.classList.remove('active-tab-content');
    tripcomContent.classList.remove('active-tab-content');
    domesticTabBtn.classList.remove('active-tab');
    internationalTabBtn.classList.remove('active-tab');
    tripcomTabBtn.classList.remove('active-tab');
    if (tab === 'domestic') {
      domesticContent.classList.add('active-tab-content');
      domesticTabBtn.classList.add('active-tab');
    } else if (tab === 'international') {
      internationalContent.classList.add('active-tab-content');
      internationalTabBtn.classList.add('active-tab');
    } else if (tab === 'tripcom') {
      tripcomContent.classList.add('active-tab-content');
      tripcomTabBtn.classList.add('active-tab');
    }
  }
  if(domesticTabBtn) domesticTabBtn.addEventListener('click', () => setActiveTravelTab('domestic'));
  if(internationalTabBtn) internationalTabBtn.addEventListener('click', () => setActiveTravelTab('international'));
  if(tripcomTabBtn) tripcomTabBtn.addEventListener('click', () => setActiveTravelTab('tripcom'));

  // Labor tabs: honoraria, stipend, notes
  const honorariaTab = document.getElementById('honorariaTabBtn');
  const stipendTab = document.getElementById('stipendTabBtn');
  const notesTab = document.getElementById('notesTabBtn');
  const honorariaContentDiv = document.getElementById('honorariaContent');
  const stipendContentDiv = document.getElementById('stipendContent');
  const notesContentDiv = document.getElementById('notesContent');

  function setActiveLaborTab(tab) {
    honorariaContentDiv.classList.remove('active-tab-content');
    stipendContentDiv.classList.remove('active-tab-content');
    notesContentDiv.classList.remove('active-tab-content');
    honorariaTab.classList.remove('active-tab');
    stipendTab.classList.remove('active-tab');
    notesTab.classList.remove('active-tab');
    if (tab === 'honoraria') {
      honorariaContentDiv.classList.add('active-tab-content');
      honorariaTab.classList.add('active-tab');
    } else if (tab === 'stipend') {
      stipendContentDiv.classList.add('active-tab-content');
      stipendTab.classList.add('active-tab');
    } else if (tab === 'notes') {
      notesContentDiv.classList.add('active-tab-content');
      notesTab.classList.add('active-tab');
    }
  }
  if(honorariaTab) honorariaTab.addEventListener('click', () => setActiveLaborTab('honoraria'));
  if(stipendTab) stipendTab.addEventListener('click', () => setActiveLaborTab('stipend'));
  if(notesTab) notesTab.addEventListener('click', () => setActiveLaborTab('notes'));

  // Category cards
  const travelCard = document.querySelector('.reim-card[data-page="travel"]');
  const laborCard = document.querySelector('.reim-card[data-page="labor"]');
  if(travelCard) travelCard.addEventListener('click', showTravel);
  if(laborCard) laborCard.addEventListener('click', showLabor);

  const allBackBtns = document.querySelectorAll('.back-btn');
  allBackBtns.forEach(btn => {
    btn.addEventListener('click', (e) => {
      if(btn.getAttribute('data-back') === 'cover') showCover();
    });
  });

  showCover();
  setActiveTravelTab('domestic');
  setActiveLaborTab('honoraria');
</script>
</body>
</html>
