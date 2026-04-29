# Portofolio
My Portofolio

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hanifah | Portfolio</title>

<style>
/* CSS RESET & BASE */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Arial, sans-serif;
    background: #fcfcfd;
    color: #333;
    line-height: 1.6;
}

/* HERO SECTION */
header {
    background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), 
                url('bg.jfif'); 
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    color: white;
    text-align: center;
    padding: 120px 30px;
}

header h1 {
    font-size: 50px;
    letter-spacing: 2px;
}

header h3 {
    margin-top: 10px;
    font-weight: normal;
    font-style: italic;
    color: #b1efb1;
}

header p {
    margin-top: 20px;
    max-width: 700px;
    margin-inline: auto;
    font-size: 1.1rem;
}

/* SECTION LAYOUT */
section {
    max-width: 1000px;
    margin: auto;
    padding: 50px 20px;
}

h2 {
    margin-bottom: 25px;
    border-left: 5px solid #44a424;
    padding-left: 15px;
}

/* CARD SYSTEM */
.card {
    background: white; /* Diubah dari abu-abu ke putih agar clean */
    padding: 25px;
    margin-bottom: 20px;
    border-radius: 12px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
}

/* CARD WITH BACKGROUNDS */
.about-card {
    background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('me.jfif');
    background-size: cover;
    background-position: center;
    color: white;
    border: none;
}

.experience-card {
    background: linear-gradient(rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0.75)), url('bgtuku.jfif');
    background-size: cover;
    background-position: center;
    color: white;
    border: none;
}

.about-card strong, .experience-card h3, .experience-card p b {
    color: #b1efb1;
}

/* PROJECT GRID */
.projects {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
}

@media (max-width: 768px) {
    .projects { grid-template-columns: 1fr; }
    header h1 { font-size: 35px; }
}

