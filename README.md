# BIMSA-Rembursement-Guideline
This is about reimbursement
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>BIMSA Finance Reimbursement Guideline</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            background: #f0f4f8;
            color: #1a2c3e;
            padding: 2rem 1rem;
            line-height: 1.5;
        }

        .container {
            max-width: 1280px;
            margin: 0 auto;
            background: white;
            border-radius: 32px;
            box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            padding: 2rem 2rem 3rem 2rem;
        }

        /* 标题区 */
        .header {
            text-align: center;
            border-bottom: 3px solid #0f5b8c;
            padding-bottom: 1.2rem;
            margin-bottom: 2rem;
        }

        .header h1 {
            font-size: 2.2rem;
            color: #0f5b8c;
            letter-spacing: -0.5px;
            font-weight: 600;
        }

        .header p {
            color: #4a627a;
            font-size: 1rem;
            margin-top: 0.5rem;
        }

        /* 卡片样式 */
        .section-card {
            background: #ffffff;
            border-radius: 24px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
            margin-bottom: 2.2rem;
            border: 1px solid #e2edf2;
            overflow: hidden;
            transition: all 0.2s;
        }

        .section-title {
            background: #eef5fa;
            padding: 1rem 1.8rem;
            font-size: 1.6rem;
            font-weight: 600;
            color: #0a4b6e;
            border-left: 6px solid #2c7da0;
            letter-spacing: -0.3px;
        }

        .section-content {
            padding: 1.5rem 1.8rem;
        }

        /* 网格布局 */
        .grid-2col {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.8rem;
        }

        @media (max-width: 780px) {
            .grid-2col {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }

            .container {
                padding: 1.5rem;
            }
        }

        .info-block {
            background: #f9fdfe;
            border-radius: 20px;
            padding: 1rem 1.4rem;
            margin-bottom: 1.2rem;
            border-left: 4px solid #61a5c2;
        }

        .info-block strong {
            color: #1f5e7e;
            display: inline-block;
            margin-bottom: 0.25rem;
        }

        .list-styled {
            padding-left: 1.4rem;
            margin: 0.8rem 0;
        }

        .list-styled li {
            margin: 0.5rem 0;
        }

        hr {
            margin: 1rem 0;
            border: 0;
            height: 1px;
            background: #cbdde6;
        }

        .badge {
            background: #eaf4e8;
            color: #2f6b3c;
            font-size: 0.75rem;
            font-weight: 500;
            padding: 0.2rem 0.6rem;
            border-radius: 30px;
            display: inline-block;
            margin-left: 0.6rem;
            vertical-align: middle;
        }

        .highlight {
            background: #fff1d6;
            padding: 0.8rem 1rem;
            border-radius: 16px;
            font-family: monospace;
            font-size: 0.85rem;
            border: 1px solid #ffe0b5;
            margin: 0.8rem 0;
        }

        .tax-number {
            background: #eef2fa;
            font-family: monospace;
            font-weight: 500;
            padding: 0.3rem 0.6rem;
            border-radius: 12px;
            display: inline-block;
        }

        .step-list {
            counter-reset: step;
            list-style: none;
            padding-left: 0;
        }

        .step-list li {
            counter-increment: step;
            margin-bottom: 0.6rem;
            padding-left: 1.8rem;
            position: relative;
        }

        .step-list li::before {
            content: "Step " counter(step);
            position: absolute;
            left: 0;
            font-weight: bold;
            color: #2c7da0;
        }

        .link-style {
            color: #1f6392;
            text-decoration: none;
            border-bottom: 1px dotted #7fbbda;
        }

        .link-style:hover {
            color: #0f3b54;
        }

        table.standard-table {
            width: 100%;
            border-collapse: collapse;
            margin: 1rem 0;
        }

        table.standard-table th,
        table.standard-table td {
            border: 1px solid #cbdde6;
            padding: 0.75rem;
            text-align: left;
            vertical-align: top;
        }

        table.standard-table th {
            background: #e2edf2;
            font-weight: 600;
        }

        .footnote {
            font-size: 0.85rem;
            color: #5e7e9a;
            border-top: 1px solid #dce5ec;
            margin-top: 1.2rem;
            padding-top: 0.8rem;
        }

        @media print {
            body {
                background: white;
                padding: 0;
            }

            .section-card {
                break-inside: avoid;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="header">
            <h1>📘 BIMSA Reimbursement Guideline</h1>
            <p>BIMSA | Documents required for reimbursement</p>
        </div>

        <!-- Domestric travel + International travel 左右两列 -->
        <div class="grid-2col">
            <!-- Domestic travel -->
            <div class="section-card">
                <div class="section-title">✈️ Domestic Travel</div>
                <div class="section-content">
                    <div class="info-block"><strong>📋 Basic Documents</strong><br>Leave Application form (Funding
                        Source);</br> Invitation letter or conference notification; </br></div>
                    <div class="info-block"><strong>🛫 Flight</strong><br>
                        - Boarding Passes (photo or original);<br>
                        - Chinese VAT invoice (note in the remark: itinerary, passenger info, etc.);<br>
                        - Online order page or booking confirmation email, showing price breakdown, passenger and
                        itinerary info;<br>
                        - Payment Proof (when the payment is more than 1w);

                    </div>
                    <div class="info-block"><strong>🚖 Car ride to and from the airport</strong><br>itinerary;</br>
                        Chinese VAT invoice;</br></div>
                    <div class="info-block"><strong>🚆 Train</strong><br>
                        - Online order page (if it’s online booking)<br>
                        - Train ticket invoice (can only be issued through the official China Railway app 122306 or from
                        the train station ticketing counter)<br>
                        📎 <a class="link-style" href="https://www.12306.cn/en/index.html" target="_blank">12036
                            Ticketing website</a> |
                        <a class="link-style"
                            href="http://www.china-railway.com.cn/english/businesses/passenger/202411/t20241115_139137.html"
                            target="_blank">Guide on invoice issurance from 12306 app</a>
                    </div>
                    <div class="highlight">
                        🧾 <strong>For invited visitors</strong>：if any support shall be provided, please inform
                        Research Affairs Department in advance to obtain the VP’s consent, the screenshot of which is
                        required by the finance.
                    </div>
                </div>
            </div>

            <!-- 国际差旅 -->
            <div class="section-card">
                <div class="section-title">🌍 International Travel</div>
                <div class="section-content">
                    <div class="info-block"><strong>📄 Basic documents</strong><br>-Leave Application;</br> -Invitation
                        email;</br> -Passport photo-page</br></div>
                    <div class="info-block"><strong>✈️ Flight</strong><br>- Boarding Passes (photo or original);<br>
                        - Air ticket invoice/ receipt;<br>
                        - Online order page or booking confirmation email, showing price breakdown, passenger and
                        itinerary info;<br>
                        - Payment Proof;</div>
                    <div class="info-block"><strong>🏨 Accommodation</strong><br>Hotel Invoice/ receipt;</br> Hotel
                        folio, specifying the price breakdown, check-in and check-out date, and with hotel’s official
                        seal);</br></div>
                    <div class="info-block"><strong>🚖 Car ride to and from the airport</strong><br>itinerary;</br>
                        Chinese VAT invoice;</br></div>
                    <div class="highlight">
                        🧾 <strong>Please note:</strong>：If the air tickets or hotel are booked on Trip.com, the Chinese
                        VAT invoice is needed.

                    </div>
                </div>
            </div>
        </div>

        <!-- Trip.com 增值税发票获取步骤 + 财务信息 -->
        <div class="section-card">
            <div class="section-title">🧾 How to get Chinese VAT invoice from Trip.com?</div>
            <div class="section-content">
                <ul class="step-list">
                    <li><br>Go to My bookings;</li>
                    <li><br>Choose your bookings of the hotel or flight;</li>
                    <li><br>Go to Service Chat and select Chinese VAT invoice;</li>
                    <li><br>Text in the chatbox the tax number and the Chinese name of BIMSA (see below)<br>
                        <span class="tax-number">🏢 <strong>Chinese Name：<highlight>北京雁栖湖应用数学研究院</highlight></strong>
                        </span><br>
                        <span class="tax-number">🔢 <strong>Tax Number：<highlight>52110000MJ0166456X</highlight>
                            </strong></span>
                    </li>
                    </dv>
                </ul>
                <div class="footnote">※ Please make sure the invoice information is correct</div>
            </div>
        </div>

        <!-- 交通标准 + 住宿标准 + 北京住宿规定 -->
        <div class="grid-2col">
            <div class="section-card">
                <div class="section-title">🚗 Transport Standard</div>
                <div class="section-content">
                    <p><br><strong>Professors</strong> are eligible for:<br>✈️ Airplane-<span
                            style="color: red;"><strong>Business Class</strong></span>/ Economy Class<br>🚆Train- <span
                            style="color: red;"><strong>First Class</strong></span><br>
                        Please refer to Page 15 (domestic travel) and Page 27 (international travel) of the <i><a
                                href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf">Financial
                                Handbook (First Edition)</a></i></p>
                </div>
            </div>
            <div class="section-card">
                <div class="section-title">🏨 Accommodation Standard within China</div>
                <div class="section-content">
                    <p><br>Upper limit for <strong>Professors:</strong> <br>Beijing/ Shanghai: 1080 RMB per night<br>
                    </p>
                    <p>Please refer to Page 15 of the <i><a
                                href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\Financial Handbook（First Edition）.pdf">Financial
                                Handbook (First Edition)</a></i> for more information</p>
                </div> 🔹 <strong>Additional Finance Regulations on Accommodations in Beijing</strong>：</p>
                <ul class="list-styled">
                    <li>Participating in academic exchanges or other official activities within Beijing shall not be
                        regarded as business trip, and in principle, the accommodation expenses incurred shall not be
                        reimbursed.</li>
                    <li>If one need to stay in the hotel regularly or frequently due to teaching or other work needs,
                        one need to report to <strong>the VP in charge for approval</strong> in advance. </li>
                    <li>If the hotel stay is only one night, no prior approval is required. If it exceedes one night,
                        one must obtain approval in advance.</li>
                </ul>
            </div>


        </div>

        <!-- 会议费用 + 每日补助标准 (Per diem) -->
        <div class="section-card">
            <div class="section-title">Per diem allowance for meals and miscellaneous fees</div>
            <div class="section-content">
                <div class="grid-1col">
                    <p class="small-text">Per diem is counted in accordance with the dates of departure and arrival
                        mentioned in the leave application form.</p>
                </div>
                <div>
                    <table class="standard-table">
                        <thead>
                            <tr>
                                <th>Length of the trip</th>
                                <th>Allowance standard</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>trips ≤ 10 days</td>
                                <td>full allowance</td>
                            </tr>
                            <tr>
                                <td>10 days ＜ trips ≤ 15 days</td>
                                <td>10 day's full allowance + extra day's half allowance</td>
                            </tr>
                            <tr>
                                <td>trips ≥ 15 days</td>
                                <td>10 day's full allowance + 5 day's half allowance</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
            <div class="highlight" style="background: #eef5fa;">
                <h3>Allowances for trips within China:</h3> Meals 100 RMB/day;<br>Local Transport 80 RMB/day.
            </div>
        </div>

        <!-- 劳务费 (Honoraria / 讲学费) + 访问学生津贴 -->
        <div class="section-card">
            <div class="section-title">👥 Labor Service Fee / Honoraria</div>
            <div class="section-content">
                <div class="grid-1col">
                    <div>
                        <strong>🎤 Honorarium per engagement</strong>
                        <ul class="list-styled">
                            <li>Guests from outside Beijing：<strong>2000 RMB</strong></li>
                            <li>Guests from institutes within Beijing：<strong>1000 RMB</strong></li>
                            <li>Guests from Tsinghua University：<strong>500 RMB</strong></li>
                        </ul>
                        <strong>📑 Documents needed：</strong>
                        <ul class="list-styled">
                            <li>Printed webpage of the talk description (including the date, time, and abstract)</li>
                            <li>Photocopy of the passport or Chinese ID card of the recipient</li>
                            <li>Bank details and phone number of the recipient</li>
                            <li>Labor service fee invoice (required when the amount is 1000 RMB or above)</li>
                        </ul>
                        <div class="highlight">
                            <strong>Please note:</strong><br>
                            - The payee shall get the invoice on their own through <strong>the Tax Bureau App</strong>
                            released by the National Tax Bureau of China. An instruction on self-issuing the labor
                            service fee invoice has been provided by the finance<br>English version:<a
                                href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\劳务费发票\Instructions for Issuing Invoice for Labor Service.docx">
                                <li>Instructions for Issuing Invoice for Labor Service</li>
                            </a><br>
                            Chinese version:<li><a
                                    href="D:\WORK BIMSA\REIMBURSE\Others\Reimburse info\劳务费发票\劳务发票开具说明.docx">《劳务发票开具说明》</a>
                            </li>
                            - But for foreign nationals who <strong>first</strong> sign up this app, they’ll need a
                            <strong>registration code</strong>, which can only be obtained from the Tax Hall in person
                            and is valid for seven days.
                        </div>
                    </div>
                    <div>
                        <strong>🎓 Stipend for visiting students</strong>
                        <ul class="list-styled">
                            <li>The cap that can be offered to students: <strong>9900 RMB/month</strong></li>
                            <li><strong>Documents needed:</strong> Application form, student identity verification, bank
                                account details, and approval from the supervising professor.</li>
                        </ul>
                        <div class="highlight" style="margin-top: 10px;">
                            📌 For visiting students, the stipend is processed monthly. Ensure all supporting documents
                            (attendance record, supervisor’s sign-off) are submitted to finance before the 20th of each
                            month.
                        </div>
                    </div>
                </div>
                <hr>
                <div class="footnote">
                    <strong>💡 Special reminder:</strong> For honoraria ≥1000 RMB, a labor service invoice must be
                    self-issued by the payee via the National Tax Bureau App. Foreign nationals registering for the
                    first time must obtain a registration code in person at the Tax Service Hall in advance.
                </div>
            </div>
        </div>

        <!-- 采购及其他补充 -->
        <div class="section-card">
            <div class="section-title">📦 Procurement & Other Important Notes</div>
            <div class="section-content">
                <p><strong>🎫 Boarding Pass</strong> is a mandatory reimbursement attachment. Please keep the original
                    or a clear photo/scan.</p>
                <p><strong>🧾 Train Ticket Reimbursement Voucher:</strong> Only electronic/paper vouchers obtained via
                    the official "Railway 12306" app or station ticket counters are accepted. Third-party booking pages
                    are not direct reimbursement vouchers but serve as supplementary proof.</p>
                <p><strong>🏨 Hotel Accommodation (Beijing):</strong> Multiple overnight stays in Beijing require prior
                    VP approval, and the approval screenshot must be submitted to the finance department.</p>
                <p><strong>✈️ International Travel Reminder:</strong> In addition to the hotel folio, the accommodation
                    invoice must bear the hotel’s official stamp. Airport transfers require a Chinese VAT invoice.</p>
                <div class="highlight">
                    📢 All reimbursement applications must comply with the latest version of the "Supplementary
                    Regulations on Travel Reimbursement" and the Financial Handbook. Preparing all required documents in
                    advance will expedite the review process.
                </div>
            </div>
        </div>

        <!-- 附录快速索引 -->
        <div class="section-card">
            <div class="section-title">🔗 Quick Links & Resources</div>
            <div class="section-content">
                <ul class="list-styled">
                    <li>🚄 China Railway 12306 Official Website (English): <a class="link-style"
                            href="https://www.12306.cn/en/index.html"
                            target="_blank">https://www.12306.cn/en/index.html</a></li>
                    <li>📘 12306 e-Invoice Issuance Guide: <a class="link-style"
                            href="http://www.china-railway.com.cn/english/businesses/passenger/202411/t20241115_139137.html"
                            target="_blank">china-railway.com.cn English Guide</a></li>
                    <li>📑 <a class="link-style" href="#">BIMSA Reimbursement Regulations (Internal)</a> – please
                        contact finance for the latest version.</li>
                    <li>📞 Finance Consultation: The Research Affairs Department assists foreign experts with the
                        registration code for the Tax App. Please contact them in advance.</li>
                </ul>
            </div>
        </div>

        <!-- 底部备注 -->
        <div
            style="margin-top: 2rem; text-align: center; font-size: 0.8rem; color: #6c8dae; border-top: 1px solid #dce5ec; padding-top: 1.2rem;">
            Beijing Yanqi Lake Institute of Applied Mathematics | Finance Department · Version 2025 · In case of
            updates, the latest financial handbook shall prevail.<br>
            This guideline is for internal reimbursement reference only. All materials must be authentic and compliant.
        </div>
    </div>
</body>

</html>
