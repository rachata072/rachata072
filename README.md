<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Name — IT Support · Network Engineer · SOC Analyst</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { font-size: 16px; scroll-behavior: smooth; }

:root {
  --cisco-blue: #049fd9;
  --cisco-dark: #00476b;
  --cisco-deeper: #003049;
  --cisco-light: #e6f7fd;
  --cisco-mid: #b3e5f7;
  --ink: #1c2b35;
  --paper: #f7fbfd;
  --paper2: #edf6fb;
  --surface: #ffffff;
  --rule: #d0e8f2;
  --muted: #6b8fa0;
  --sans: 'Plus Jakarta Sans', system-ui, sans-serif;
  --mono: 'Space Mono', monospace;
}

body {
  background: var(--paper);
  color: var(--ink);
  font-family: var(--sans);
  font-size: 16px;
  line-height: 1.7;
  overflow-x: hidden;
}

/* ── MASTHEAD ── */
.masthead {
  background: var(--cisco-deeper);
  border-bottom: 3px solid var(--cisco-blue);
}

.masthead-top {
  display: flex;
  align-items: stretch;
  border-bottom: 1px solid rgba(4,159,217,0.25);
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 48px;
}

.masthead-meta {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .08em;
  color: rgba(255,255,255,0.45);
  padding: 10px 0;
  display: flex;
  align-items: center;
  flex: 1;
}

.masthead-nav {
  display: flex;
  align-items: stretch;
  margin-left: auto;
}

.masthead-nav a {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .1em;
  text-transform: uppercase;
  text-decoration: none;
  color: rgba(255,255,255,0.5);
  padding: 10px 16px;
  border-left: 1px solid rgba(4,159,217,0.2);
  display: flex;
  align-items: center;
  transition: all .15s;
}
.masthead-nav a:hover {
  color: var(--cisco-blue);
  background: rgba(4,159,217,0.08);
}

.masthead-main {
  max-width: 1200px;
  margin: 0 auto;
  padding: 44px 48px 40px;
  display: grid;
  grid-template-columns: 1fr auto;
  align-items: end;
  gap: 40px;
}

.masthead-name {
  font-family: var(--sans);
  font-size: clamp(3rem, 7vw, 6rem);
  font-weight: 700;
  line-height: .95;
  letter-spacing: -.03em;
  color: #ffffff;
}

.masthead-name span {
  color: var(--cisco-blue);
  font-weight: 300;
  font-style: italic;
  display: block;
  font-size: clamp(1.1rem, 2vw, 1.6rem);
  letter-spacing: .01em;
  margin-top: 10px;
  font-family: var(--sans);
}

.masthead-right {
  text-align: right;
  padding-bottom: 4px;
}

.role-stack {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 6px;
  margin-bottom: 20px;
}

.role-chip {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: .07em;
  color: var(--cisco-blue);
  background: rgba(4,159,217,0.12);
  border: 1px solid rgba(4,159,217,0.3);
  padding: 5px 12px;
  border-radius: 2px;
  white-space: nowrap;
}

.avail-block {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 5px;
}

.avail-badge {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  background: rgba(4,159,217,0.15);
  border: 1px solid rgba(4,159,217,0.35);
  color: #ffffff;
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .06em;
  padding: 7px 14px;
  border-radius: 2px;
}

.avail-dot {
  width: 6px; height: 6px;
  border-radius: 50%;
  background: #4ade80;
  animation: blink 2s ease-in-out infinite;
}

@keyframes blink { 0%,100%{opacity:1} 50%{opacity:.25} }

.avail-sub {
  font-family: var(--mono);
  font-size: 9px;
  color: rgba(255,255,255,0.35);
  letter-spacing: .07em;
}

/* ── BODY LAYOUT ── */
.body-wrap {
  display: grid;
  grid-template-columns: 1fr 300px;
  max-width: 1200px;
  margin: 0 auto;
  border-left: 1px solid var(--rule);
  border-right: 1px solid var(--rule);
  background: var(--surface);
  min-height: 100vh;
}

.main-col { border-right: 1px solid var(--rule); }
.aside-col { background: var(--paper); }

/* ── SECTION LABEL ── */
.sec-label {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: var(--cisco-blue);
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 28px;
}
.sec-label::after { content:''; flex:1; height:1px; background: var(--rule); }

/* ── LEDE ── */
.lede-block {
  padding: 44px 44px 40px;
  border-bottom: 1px solid var(--rule);
}