/* CERTIFICATIONS & BUTTONS */
.cert-card {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.provider {
    color: #44a424;
    font-weight: bold;
    font-size: 14px;
}

.btn-cert {
    display: inline-block;
    color: #4facfe;
    text-decoration: none;
    font-size: 13px;
    font-weight: bold;
    border: 1px solid #4facfe;
    padding: 5px 12px;
    border-radius: 4px;
    transition: 0.3s;
}

.btn-cert:hover {
    background: #4facfe;
    color: white;
}

/* MODAL / POP-UP SYSTEM */
.modal-overlay {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    background: rgba(0, 0, 0, 0.85);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    opacity: 0;
    visibility: hidden;
    transition: 0.3s;
}

.modal-overlay:target {
    opacity: 1;
    visibility: visible;
}

.modal-content {
    background: white;
    padding: 15px;
    border-radius: 8px;
    max-width: 90%;
    max-height: 90%;
    position: relative;
    text-align: center;
}

.modal-content img {
    max-width: 100%;
    max-height: 70vh;
    border-radius: 4px;
}

.modal-close {
    position: absolute;
    top: -15px; right: -15px;
    background: #44a424;
    color: white;
    width: 35px; height: 35px;
    border-radius: 50%;
    text-decoration: none;
    line-height: 35px;
    font-weight: bold;
}

.modal-close-area {
    position: absolute;
    width: 100%; height: 100%;
}

/* SKILLS TAGS */
.skills span {
    display: inline-block;
    background: linear-gradient(90deg, #44a424, #b1efb1);
    color: white;
    padding: 8px 15px;
    margin: 5px;
    border-radius: 20px;
    font-size: 14px;
    font-weight: bold;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 40px 20px;
    background: #333;
    color: white;
}

footer a { color: #b1efb1; text-decoration: none; margin: 0 10px; }
</style>
</head>

<body>

<header>
    <h1>Hanifah</h1>
    <h3>"Where Logic Meets Latte"</h3>
    <p>
        Beyond pulling shots, I apply my education background to streamline coffee operations. 
        I focus on making the bar run like a well-oiled machine—from maintaining precise 
        financial records and inventory to delivering a seamless experience for every customer.
    </p>
</header>

<section>
    <h2>About Me</h2>
    <div class="card about-card">
        <p style="margin-bottom: 15px;">
            I have hands-on experience in fast-paced operational environments, where I developed strong problem-solving,
            multitasking, and decision-making skills.
        </p>
        <p>
            With a background in <strong>Informatics Engineering</strong>, I am interested in using data and technology
            to improve business operations and efficiency.
        </p>
    </div>
</section>

<section>
    <h2>Education</h2>
    <div class="card">
        <p><strong>Bachelor’s Degree in Computer Science (2025)</strong></p>
        <p>Budi Luhur University, Jakarta, Indonesia | GPA: 3.58</p>
        <p style="font-size: 0.9rem; margin-top: 10px; color: #666;">
            Relevant Coursework: Data Analysis, Database Management, Information Systems, Basic Programming. 
            Developed skills in data processing, accuracy, and structured problem solving.
        </p>
    </div>
</section>

<section>
    <h2>Experience</h2>
    <div class="card experience-card">
        <h3>Barista & Ops — Toko Kopi Tuku (July 2022 – April 2026)</h3>
        
        <p style="font-weight: bold; margin-top: 15px;">Commercial & Events:</p>
        <ul style="padding-left: 20px; margin-bottom: 15px;">
            <li>Managed bulk orders and coffee activations for corporate/private events with high precision.</li>
            <li>Represented the brand in major exhibitions, handling booth operations and customer relations.</li>
            <li>Served as <b>PIC for 4 Cloud Kitchen outlets</b>, coordinating daily operations and team workflows.</li>
        </ul>

        <p style="font-weight: bold;">Operational & Finance (ERP System):</p>
        <ul style="padding-left: 20px;">
            <li>Handled <b>PO processing and data entry via ERP system</b> with 100% data accuracy.</li>
            <li>Managed cash/cashless transactions, reconciliation, and daily sales reporting.</li>
            <li>Supervised inventory levels, petty cash tracking, and stock management.</li>
        </ul>
    </div>
</section>

<section>
    <h2>Academic Projects</h2>
    <div class="projects">
        <div class="card">
            <h3>Sales Data Encryption (AES-256)</h3>
            <p>Developed a secure web-based system to protect daily sales transaction data using AES-256 encryption.</p>
            <ul style="margin-top:10px; padding-left: 20px;">
                <li>Implemented PHP-based AES-256 encryption/decryption</li>
                <li>Integrated MySQL for secure financial data storage</li>
                <li>Applied data security principles to sensitive records</li>
            </ul>
        </div>
    </div>
</section>

<section>
    <h2>Certifications</h2>
    <div class="projects">
        <div class="card cert-card">
            <div>
                <h3>Basic Computer Algorithm Competency</h3>
                <p class="provider">Universitas Budi Luhur</p>
            </div>
            <a href="#cert1" class="btn-cert">View ↗</a>
        </div>

        <div class="card cert-card">
            <div>
                <h3>Intermediate Barista Toko Kopi Tuku</h3>
                <p class="provider">Barista Academy</p>
            </div>
            <a href="#cert2" class="btn-cert">View ↗</a>
        </div>
    </div>
</section>

<section>
    <h2>Skills</h2>
    <div class="card">
        <h4 style="margin-bottom:10px;">Technical</h4>
        <div class="skills">
            <span>Microsoft Office</span>
            <span>PHP</span>
            <span>SQL (Basic)</span>
            <span>System Logic</span>
            <span>Networking</span>
        </div>

        <h4 style="margin-top:20px; margin-bottom:10px;">Core</h4>
        <div class="skills">
            <span>Problem Solving</span>
            <span>Operational Strategy</span>
            <span>Demand Forecasting</span>
            <span>Adaptability</span>
        </div>
    </div>
</section>

<div id="cert1" class="modal-overlay">
    <a href="#" class="modal-close-area"></a> 
    <div class="modal-content">
        <a href="#" class="modal-close">&times;</a> 
        <img src="algo.jpg" alt="Basic Computer Algorithm Competency">
        <p style="margin-top:10px; font-weight:bold;">Verified Basic Computer Algorithm Competency Certification</p>
    </div>
</div>

<div id="cert2" class="modal-overlay">
    <a href="#" class="modal-close-area"></a>
    <div class="modal-content">
        <a href="#" class="modal-close">&times;</a>
        <img src="barista.jpg" alt="Intermediate Barista Toko Kopi Tuku">
        <p style="margin-top:10px; font-weight:bold;">Verified Intermediate Barista Toko Kopi Tuku Certification</p>
    </div>
</div>

<footer>
    <p>Contact Me</p>
    <div style="margin: 15px 0;">
        <a href="mailto:hanifahneness@gmail.com">Email</a> | 
        <a href="https://www.linkedin.com/in/hanifahhan" target="_blank">LinkedIn</a> | 
        <a href="https://github.com/username-kamu" target="_blank">GitHub</a>
    </div>
    <p style="font-size: 11px; opacity: 0.5;">&copy; 2026 Hanifah Portfolio</p>
</footer>

</body>
</html>