.lede-columns {
  display: grid;
  grid-template-columns: 1.1fr 1fr;
  gap: 44px;
  align-items: start;
}

.lede-drop {
  font-size: clamp(1.15rem, 2vw, 1.4rem);
  font-weight: 600;
  line-height: 1.45;
  color: var(--cisco-dark);
  margin-bottom: 16px;
  letter-spacing: -.01em;
}

.lede-body {
  font-size: 14px;
  line-height: 1.85;
  color: var(--muted);
  font-weight: 400;
}

.stat-entry {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  padding: 12px 0;
  border-bottom: 1px solid var(--rule);
  gap: 12px;
}
.stat-entry:first-child { border-top: 1px solid var(--rule); }

.stat-k {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .07em;
  text-transform: uppercase;
  color: var(--muted);
  white-space: nowrap;
}
.stat-v {
  font-size: 13px;
  font-weight: 600;
  color: var(--ink);
  text-align: right;
}

/* ── PROJECTS ── */
.projects-block { padding: 40px 44px 44px; }

.project-item {
  padding: 28px 0;
  border-bottom: 1px solid var(--rule);
  position: relative;
  padding-left: 20px;
}
.project-item:first-of-type { border-top: 1px solid var(--rule); }

.project-item::before {
  content: '';
  position: absolute;
  left: 0; top: 28px; bottom: 28px;
  width: 3px;
  background: var(--rule);
  border-radius: 2px;
  transition: background .2s;
}
.project-item:hover::before { background: var(--cisco-blue); }

.proj-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 16px;
  margin-bottom: 6px;
}

.proj-num {
  font-family: var(--mono);
  font-size: 10px;
  color: var(--cisco-blue);
  letter-spacing: .06em;
  margin-bottom: 6px;
}

.proj-h {
  font-size: 15px;
  font-weight: 700;
  line-height: 1.3;
  color: var(--ink);
  letter-spacing: -.01em;
}

.proj-gh {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .05em;
  color: var(--cisco-blue);
  text-decoration: none;
  white-space: nowrap;
  border-bottom: 1px solid rgba(4,159,217,0.4);
  padding-bottom: 1px;
  flex-shrink: 0;
  transition: opacity .15s;
}
.proj-gh:hover { opacity: .6; }

.proj-p {
  font-size: 13.5px;
  line-height: 1.8;
  color: var(--muted);
  margin-bottom: 14px;
  font-weight: 400;
}

.proj-chips { display: flex; flex-wrap: wrap; gap: 5px; }

.chip {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .03em;
  padding: 4px 10px;
  border: 1px solid var(--rule);
  color: var(--muted);
  background: var(--paper);
  border-radius: 2px;
}

.chip-blue {
  border-color: rgba(4,159,217,0.4);
  color: var(--cisco-dark);
  background: var(--cisco-light);
}

/* ── SIDEBAR ── */
.aside-header {
  background: var(--cisco-deeper);
  padding: 28px 28px 24px;
  border-bottom: 2px solid var(--cisco-blue);
}

.aside-header-label {
  font-family: var(--mono);
  font-size: 9px;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.4);
  margin-bottom: 8px;
}

.aside-header-text {
  font-size: 13px;
  font-weight: 500;
  color: rgba(255,255,255,0.9);
  line-height: 1.6;
}

.aside-block {
  padding: 28px;
  border-bottom: 1px solid var(--rule);
}

.aside-sec-label {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .13em;
  text-transform: uppercase;
  color: var(--cisco-blue);
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 18px;
}
.aside-sec-label::after { content:''; flex:1; height:1px; background:var(--rule); }

/* CERTS */
.cert-item {
  padding: 13px 0;
  border-bottom: 1px solid var(--rule);
}
.cert-item:last-child { border-bottom: none; }

.cert-badge { display: flex; align-items: flex-start; gap: 11px; }

.cert-icon {
  width: 34px; height: 34px;
  border-radius: 3px;
  display: flex; align-items: center; justify-content: center;
  font-family: var(--mono);
  font-size: 9px;
  flex-shrink: 0;
  text-align: center;
  line-height: 1.2;
  font-weight: 700;
}

.ci-cisco { background: #049fd9; color: #fff; }
.ci-aws   { background: #232f3e; color: #ff9900; }
.ci-isc   { background: #005396; color: #fff; }
.ci-goog  { background: #4285f4; color: #fff; }
.ci-ibm   { background: #1f70c1; color: #fff; }

.cert-name-sm { font-size: 12px; font-weight: 700; color: var(--ink); margin-bottom: 2px; line-height: 1.3; letter-spacing: -.01em; }
.cert-issuer-sm { font-family: var(--mono); font-size: 10px; color: var(--muted); }
.cert-earned { font-family: var(--mono); font-size: 9px; color: #16a34a; letter-spacing: .06em; text-transform: uppercase; margin-top: 4px; }

/* SKILLS */
.skill-group { margin-bottom: 16px; }
.skill-group:last-child { margin-bottom: 0; }

.skill-g-label {
  font-family: var(--mono);
  font-size: 9px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 7px;
}

.skill-pills { display: flex; flex-wrap: wrap; gap: 5px; }

.pill {
  font-size: 11px;
  font-weight: 500;
  padding: 4px 10px;
  background: var(--paper2);
  color: var(--ink);
  border-radius: 2px;
  border: 1px solid var(--rule);
  letter-spacing: -.01em;
}

.pill-em {
  background: var(--cisco-dark);
  color: #fff;
  border-color: var(--cisco-dark);
}

/* CONTACT */
.contact-line {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 12px 0;
  border-bottom: 1px solid var(--rule);
  text-decoration: none;
  color: var(--ink);
  transition: color .15s;
}
.contact-line:first-child { border-top: 1px solid var(--rule); }
.contact-line:hover { color: var(--cisco-blue); }
.contact-line:hover .cl-arrow { transform: translate(3px, -3px); }

.cl-type {
  font-family: var(--mono);
  font-size: 9px;
  letter-spacing: .09em;
  text-transform: uppercase;
  color: var(--muted);
  width: 52px;
  flex-shrink: 0;
}
.cl-val { font-size: 12px; font-weight: 600; flex: 1; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
.cl-arrow { font-size: 12px; color: var(--muted); transition: transform .15s; flex-shrink: 0; }

/* ── FOOTER ── */
footer {
  background: var(--cisco-deeper);
  border-top: 2px solid var(--cisco-blue);
  max-width: 1200px;
  margin: 0 auto;
  border-left: 1px solid rgba(4,159,217,0.2);
  border-right: 1px solid rgba(4,159,217,0.2);
  display: grid;
  grid-template-columns: 1fr 300px;
}

.footer-left {
  padding: 20px 44px;
  border-right: 1px solid rgba(4,159,217,0.2);
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 8px;
}

.footer-right {
  padding: 20px 28px;
  display: flex;
  align-items: center;
}

footer p, footer span {
  font-family: var(--mono);
  font-size: 10px;
  color: rgba(255,255,255,0.35);
  letter-spacing: .05em;
}

.footer-blue { color: var(--cisco-blue); }

/* ── REVEAL ── */
.sr { opacity: 0; transform: translateY(14px); transition: opacity .5s ease, transform .5s ease; }
.sr.in { opacity: 1; transform: translateY(0); }

/* ── RESPONSIVE ── */
@media (max-width: 900px) {
  .body-wrap { grid-template-columns: 1fr; border: none; }
  .main-col { border-right: none; }
  footer { grid-template-columns: 1fr; max-width: 100%; border-left: none; border-right: none; }
  .footer-left { border-right: none; border-bottom: 1px solid rgba(4,159,217,0.2); padding: 20px 24px; }
  .footer-right { padding: 16px 24px; }
  .masthead-main { grid-template-columns: 1fr; padding: 32px 24px 28px; }
  .masthead-right { text-align: left; }
  .role-stack { align-items: flex-start; }
  .avail-block { align-items: flex-start; }
  .lede-columns { grid-template-columns: 1fr; }
  .lede-block, .projects-block { padding: 28px 24px; }
  .aside-block, .aside-header { padding: 24px; }
  .masthead-top { padding: 0 24px; }
  .masthead-nav { display: none; }
}
</style>
</head>
<body>

<!-- MASTHEAD -->
<header class="masthead">
  <div class="masthead-top">
    <span class="masthead-meta">Portfolio — 2026 · Vancouver, BC</span>
    <nav class="masthead-nav">
      <a href="#projects">Projects</a>
      <a href="#certs">Credentials</a>
      <a href="#skills">Skills</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
  <div class="masthead-main">
    <h1 class="masthead-name">
      Your Name
      <span>IT Support &nbsp;·&nbsp; Network Engineer &nbsp;·&nbsp; SOC Analyst</span>
    </h1>
    <div class="masthead-right">
      <div class="role-stack">
        <span class="role-chip">IT Support Specialist</span>
        <span class="role-chip">Network Engineer</span>
        <span class="role-chip">SOC Analyst</span>
      </div>
      <div class="avail-block">
        <span class="avail-badge">
          <span class="avail-dot"></span>
          Open to opportunities
        </span>
        <span class="avail-sub">Canada relocation &nbsp;·&nbsp; Remote global</span>
      </div>
    </div>
  </div>
</header>

<div class="body-wrap">

  <!-- MAIN -->
  <main class="main-col">

    <div class="lede-block sr">
      <div class="lede-columns">
        <div>
          <p class="lede-drop">Hands-on IT professional with a strong foundation across support, networking, and security.</p>
          <p class="lede-body">Five industry certifications earned — CCNA, AWS Cloud Practitioner, ISC² CC, Google Cybersecurity, and IBM Data Science. Five portfolio projects built in real lab environments and documented for production readiness. Focused on Microsoft 365 administration, Active Directory, network analysis, and cloud security operations. Available for roles in Canada and remote positions globally.</p>
        </div>
        <div>
          <div class="stat-entry"><span class="stat-k">Certifications</span><span class="stat-v">5 Earned</span></div>
          <div class="stat-entry"><span class="stat-k">Portfolio projects</span><span class="stat-v">5 on GitHub</span></div>
          <div class="stat-entry"><span class="stat-k">Lab environment</span><span class="stat-v">GNS3 + Packet Tracer</span></div>
          <div class="stat-entry"><span class="stat-k">Cloud</span><span class="stat-v">AWS + Microsoft 365</span></div>
          <div class="stat-entry"><span class="stat-k">Location</span><span class="stat-v">Vancouver, BC</span></div>
          <div class="stat-entry"><span class="stat-k">Work preference</span><span class="stat-v">Canada · Remote global</span></div>
        </div>
      </div>
    </div>

    <div class="projects-block" id="projects">
      <p class="sec-label">02 — Portfolio projects</p>

      <div class="project-item sr">
        <p class="proj-num">PROJECT 01</p>
        <div class="proj-header">
          <h3 class="proj-h">M365 Developer Tenant — Full Admin Configuration</h3>
          <a href="https://github.com/yourusername/m365-admin-lab" target="_blank" class="proj-gh">↗ GitHub</a>
        </div>
        <p class="proj-p">Provisioned a Microsoft 365 Developer Tenant end-to-end: 10 users, Exchange Online mailboxes, SharePoint, Intune device compliance policies, and Defender for Business. Demonstrates real cloud admin capability across the full M365 stack — the most-asked-about environment in helpdesk and sysadmin interviews.</p>
        <div class="proj-chips">
          <span class="chip chip-blue">Microsoft 365</span>
          <span class="chip chip-blue">Azure AD / Entra</span>
          <span class="chip">Intune</span>
          <span class="chip">Exchange Online</span>
          <span class="chip">Defender for Business</span>
          <span class="chip">SharePoint</span>
        </div>
      </div>

      <div class="project-item sr">
        <p class="proj-num">PROJECT 02</p>
        <div class="proj-header">
          <h3 class="proj-h">Active Directory Home Lab — Windows Server 2022 + GPO</h3>
          <a href="https://github.com/yourusername/active-directory-home-lab" target="_blank" class="proj-gh">↗ GitHub</a>
        </div>
        <p class="proj-p">Built a full Active Directory environment on local VMs: Windows Server 2022 domain controller, OU structure for IT / HR / Finance departments, 5 Group Policies covering password policy, drive mapping, and security restrictions. Domain-joined a Windows 11 client and verified all policies. Includes gpresult reports and a network topology diagram.</p>
        <div class="proj-chips">
          <span class="chip chip-blue">Active Directory DS</span>
          <span class="chip chip-blue">Group Policy (GPO)</span>
          <span class="chip">Windows Server 2022</span>
          <span class="chip">DNS & DHCP</span>
          <span class="chip">VirtualBox</span>
        </div>
      </div>

      <div class="project-item sr">
        <p class="proj-num">PROJECT 03</p>
        <div class="proj-header">
          <h3 class="proj-h">Freshservice ITSM — 20-Ticket Helpdesk Simulation</h3>
          <a href="https://github.com/yourusername/freshservice-itsm-lab" target="_blank" class="proj-gh">↗ GitHub</a>
        </div>
        <p class="proj-p">Configured Freshservice from scratch — service catalog, three SLA tiers, and ticket categories — then created and resolved 20 realistic helpdesk tickets across password resets, VPN access, printer issues, new hire onboarding, and hardware replacements. Demonstrates PSA familiarity that MSP roles expect on day one.</p>
        <div class="proj-chips">
          <span class="chip chip-blue">Freshservice</span>
          <span class="chip chip-blue">ITSM / PSA</span>
          <span class="chip">SLA Management</span>
          <span class="chip">Ticket lifecycle</span>
          <span class="chip">MSP workflows</span>
        </div>
      </div>

      <div class="project-item sr">
        <p class="proj-num">PROJECT 04</p>
        <div class="proj-header">
          <h3 class="proj-h">Wireshark — Protocol Capture & Network Analysis</h3>
          <a href="https://github.com/yourusername/wireshark-network-analysis" target="_blank" class="proj-gh">↗ GitHub</a>
        </div>
        <p class="proj-p">Captured and annotated five network scenarios: DNS query/response, TCP 3-way handshake, HTTP vs HTTPS payload comparison, ICMP echo analysis, and packet loss detection via I/O graphs. Each capture ships as a .pcap file with written analysis explaining what the packets reveal about protocol behaviour.</p>
        <div class="proj-chips">
          <span class="chip chip-blue">Wireshark</span>
          <span class="chip chip-blue">TCP/IP</span>
          <span class="chip">DNS</span>
          <span class="chip">HTTP / HTTPS</span>
          <span class="chip">ICMP</span>
          <span class="chip">CCNA-aligned</span>
        </div>
      </div>

      <div class="project-item sr">
        <p class="proj-num">PROJECT 05</p>
        <div class="proj-header">
          <h3 class="proj-h">IT Runbook — 5 Standard Operating Procedures</h3>
          <a href="https://github.com/yourusername/it-runbook-sops" target="_blank" class="proj-gh">↗ GitHub</a>
        </div>
        <p class="proj-p">A 30-page professional runbook with five fully-documented SOPs: new employee onboarding, account offboarding, password reset and lockout workflow, laptop setup checklist, and network connectivity troubleshooting using OSI-layer methodology. Formatted for MSP and enterprise use with escalation paths and revision history.</p>
        <div class="proj-chips">
          <span class="chip chip-blue">SOPs</span>
          <span class="chip chip-blue">IT Runbook</span>
          <span class="chip">Onboarding / Offboarding</span>
          <span class="chip">Troubleshooting</span>
          <span class="chip">MSP-ready</span>
        </div>
      </div>
    </div>
  </main>

  <!-- SIDEBAR -->
  <aside class="aside-col">

    <div class="aside-header">
      <p class="aside-header-label">Availability</p>
      <p class="aside-header-text">Open to IT Support, Network Engineer, and SOC Analyst roles. Available for positions across Canada and remote opportunities worldwide.</p>
    </div>

    <div class="aside-block sr" id="certs">
      <p class="aside-sec-label">01 — Credentials</p>

      <div class="cert-item">
        <div class="cert-badge">
          <div class="cert-icon ci-cisco">Cisco</div>
          <div>
            <p class="cert-name-sm">CCNA</p>
            <p class="cert-issuer-sm">Cisco — 200-301</p>
            <p class="cert-earned">✓ Earned</p>
          </div>
        </div>
      </div>

      <div class="cert-item">
        <div class="cert-badge">
          <div class="cert-icon ci-aws">AWS</div>
          <div>
            <p class="cert-name-sm">AWS Cloud Practitioner</p>
            <p class="cert-issuer-sm">Amazon Web Services</p>
            <p class="cert-earned">✓ Earned</p>
          </div>
        </div>
      </div>

      <div class="cert-item">
        <div class="cert-badge">
          <div class="cert-icon ci-isc">ISC²</div>
          <div>
            <p class="cert-name-sm">CC — Certified in Cybersecurity</p>
            <p class="cert-issuer-sm">ISC²</p>
            <p class="cert-earned">✓ Earned</p>
          </div>
        </div>
      </div>

      <div class="cert-item">
        <div class="cert-badge">
          <div class="cert-icon ci-goog">G</div>
          <div>
            <p class="cert-name-sm">Google Cybersecurity Certificate</p>
            <p class="cert-issuer-sm">Google / Coursera</p>
            <p class="cert-earned">✓ Earned</p>
          </div>
        </div>
      </div>

      <div class="cert-item">
        <div class="cert-badge">
          <div class="cert-icon ci-ibm">IBM</div>
          <div>
            <p class="cert-name-sm">Data Science Professional</p>
            <p class="cert-issuer-sm">IBM / Coursera</p>
            <p class="cert-earned">✓ Earned</p>
          </div>
        </div>
      </div>
    </div>

    <div class="aside-block sr" id="skills">
      <p class="aside-sec-label">03 — Skills</p>

      <div class="skill-group">
        <p class="skill-g-label">Cloud & Identity</p>
        <div class="skill-pills">
          <span class="pill pill-em">Microsoft 365</span>
          <span class="pill pill-em">AWS</span>
          <span class="pill">Azure AD</span>
          <span class="pill">Intune</span>
          <span class="pill">Entra ID</span>
        </div>
      </div>

      <div class="skill-group">
        <p class="skill-g-label">Systems</p>
        <div class="skill-pills">
          <span class="pill pill-em">Active Directory</span>
          <span class="pill">Windows Server 2022</span>
          <span class="pill">GPO</span>
          <span class="pill">DNS / DHCP</span>
          <span class="pill">Ubuntu Linux</span>
        </div>
      </div>

      <div class="skill-group">
        <p class="skill-g-label">Networking</p>
        <div class="skill-pills">
          <span class="pill pill-em">CCNA</span>
          <span class="pill">Wireshark</span>
          <span class="pill">GNS3</span>
          <span class="pill">Packet Tracer</span>
          <span class="pill">TCP/IP</span>
          <span class="pill">VLANs</span>
        </div>
      </div>

      <div class="skill-group">
        <p class="skill-g-label">Security</p>
        <div class="skill-pills">
          <span class="pill pill-em">ISC² CC</span>
          <span class="pill">Google Cybersecurity</span>
          <span class="pill">Defender for Business</span>
          <span class="pill">MFA / Conditional Access</span>
        </div>
      </div>

      <div class="skill-group">
        <p class="skill-g-label">ITSM & Data</p>
        <div class="skill-pills">
          <span class="pill">Freshservice</span>
          <span class="pill">Python</span>
          <span class="pill">PowerShell</span>
          <span class="pill">Git / GitHub</span>
          <span class="pill">IBM Data Science</span>
        </div>
      </div>
    </div>

    <div class="aside-block sr" id="contact">
      <p class="aside-sec-label">04 — Contact</p>

      <a href="mailto:you@email.com" class="contact-line">
        <span class="cl-type">Email</span>
        <span class="cl-val">you@email.com</span>
        <span class="cl-arrow">↗</span>
      </a>
      <a href="https://linkedin.com/in/yourprofile" target="_blank" class="contact-line">
        <span class="cl-type">LinkedIn</span>
        <span class="cl-val">linkedin.com/in/yourprofile</span>
        <span class="cl-arrow">↗</span>
      </a>
      <a href="https://github.com/yourusername" target="_blank" class="contact-line">
        <span class="cl-type">GitHub</span>
        <span class="cl-val">github.com/yourusername</span>
        <span class="cl-arrow">↗</span>
      </a>
      <a href="/resume.pdf" class="contact-line">
        <span class="cl-type">Resume</span>
        <span class="cl-val">Download PDF</span>
        <span class="cl-arrow">↗</span>
      </a>
    </div>

  </aside>
</div>

<footer>
  <div class="footer-left">
    <span>© 2026 <span class="footer-blue">Your Name</span></span>
    <span>IT Support · Network Engineer · SOC Analyst</span>
    <span>Hosted on GitHub Pages</span>
  </div>
  <div class="footer-right">
    <span>Canada relocation &nbsp;·&nbsp; Remote global</span>
  </div>
</footer>

<script>
const io = new IntersectionObserver(entries => {
  entries.forEach((e, i) => {
    if (e.isIntersecting) {
      setTimeout(() => e.target.classList.add('in'), i * 70);
      io.unobserve(e.target);
    }
  });
}, { threshold: 0.06 });
document.querySelectorAll('.sr').forEach(el => io.observe(el));
</script>
</body>
</html>