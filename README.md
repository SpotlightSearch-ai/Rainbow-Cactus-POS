[Spotlight Live OS.dc.html](https://github.com/user-attachments/files/31339532/Spotlight.Live.OS.dc.html)
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="./support.js"></script>
</head>
<body>
<x-dc>
<helmet>
<link rel="stylesheet" href="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/tokens/colors.css">
<link rel="stylesheet" href="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/tokens/typography.css">
<link rel="stylesheet" href="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/tokens/spacing.css">
<link rel="stylesheet" href="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/tokens/effects.css">
<link rel="stylesheet" href="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/styles.css">
<script src="_ds/spotlightsearch-io-design-system-957fb6fd-afa8-4737-be47-50418205527f/_ds_bundle.js"></script>
<style>
  html,body{margin:0;padding:0;background:#0C0E10}
  *{box-sizing:border-box}
  a{color:#2FE0C4;text-decoration:none}
  a:hover{color:#7CE9D8}
  ::-webkit-scrollbar{width:10px;height:10px}
  ::-webkit-scrollbar-thumb{background:#23282C;border-radius:99px}
  ::-webkit-scrollbar-track{background:transparent}
</style>
</helmet>

<div style="display:flex;min-height:100vh;background:#0C0E10;color:#EAF0F0;font-family:var(--font-body);font-size:14.5px">

  <aside style="width:250px;flex:none;height:100vh;position:sticky;top:0;display:flex;flex-direction:column;background:#0C0E10;border-right:1px solid #1B1F22">
    <sc-if value="{{ isVenue }}" hint-placeholder-val="{{ true }}">
      <div style="padding:22px 22px 18px">
        <div style="font-family:var(--font-display);font-weight:800;font-size:11px;letter-spacing:.26em;color:#8A939A;line-height:1">THE RAINBOW</div>
        <div style="margin-top:5px;font-family:var(--font-display);font-weight:800;font-size:27px;letter-spacing:.02em;line-height:1"><span style="color:#E8705A">C</span><span style="color:#E3B85F">A</span><span style="color:#F2D06B">C</span><span style="color:#2FE0C4">T</span><span style="color:#7CC2B7">U</span><span style="color:#9BA8E8">S</span></div>
        <div style="margin-top:7px;font:500 8.5px/1 var(--font-mono);letter-spacing:.24em;text-transform:uppercase;color:#5B646B">Virginia Beach</div>
      </div>
    </sc-if>
    <sc-if value="{{ isPerformer }}">
      <div style="padding:22px 22px 18px">
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Logo" variant="inline" size="{{ 38 }}" theme="dark" hint-size="auto,22px"></x-import>
        <div style="margin-top:9px;font:500 8.5px/1.5 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Artist Account<br>Kamilla Belladonna</div>
      </div>
    </sc-if>

    <nav style="flex:1;overflow-y:auto;padding:4px 12px 20px;display:flex;flex-direction:column;gap:14px">

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Proposal</div>
        <button onClick="{{ go.cover }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.cover.bg }};color:{{ nv.cover.fg }}">Overview</button>
        <button onClick="{{ go.problem }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.problem.bg }};color:{{ nv.problem.fg }}">The Problem</button>
        <button onClick="{{ go.platform }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.platform.bg }};color:{{ nv.platform.fg }}">The Platform</button>
        <button onClick="{{ go.integrations }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.integrations.bg }};color:{{ nv.integrations.fg }}">Integrations</button>
        <button onClick="{{ go.migration }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.migration.bg }};color:{{ nv.migration.fg }}">Migration &amp; Terms</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Owner</div>
        <button onClick="{{ go.command }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.command.bg }};color:{{ nv.command.fg }}">Command Center</button>
        <button onClick="{{ go.financials }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.financials.bg }};color:{{ nv.financials.fg }}">Financials</button>
        <button onClick="{{ go.payroll }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.payroll.bg }};color:{{ nv.payroll.fg }}">Payroll Runs</button>
        <button onClick="{{ go.analytics }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.analytics.bg }};color:{{ nv.analytics.fg }}">Venue Analytics</button>
        <button onClick="{{ go.compliance }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.compliance.bg }};color:{{ nv.compliance.fg }}">Compliance Vault</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Manager</div>
        <button onClick="{{ go.tonight }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.tonight.bg }};color:{{ nv.tonight.fg }}">Tonight · Run of Show</button>
        <button onClick="{{ go.booking }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.booking.bg }};color:{{ nv.booking.fg }}">Booking Calendar</button>
        <button onClick="{{ go.scheduling }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.scheduling.bg }};color:{{ nv.scheduling.fg }}">Scheduling &amp; Shifts</button>
        <button onClick="{{ go.boxoffice }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.boxoffice.bg }};color:{{ nv.boxoffice.fg }}">Box Office</button>
        <button onClick="{{ go.bar }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.bar.bg }};color:{{ nv.bar.fg }}">Bar, Kitchen &amp; POS</button>
        <button onClick="{{ go.inventory }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.inventory.bg }};color:{{ nv.inventory.fg }}">Inventory</button>
        <button onClick="{{ go.workorders }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.workorders.bg }};color:{{ nv.workorders.fg }}">Work Orders</button>
        <button onClick="{{ go.cases }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.cases.bg }};color:{{ nv.cases.fg }}">HR Cases</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Employee</div>
        <button onClick="{{ go.myshift }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.myshift.bg }};color:{{ nv.myshift.fg }}">My Shift</button>
        <button onClick="{{ go.timeclock }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.timeclock.bg }};color:{{ nv.timeclock.fg }}">Clock &amp; Checklists</button>
        <button onClick="{{ go.swaps }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.swaps.bg }};color:{{ nv.swaps.fg }}">Swaps &amp; Availability</button>
        <button onClick="{{ go.report }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.report.bg }};color:{{ nv.report.fg }}">Report an Issue</button>
        <button onClick="{{ go.mypay }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.mypay.bg }};color:{{ nv.mypay.fg }}">My Pay &amp; Tips</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Performer · Artist Account</div>
        <button onClick="{{ go.bookings }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.bookings.bg }};color:{{ nv.bookings.fg }}">My Bookings</button>
        <button onClick="{{ go.opencalls }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.opencalls.bg }};color:{{ nv.opencalls.fg }}">Open Calls</button>
        <button onClick="{{ go.venueportal }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.venueportal.bg }};color:{{ nv.venueportal.fg }}">Venue Portal · Cactus</button>
        <button onClick="{{ go.contracts }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.contracts.bg }};color:{{ nv.contracts.fg }}">Contracts</button>
        <button onClick="{{ go.settlements }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.settlements.bg }};color:{{ nv.settlements.fg }}">Settlements</button>
        <button onClick="{{ go.rider }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.rider.bg }};color:{{ nv.rider.fg }}">Rider &amp; Media Kit</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Guest &amp; Vendor</div>
        <button onClick="{{ go.listing }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.listing.bg }};color:{{ nv.listing.fg }}">Event Listing</button>
        <button onClick="{{ go.checkout }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.checkout.bg }};color:{{ nv.checkout.fg }}">Checkout</button>
        <button onClick="{{ go.ticket }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.ticket.bg }};color:{{ nv.ticket.fg }}">Digital Ticket</button>
        <button onClick="{{ go.purchasing }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.purchasing.bg }};color:{{ nv.purchasing.fg }}">Vendor Orders</button>
        <button onClick="{{ go.receiving }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.receiving.bg }};color:{{ nv.receiving.fg }}">Receiving</button>
      </div>

      <div style="display:flex;flex-direction:column;gap:2px">
        <div style="padding:6px 10px 8px;font:500 9px/1 var(--font-mono);letter-spacing:.22em;text-transform:uppercase;color:#4A5257">Platform</div>
        <button onClick="{{ go.door }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.door.bg }};color:{{ nv.door.fg }}">Door &amp; Access</button>
        <button onClick="{{ go.admin }}" style="all:unset;cursor:pointer;padding:9px 12px;border-radius:8px;font-size:13.5px;transition:background 160ms,color 160ms;background:{{ nv.admin.bg }};color:{{ nv.admin.fg }}">Admin &amp; Roles</button>
      </div>
    </nav>

    <div style="padding:14px 22px 18px;border-top:1px solid #1B1F22;display:flex;align-items:center;gap:10px">
      <span style="width:26px;height:26px;border-radius:50%;border:1px solid #4A3C1E;display:inline-flex;align-items:center;justify-content:center;flex:none">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#C79A45" stroke-width="2"><circle cx="12" cy="12" r="3"/><ellipse cx="12" cy="12" rx="10" ry="4.5" transform="rotate(-30 12 12)"/></svg>
      </span>
      <span style="font-size:13px;color:#C79A45">Hedy AI</span>
      <span style="margin-left:auto;font:500 8px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">ON</span>
    </div>
    <div style="padding:0 22px 18px;display:flex;align-items:center;gap:7px">
      <span style="font:500 8px/1.4 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#3A4046">Powered by</span>
      <span style="font-family:var(--font-display);font-weight:800;font-size:10px;letter-spacing:-.01em;line-height:1"><span style="color:#5B646B">Spotlight</span><span style="color:#2F8A80">Search</span><span style="color:#3A4046">.io</span></span>
    </div>
  </aside>

  <main id="ss-main" style="flex:1;min-width:0;height:100vh;overflow-y:auto">

    <sc-if value="{{ pg.cover }}" hint-placeholder-val="{{ true }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <h1 style="margin:0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Proposal</h1>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,34px">Download PDF</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,34px">Approve Pilot</x-import>
        </div>
      </header>

      <div style="padding:52px 40px 72px;background:radial-gradient(120% 90% at 50% -20%,rgba(6,229,199,.10) 0%,transparent 55%)">
        <div style="max-width:1180px;margin:0 auto">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tone="signal" theme="dark" hint-size="auto,12px">Prepared for The Rainbow Cactus · Virginia Beach, VA · August 2026</x-import>
          <h2 style="margin:22px 0 0;font:800 66px/.98 var(--font-display);letter-spacing:-.02em;color:#EAF0F0;max-width:17ch;text-wrap:balance">One Operating System For The Cactus.</h2>
          <p style="margin:22px 0 0;max-width:64ch;font:400 19px/1.5 var(--font-body);color:#8A939A">SpotlightSearch.io becomes the event manager for 475 S. Lynnhaven Road — replacing the ticketing platform and the point of sale with one system that carries the owner, the managers, every bartender and door host on shift, and every queen on the bill.</p>

          <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:18px;margin-top:44px">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Nights Programmed</x-import></div>
              <div style="margin-top:12px;font:500 40px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">7</div>
              <div style="margin-top:8px;font-size:13px;line-height:1.5;color:#5B646B">What It Do?! · Pool Tournament · Drag Karaoke · Saturday Drag · Men Next Door · viewing parties · guest bookings</div>
            </div>
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">People On System</x-import></div>
              <div style="margin-top:12px;font:500 40px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">22</div>
              <div style="margin-top:8px;font-size:13px;line-height:1.5;color:#5B646B">8 bartenders · 4 security · kitchen · 5 resident cast · DJ · managers</div>
            </div>
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Platforms Retired</x-import></div>
              <div style="margin-top:12px;font:500 40px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">2</div>
              <div style="margin-top:8px;font-size:13px;line-height:1.5;color:#5B646B">Third-party ticketing and the current point of sale, consolidated</div>
            </div>
            <div style="background:#15181B;border:1px solid #4A3C1E;border-radius:16px;padding:24px;box-shadow:0 0 24px rgba(199,154,69,.10)">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Fees Recovered / Yr</x-import></div>
              <div style="margin-top:12px;font:500 40px/1 var(--font-mono);letter-spacing:-.02em;color:#E3B85F">$61,400</div>
              <div style="margin-top:8px;font-size:13px;line-height:1.5;color:#5B646B">Estimate — per-ticket fees, card fees, duplicate subscriptions</div>
            </div>
          </div>

          <div style="display:grid;grid-template-columns:1.1fr .9fr;gap:20px;margin-top:20px">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:32px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">What This Proposal Covers</x-import></div>
              <div style="display:grid;gap:16px;margin-top:20px">
                <div style="display:flex;gap:14px;align-items:flex-start"><span style="width:22px;flex:none;font:500 11px/1.5 var(--font-mono);color:#2FE0C4">01</span><div><div style="font-weight:600">Four portals, one record</div><div style="font-size:13.5px;color:#8A939A;line-height:1.6">Owner, manager, employee and performer views over the same night — plus a public ticket page and a vendor desk.</div></div></div>
                <div style="display:flex;gap:14px;align-items:flex-start"><span style="width:22px;flex:none;font:500 11px/1.5 var(--font-mono);color:#2FE0C4">02</span><div><div style="font-weight:600">Nightly operations, not monthly reports</div><div style="font-size:13.5px;color:#8A939A;line-height:1.6">Prep and teardown check-offs, run of show, door counts and bar sales settled before the lights come up at 2 AM.</div></div></div>
                <div style="display:flex;gap:14px;align-items:flex-start"><span style="width:22px;flex:none;font:500 11px/1.5 var(--font-mono);color:#2FE0C4">03</span><div><div style="font-weight:600">A real escalation path for staff</div><div style="font-size:13.5px;color:#8A939A;line-height:1.6">Maintenance work orders, interpersonal reports and harassment complaints — named, confidential or anonymous, the reporter chooses per report.</div></div></div>
                <div style="display:flex;gap:14px;align-items:flex-start"><span style="width:22px;flex:none;font:500 11px/1.5 var(--font-mono);color:#2FE0C4">04</span><div><div style="font-weight:600">Payroll and settlements in one ledger</div><div style="font-size:13.5px;color:#8A939A;line-height:1.6">Clock-ins, tip pools, entertainer settlements and signed agreements reach QuickBooks without anyone re-keying a number.</div></div></div>
              </div>
            </div>
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:32px;display:flex;flex-direction:column">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Signature</x-import></div>
              <p style="margin:22px 0 0;font:800 30px/1.12 var(--font-display);letter-spacing:-.01em;color:#EAF0F0">Always in the know.<br><span style="color:#2FE0C4">Never the last to know.</span></p>
              <p style="margin:20px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Virginia Beach's home for the LGBTQ+ community since 1997 runs seven nights a week on three disconnected systems. This proposal replaces them with a console the owner can read at close.</p>
              <div style="margin-top:auto;padding-top:24px;display:flex;gap:10px;flex-wrap:wrap">
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" onClick="{{ go.problem }}" hint-size="auto,34px">Read the case</x-import>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" onClick="{{ go.command }}" hint-size="auto,34px">Open the product</x-import>
              </div>
            </div>
          </div>

          <div style="margin-top:20px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px 32px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">The Week, As It Stands</x-import></div>
            <div style="display:grid;grid-template-columns:repeat(7,1fr);gap:12px;margin-top:20px">
              <div style="border-top:2px solid #23282C;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">MON</div><div style="margin-top:10px;font-size:13px;color:#5B646B">Closed</div></div>
              <div style="border-top:2px solid #23282C;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">TUE</div><div style="margin-top:10px;font-size:13px;color:#5B646B">Game night</div></div>
              <div style="border-top:2px solid #2FE0C4;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">WED</div><div style="margin-top:10px;font-size:13px;color:#EAF0F0">What It Do?!<br><span style="color:#5B646B">10:30 PM</span></div></div>
              <div style="border-top:2px solid #2FE0C4;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">THU</div><div style="margin-top:10px;font-size:13px;color:#EAF0F0">Pool Tournament<br><span style="color:#5B646B">8 PM · free to play</span></div></div>
              <div style="border-top:2px solid #2FE0C4;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">FRI</div><div style="margin-top:10px;font-size:13px;color:#EAF0F0">All Stars 8 PM<br>Drag Karaoke 9 PM</div></div>
              <div style="border-top:2px solid #2FE0C4;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">SAT</div><div style="margin-top:10px;font-size:13px;color:#EAF0F0">Saturday Drag Show<br><span style="color:#5B646B">doors 7 · show 10:30</span></div></div>
              <div style="border-top:2px solid #2FE0C4;padding-top:14px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">SUN</div><div style="margin-top:10px;font-size:13px;color:#EAF0F0">Men Next Door<br><span style="color:#5B646B">Uncovered</span></div></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.problem }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <h1 style="margin:0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">The Problem</h1>
        <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Current State · August 2026</x-import></div>
      </header>
      <div style="padding:44px 40px 80px;max-width:1180px;margin:0 auto">
        <h2 style="margin:0;font:800 44px/1.04 var(--font-display);letter-spacing:-.015em;color:#EAF0F0;max-width:20ch">Three Systems, One Room, No Shared Truth.</h2>
        <p style="margin:18px 0 0;max-width:66ch;font:400 17px/1.6 var(--font-body);color:#8A939A">Ticketing, point of sale and labour each hold a piece of the night. Nothing reconciles until someone exports all three and joins them by hand the next afternoon.</p>

        <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:36px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="critical" dot="{{ false }}" hint-size="auto,20px">Ticketing</x-import>
            <div style="margin-top:16px;font-weight:600;font-size:16px">Door revenue lives on someone else's platform</div>
            <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">A guest ticket that lists at $15 arrives as $17.85 at checkout, and the venue never owns the buyer. Guest bookings routed through an outside promoter keep the attendee list with the promoter.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="critical" dot="{{ false }}" hint-size="auto,20px">Point of Sale</x-import>
            <div style="margin-top:16px;font-weight:600;font-size:16px">Bar and kitchen never meet the bill</div>
            <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Nobody can say whether Thursday pool night out-earns a Saturday drag show per head, because cover, bar tabs and loaded fries are counted in different logins.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="caution" dot="{{ false }}" hint-size="auto,20px">Labour</x-import>
            <div style="margin-top:16px;font-weight:600;font-size:16px">Shifts, tips and entertainer pay are a spreadsheet</div>
            <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Eight bartenders on rotation, four security, prep and teardown hours and the tip-out to the cast are reconstructed weekly from memory and group texts.</p>
          </div>
        </div>

        <div style="margin-top:20px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Where the night breaks</div>
          <div style="display:grid;grid-template-columns:1.3fr 1.1fr 1.1fr .7fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Moment</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Today</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">With SpotlightSearch</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Lag Removed</div>

            <div style="padding:16px 26px;border-top:1px solid #23282C">Doors at 7</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#8A939A">Scan app on a phone, cover counted separately</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#EAF0F0">Live head count against occupancy</div>
            <div style="padding:16px 26px;border-top:1px solid #23282C;color:#2FE0C4;font-family:var(--font-mono);font-size:12.5px">~40 min</div>

            <div style="padding:16px 26px;border-top:1px solid #23282C">Cast settles after last number</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#8A939A">Cash from the drawer, note in a book</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#EAF0F0">Settlement sheet signed on the spot</div>
            <div style="padding:16px 26px;border-top:1px solid #23282C;color:#2FE0C4;font-family:var(--font-mono);font-size:12.5px">2 days</div>

            <div style="padding:16px 26px;border-top:1px solid #23282C">Something breaks mid-show</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#8A939A">Text to a manager, lost by Monday</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#EAF0F0">Work order with owner, photo and SLA</div>
            <div style="padding:16px 26px;border-top:1px solid #23282C;color:#2FE0C4;font-family:var(--font-mono);font-size:12.5px">Indefinite</div>

            <div style="padding:16px 26px;border-top:1px solid #23282C">Payroll close</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#8A939A">Three exports joined by hand</div>
            <div style="padding:16px;border-top:1px solid #23282C;color:#EAF0F0">Approved hours post to QuickBooks</div>
            <div style="padding:16px 26px;border-top:1px solid #23282C;color:#2FE0C4;font-family:var(--font-mono);font-size:12.5px">~6 hrs/period</div>
          </div>
        </div>

        <div style="margin-top:20px;background:#15181B;border:1px solid #23282C;border-left:3px solid #E8705A;border-radius:16px;padding:26px 30px">
          <div style="font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#E8705A">Unaddressed Risk</div>
          <div style="margin-top:12px;font-weight:600;font-size:17px">There is no channel for a complaint the manager on duty should not see first.</div>
          <p style="margin:10px 0 0;max-width:78ch;font-size:13.5px;line-height:1.7;color:#8A939A">Harassment and interpersonal conflict currently escalate through the same person they may involve. A room that has been a safe space since 1997 deserves a reporting surface built to the same standard as the door policy.</p>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.platform }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <h1 style="margin:0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">The Platform</h1>
        <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">12 Modules · 4 Portals</x-import></div>
      </header>
      <div style="padding:44px 40px 80px;max-width:1180px;margin:0 auto">
        <h2 style="margin:0;font:800 44px/1.04 var(--font-display);letter-spacing:-.015em;color:#EAF0F0;max-width:22ch">Every Role Sees The Same Night, Cut To Their Job.</h2>

        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:18px;margin-top:34px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Owner</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Nightly margin, labour percentage, payroll approvals, ABC and compliance documents. Read-only on operations, final say on money.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Manager</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Run of show, rota, box office, bar and kitchen, stock, work orders. Everything decided before doors at seven.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Employee</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Their shift, their check-offs, their clock, their tips — and a reporting channel that does not route through their manager.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Performer</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Bookings, signed agreements, tech rider, settlement history and payout status. No group chat required.</p>
          </div>
        </div>

        <div style="margin-top:32px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Module Map</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-top:18px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Ticketing &amp; Box Office</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Tiers, presales, comps, guest list, door scan, live capacity, 21+ ID prompt.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Bar, Kitchen &amp; POS</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Tabs, rounds, food fires, comps, voids, per-bartender sales and tip capture.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Scheduling &amp; Shifts</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Rotating bar rota, security coverage, prep and teardown blocks, swaps.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Payroll &amp; Time Clock</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">On-site clock-in, break rules, tip pool, approval, QuickBooks post.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Booking Calendar</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Resident nights, guest queens, promoter co-productions, private hire, holds.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Contracts &amp; Settlements</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Guarantee or door split, rider terms, DocuSign, same-night payout.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Inventory &amp; Purchasing</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Par levels, weekly count, pour cost, purchase orders, receiving.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Work Orders</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Maintenance tickets with severity, owner, SLA clock and photo evidence.</div></div>
          <div style="background:#15181B;border:1px solid rgba(6,229,199,.28);border-radius:14px;padding:20px;box-shadow:0 0 30px rgba(6,229,199,.08)"><div style="font-weight:600;font-size:14.5px">HR Cases &amp; Reporting</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Named, confidential or anonymous. Harassment routes past the line manager.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Marketing &amp; CRM</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Event pages, weekly flyer schedule, repeat attendance, announcements.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Analytics</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Per-night margin, spend per head, labour percentage, format comparison.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:14px;padding:20px"><div style="font-weight:600;font-size:14.5px">Door &amp; Access Control</div><div style="margin-top:8px;font-size:13px;line-height:1.6;color:#8A939A">Scanner devices, staff badges, back-of-house access, incident log.</div></div>
        </div>

        <div style="margin-top:26px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Routine Ops</x-import></div>
          <div style="margin-top:14px;font:800 26px/1.1 var(--font-display);letter-spacing:-.01em">Every Night Runs The Same Four Blocks.</div>
          <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-top:22px">
            <div style="border-left:2px solid #2FE0C4;padding-left:16px"><div style="font:500 10px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">16:00 · PREP</div><div style="margin-top:10px;font-size:13.5px;color:#8A939A;line-height:1.6">Stock pull, ice, glassware, kitchen line check, stage and light check, till float.</div></div>
            <div style="border-left:2px solid #2FE0C4;padding-left:16px"><div style="font:500 10px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">19:00 · DOORS</div><div style="margin-top:10px;font-size:13.5px;color:#8A939A;line-height:1.6">Scanner online, security posted, ID checks, guest list loaded, head count live.</div></div>
            <div style="border-left:2px solid #2FE0C4;padding-left:16px"><div style="font:500 10px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">22:30 · SHOW</div><div style="margin-top:10px;font-size:13.5px;color:#8A939A;line-height:1.6">Run of show, set order, tip round calls, incident log open, last call timing.</div></div>
            <div style="border-left:2px solid #2FE0C4;padding-left:16px"><div style="font:500 10px/1 var(--font-mono);letter-spacing:.16em;color:#2FE0C4">02:00 · TEARDOWN</div><div style="margin-top:10px;font-size:13.5px;color:#8A939A;line-height:1.6">Cash drop, cast settlements signed, closing check-off, work orders raised.</div></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.integrations }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <h1 style="margin:0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Integrations</h1>
        <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">3 Live · 1 On Roadmap</x-import></div>
      </header>
      <div style="padding:44px 40px 80px;max-width:1180px;margin:0 auto">
        <h2 style="margin:0;font:800 44px/1.04 var(--font-display);letter-spacing:-.015em;color:#EAF0F0;max-width:20ch">Connected Where It Matters. Nowhere Else.</h2>
        <p style="margin:18px 0 0;max-width:64ch;font:400 17px/1.6 var(--font-body);color:#8A939A">The Cactus keeps its accountant, its calendar and its signing workflow. Everything operational moves in-house.</p>

        <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:34px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
              <div style="font-weight:700;font-size:18px">QuickBooks</div>
              <span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase"><span style="width:5px;height:5px;border-radius:50%;background:currentColor"></span>Connected</span>
            </div>
            <p style="margin:14px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Approved payroll runs, cast settlements, supplier invoices and nightly sales summaries post as journal entries. No CSV.</p>
            <div style="margin-top:18px;display:flex;flex-direction:column;gap:8px;font:500 10.5px/1 var(--font-mono);letter-spacing:.1em;color:#5B646B">
              <span>SALES JOURNAL · NIGHTLY</span><span>SETTLEMENTS · ON SIGN</span><span>AP INVOICES · ON RECEIPT</span>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
              <div style="font-weight:700;font-size:18px">DocuSign</div>
              <span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase"><span style="width:5px;height:5px;border-radius:50%;background:currentColor"></span>Connected</span>
            </div>
            <p style="margin:14px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Entertainer agreements, W-9s, private hire contracts and policy acknowledgements are issued from the booking record and filed back against it.</p>
            <div style="margin-top:18px;display:flex;flex-direction:column;gap:8px;font:500 10.5px/1 var(--font-mono);letter-spacing:.1em;color:#5B646B">
              <span>PERFORMER AGREEMENT</span><span>W-9 · ANNUAL</span><span>HANDBOOK ACKNOWLEDGEMENT</span>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
              <div style="font-weight:700;font-size:18px">Google Calendar</div>
              <span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase"><span style="width:5px;height:5px;border-radius:50%;background:currentColor"></span>Connected</span>
            </div>
            <p style="margin:14px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Confirmed bookings, call times and shift assignments sync two-way to staff and cast calendars. Holds stay private until confirmed.</p>
            <div style="margin-top:18px;display:flex;flex-direction:column;gap:8px;font:500 10.5px/1 var(--font-mono);letter-spacing:.1em;color:#5B646B">
              <span>CALL TIMES · TWO-WAY</span><span>SHIFTS · PUSH</span><span>HOLDS · PRIVATE</span>
            </div>
          </div>
        </div>

        <div style="margin-top:20px;background:#15181B;border:1px solid #4A3C1E;border-radius:16px;padding:32px;box-shadow:0 0 30px rgba(199,154,69,.08)">
          <div style="display:flex;align-items:flex-start;justify-content:space-between;gap:24px">
            <div style="max-width:66ch">
              <div style="display:flex;align-items:center;gap:12px">
                <div style="font-weight:700;font-size:20px;color:#EAF0F0">SpotlightSearch Terminal</div>
                <span style="display:inline-flex;padding:4px 10px;border-radius:999px;border:1px solid rgba(199,154,69,.55);color:#E3B85F;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Coming Soon</span>
              </div>
              <p style="margin:14px 0 0;font-size:14px;line-height:1.7;color:#8A939A">Our own card terminal, built for the bar rail and the door — tap, tip prompt and ticket scan on one device, settling straight into the same ledger. Until it ships, the platform runs on third-party terminals, so nothing about this proposal waits on hardware.</p>
            </div>
            <div style="display:grid;gap:10px;min-width:230px">
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13px"><span style="color:#8A939A">Third-party terminals</span><span style="color:#2FE0C4;font-family:var(--font-mono);font-size:11.5px">SUPPORTED</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13px"><span style="color:#8A939A">Cactus Terminal pilot</span><span style="color:#E3B85F;font-family:var(--font-mono);font-size:11.5px">Q2 2027</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13px"><span style="color:#8A939A">Rate at launch</span><span style="color:#E3B85F;font-family:var(--font-mono);font-size:11.5px">TBC</span></div>
            </div>
          </div>
        </div>

        <div style="margin-top:20px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Explicitly Not Integrated</x-import></div>
          <p style="margin:12px 0 0;max-width:78ch;font-size:13.5px;line-height:1.7;color:#8A939A">The incumbent ticketing platform and point of sale are replaced, not connected. Historical sales and attendee records are imported once during migration and then retired — the venue owns the guest list from cutover onward.</p>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.migration }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <h1 style="margin:0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Migration &amp; Terms</h1>
        <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Cutover Without A Dark Night</x-import></div>
      </header>
      <div style="padding:44px 40px 80px;max-width:1180px;margin:0 auto">
        <h2 style="margin:0;font:800 44px/1.04 var(--font-display);letter-spacing:-.015em;color:#EAF0F0;max-width:20ch">Six Weeks. No Night Goes Dark.</h2>

        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-top:34px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;color:#2FE0C4">WEEK 1–2 · SET UP</div>
            <div style="margin-top:12px;font-weight:600">Load the venue</div>
            <p style="margin:8px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Floor plan, occupancy, bar and kitchen menus, staff roster, resident cast, pay rates, vendor list. Historical ticket and sales data imported.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;color:#2FE0C4">WEEK 3 · PARALLEL</div>
            <div style="margin-top:12px;font-weight:600">Run both, sell on one</div>
            <p style="margin:8px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Scheduling, clock-in and work orders go live. Ticketing stays on the incumbent while the team learns the console.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;color:#2FE0C4">WEEK 4 · CUTOVER</div>
            <div style="margin-top:12px;font-weight:600">Sell the first show</div>
            <p style="margin:8px 0 0;font-size:13px;line-height:1.65;color:#8A939A">A Wednesday is chosen as the first ticketed night on SpotlightSearch. Door scan, bar and settlement all run in-platform.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;color:#2FE0C4">WEEK 5–6 · CLOSE</div>
            <div style="margin-top:12px;font-weight:600">Retire the old stack</div>
            <p style="margin:8px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Saturday drag and guest bookings migrate, payroll runs end-to-end, incumbent contracts are cancelled.</p>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-top:20px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Commercials</x-import></div>
            <div style="margin-top:20px;display:grid;gap:0">
              <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Platform licence</span><span style="font-family:var(--font-mono);color:#E3B85F">$0 · pilot term</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Per ticket sold</span><span style="font-family:var(--font-mono);color:#E3B85F">$0.79 + 2.4%</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Card processing</span><span style="font-family:var(--font-mono);color:#E3B85F">Pass-through</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Staff seats</span><span style="font-family:var(--font-mono);color:#E3B85F">Unlimited</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px 0"><span style="color:#8A939A">Migration &amp; training</span><span style="font-family:var(--font-mono);color:#E3B85F">Included</span></div>
            </div>
            <p style="margin:18px 0 0;font-size:12.5px;line-height:1.6;color:#5B646B">Figures are indicative and subject to a signed pilot agreement. No termination fee during the pilot term.</p>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px;display:flex;flex-direction:column">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">What We Need From The Cactus</x-import></div>
            <div style="margin-top:20px;display:grid;gap:14px;font-size:13.5px;line-height:1.65;color:#8A939A">
              <div style="display:flex;gap:12px"><span style="color:#2FE0C4">✓</span><span>One named operational owner — a manager who can approve the rota and the run of show.</span></div>
              <div style="display:flex;gap:12px"><span style="color:#2FE0C4">✓</span><span>Current staff roster with pay rates, and the resident cast agreements as they stand.</span></div>
              <div style="display:flex;gap:12px"><span style="color:#2FE0C4">✓</span><span>Read access to the existing ticketing and POS exports for the last twelve months.</span></div>
              <div style="display:flex;gap:12px"><span style="color:#2FE0C4">✓</span><span>Two hours of floor time before doors on three consecutive Wednesdays for training.</span></div>
              <div style="display:flex;gap:12px"><span style="color:#2FE0C4">✓</span><span>A decision on who receives anonymous harassment reports, and who does not.</span></div>
            </div>
            <div style="margin-top:auto;padding-top:24px;border-top:1px solid #23282C;font-size:12.5px;line-height:1.7;color:#5B646B">
              The Rainbow Cactus · 475 S. Lynnhaven Rd, Virginia Beach, VA 23452 · (757) 368-0441 · contactus@TheRainbowCactus.Gay
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.command }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Owner · The Rainbow Cactus</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Command Center</h1>
        </div>
        <div style="display:flex;align-items:center;gap:16px">
          <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Sat 22 Aug · 23:41 EDT</span>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" hint-size="auto,20px">Doors Open</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px;display:flex;align-items:center;justify-content:space-between;gap:32px;flex-wrap:wrap">
          <div>
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Tonight</x-import></div>
            <div style="margin-top:12px;font:800 28px/1.05 var(--font-display);letter-spacing:-.01em">Saturday Night Drag Show</div>
            <div style="margin-top:10px;font-size:13.5px;color:#8A939A">Kamilla Belladonna · Chanel Clitopatra · Jasmine Saville · music by DJ Airrick</div>
          </div>
          <div style="display:flex;gap:36px;align-items:center">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Gauge" value="{{ 78 }}" size="{{ 104 }}" thickness="{{ 7 }}" label="Occupancy" sublabel="of 240" tone="signal" hint-size="104px,140px"></x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Gauge" value="{{ 31 }}" size="{{ 104 }}" thickness="{{ 7 }}" label="Labour" sublabel="of sales" tone="healthy" hint-size="104px,140px"></x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Gauge" value="{{ 64 }}" size="{{ 104 }}" thickness="{{ 7 }}" label="Bar Pace" sublabel="vs avg" tone="caution" hint-size="104px,140px"></x-import>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Door Revenue</x-import></div>
            <div style="margin-top:12px;font:500 34px/1 var(--font-mono);letter-spacing:-.02em;color:#E3B85F">$3,180</div>
            <div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#2FE0C4">▴ 12% vs last Saturday</div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Bar &amp; Kitchen</x-import></div>
            <div style="margin-top:12px;font:500 34px/1 var(--font-mono);letter-spacing:-.02em;color:#E3B85F">$7,942</div>
            <div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#2FE0C4">▴ 6% vs last Saturday</div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Spend Per Head</x-import></div>
            <div style="margin-top:12px;font:500 34px/1 var(--font-mono);letter-spacing:-.02em;color:#E3B85F">$42.40</div>
            <div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#8A939A">187 guests in the room</div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Projected Margin</x-import></div>
            <div style="margin-top:12px;font:500 34px/1 var(--font-mono);letter-spacing:-.02em;color:#E3B85F">$4,610</div>
            <div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#8A939A">after labour, cast and cost of goods</div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-left:3px solid #E3B85F;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Active System Signal</x-import></div>
            <div style="margin-top:12px;font-weight:700;font-size:17px">Bar three is running the room alone</div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A"><span style="color:#EAF0F0;font-weight:600">Problem:</span> Head count passed 180 at 22:50 with two bartenders on the floor. Average ticket time on bar three is 4m 20s against a 2m target.</p>
            <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A"><span style="color:#EAF0F0;font-weight:600">Predicted outcome:</span> Roughly $700 of bar revenue lost between now and last call if service time holds.</p>
            <div style="display:flex;gap:10px;margin-top:18px">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Ignore</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Call In Cover</x-import>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Live Feed</x-import></div>
            <div style="margin-top:18px;display:grid;gap:14px">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.FeedItem" status="healthy" time="23:38" theme="dark" hint-size="100%,42px">Second set called — Chanel Clitopatra on stage</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.FeedItem" status="caution" time="23:12" theme="dark" hint-size="100%,42px">Work order raised — ice machine, back bar</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.FeedItem" status="healthy" time="22:50" theme="dark" hint-size="100%,42px">Head count 180 — 60 under occupancy</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.FeedItem" status="neutral" time="19:02" theme="dark" hint-size="100%,42px">Doors opened — 4 security posted</x-import>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Needs Your Signature</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="font-size:13.5px">Payroll — period ending 23 Aug</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">$14,208</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="font-size:13.5px">Guest booking — 12 Sep</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">$1,800</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="font-size:13.5px">Liquor purchase order #2214</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">$3,940</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;padding:14px;background:#0F1214;border:1px solid rgba(232,112,90,.3);border-radius:10px"><span style="font-size:13.5px">HR case CS-0042 — escalated</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E8705A">REVIEW</span></div>
            </div>
            <div style="margin-top:18px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" hint-size="100%,32px">Open Approvals Queue</x-import></div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;display:flex;align-items:center;justify-content:space-between">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">This Week By Night</x-import></div>
            <span style="font:500 10px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">17 – 23 August</span>
          </div>
          <div style="display:grid;grid-template-columns:1.3fr .8fr .7fr .7fr .7fr .7fr .8fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Night</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Format</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Heads</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Door</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Bar</div>
            <div style="padding:12px 16px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Labour</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Margin</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C">Wed 19</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;color:#8A939A">What It Do?!</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">96</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$480</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$2,910</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">34%</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$1,240</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C">Thu 20</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;color:#8A939A">Pool Tournament</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">71</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#8A939A">—</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$2,140</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">41%</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$610</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C">Fri 21</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;color:#8A939A">Pangina Heals · guest</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">238</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$4,247</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$9,860</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">28%</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$6,020</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;color:#2FE0C4">Sat 22 · live</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;color:#8A939A">Saturday Drag Show</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">187</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$3,180</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$7,942</div>
            <div style="padding:15px 16px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">31%</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$4,610</div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.financials }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Owner</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Financials</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Export P&amp;L</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Sync QuickBooks</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Revenue · Aug MTD" value="$214,860" tone="money" delta="9.4% vs July" deltaDir="up" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Cost Of Goods" value="$52,190" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import><div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#8A939A">24.3% of revenue</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Labour" value="$68,420" tone="money" delta="31.8% of revenue" deltaDir="up" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Net · MTD" value="$41,700" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import><div style="margin-top:10px;font:500 11px/1 var(--font-mono);color:#2FE0C4">19.4% margin</div></div>
        </div>

        <div style="display:grid;grid-template-columns:1.4fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Revenue By Format · Last 30 Nights</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">PER NIGHT AVERAGE</span>
            </div>
            <div style="margin-top:26px;display:grid;gap:18px">
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Guest headliner bookings</span><span style="font-family:var(--font-mono);color:#E3B85F">$14,107</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Saturday Night Drag Show</span><span style="font-family:var(--font-mono);color:#E3B85F">$11,122</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:79%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Friday Drag Karaoke with Marc</span><span style="font-family:var(--font-mono);color:#E3B85F">$6,480</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:46%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Sunday · Men Next Door</span><span style="font-family:var(--font-mono);color:#E3B85F">$5,240</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:37%;height:100%;background:#7CC2B7"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Wednesday · What It Do?!</span><span style="font-family:var(--font-mono);color:#E3B85F">$3,390</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:24%;height:100%;background:#7CC2B7"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Thursday · Pool Tournament</span><span style="font-family:var(--font-mono);color:#E3B85F">$2,140</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:15%;height:100%;background:#2F8A80"></div></div></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Fees Retired At Cutover</x-import></div>
            <p style="margin:14px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Annualised on the last 30 nights of volume.</p>
            <div style="margin-top:20px;display:grid;gap:0">
              <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C;font-size:13.5px"><span style="color:#8A939A">Third-party ticket fees</span><span style="font-family:var(--font-mono);color:#E3B85F">$38,900</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C;font-size:13.5px"><span style="color:#8A939A">POS subscription &amp; add-ons</span><span style="font-family:var(--font-mono);color:#E3B85F">$11,640</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C;font-size:13.5px"><span style="color:#8A939A">Scheduling tool</span><span style="font-family:var(--font-mono);color:#E3B85F">$2,880</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C;font-size:13.5px"><span style="color:#8A939A">Card rate delta</span><span style="font-family:var(--font-mono);color:#E3B85F">$7,980</span></div>
              <div style="display:flex;justify-content:space-between;padding:16px 0;font-size:15px;font-weight:600"><span>Recovered per year</span><span style="font-family:var(--font-mono);color:#E3B85F">$61,400</span></div>
            </div>
            <div style="margin-top:14px;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:12.5px;line-height:1.6;color:#5B646B">Net of SpotlightSearch per-ticket pricing. Card processing is passed through at cost.</div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.payroll }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Owner · Period Ending 23 Aug 2026</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Payroll Run</h1>
        </div>
        <div style="display:flex;align-items:center;gap:10px">
          <span style="display:inline-flex;padding:5px 12px;border-radius:999px;border:1px solid rgba(227,184,95,.5);color:#E3B85F;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Awaiting Approval</span>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="money" size="sm" hint-size="auto,32px">Approve &amp; Post</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Gross Wages" value="$11,486" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Declared Tips" value="$2,722" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Hours" value="612.5" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Exceptions</x-import></div><div style="margin-top:12px;font:500 32px/1 var(--font-mono);color:#E8705A">3</div></div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Staff Lines</div>
          <div style="display:grid;grid-template-columns:1.4fr .9fr .6fr .6fr .7fr .7fr .9fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Name</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Role</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Hrs</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">OT</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Wages</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Tips</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Devon Marsh</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bartender</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">38.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$798</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$412</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">CLEAR</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Rosa Iglesias</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bartender</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">44.5</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">4.5</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$1,012</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$538</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">OT REVIEW</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Tyrell Banks</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Security lead</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">40.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$920</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">CLEAR</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Priya Raman</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Kitchen</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">36.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$756</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$96</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">CLEAR</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Micah Ortega</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Door host</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">27.5</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$550</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$88</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E8705A">MISSED CLOCK-OUT</div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Tip Pool Distribution</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Card tips are pooled nightly and split on the published rule. Cash tips to the cast are recorded but not pooled.</p>
            <div style="margin-top:20px;display:grid;gap:12px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Bar — 70%</span><span style="font-family:var(--font-mono);color:#E3B85F">$1,905</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Door &amp; security — 15%</span><span style="font-family:var(--font-mono);color:#E3B85F">$408</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Kitchen — 15%</span><span style="font-family:var(--font-mono);color:#E3B85F">$409</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Cast Settlements · Contractors</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Paid outside payroll against signed agreements. 1099 totals accrue automatically.</p>
            <div style="margin-top:20px;display:grid;gap:12px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Kamilla Belladonna</span><span style="font-family:var(--font-mono);color:#E3B85F">$650</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Chanel Clitopatra</span><span style="font-family:var(--font-mono);color:#E3B85F">$650</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>Jasmine Saville</span><span style="font-family:var(--font-mono);color:#E3B85F">$500</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span>DJ Airrick</span><span style="font-family:var(--font-mono);color:#E3B85F">$400</span></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.analytics }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Owner</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Venue Analytics</h1>
        </div>
        <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Rolling 90 Nights</x-import></div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:1.3fr 1fr;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Attendance By Night Of Week</x-import></div>
            <div style="margin-top:28px;display:flex;align-items:flex-end;gap:14px;height:200px">
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">—</span><div style="width:100%;height:4%;background:#23282C;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">MON</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">54</span><div style="width:100%;height:23%;background:#2F8A80;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">TUE</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">96</span><div style="width:100%;height:40%;background:#7CC2B7;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">WED</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">71</span><div style="width:100%;height:30%;background:#7CC2B7;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">THU</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">164</span><div style="width:100%;height:69%;background:#2FE0C4;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">FRI</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#EAF0F0">198</span><div style="width:100%;height:83%;background:#2FE0C4;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">SAT</span></div>
              <div style="flex:1;display:flex;flex-direction:column;align-items:center;gap:10px;height:100%;justify-content:flex-end"><span style="font:500 11px/1 var(--font-mono);color:#8A939A">122</span><div style="width:100%;height:51%;background:#7CC2B7;border-radius:6px 6px 0 0"></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">SUN</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Guest Base</x-import></div>
            <div style="margin-top:22px;display:grid;gap:18px">
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Returning within 30 days</span><span style="font-family:var(--font-mono);color:#2FE0C4">47%</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:47%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">First-time attendees</span><span style="font-family:var(--font-mono);color:#EAF0F0">31%</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:31%;height:100%;background:#7CC2B7"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Arrived for a guest headliner</span><span style="font-family:var(--font-mono);color:#EAF0F0">22%</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:22%;height:100%;background:#2F8A80"></div></div></div>
            </div>
            <div style="margin-top:24px;padding:18px;background:#0F1214;border:1px solid #4A3C1E;border-radius:12px">
              <div style="display:flex;align-items:center;gap:8px;font:500 10px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#C79A45">Hedy · Suggestion</div>
              <p style="margin:12px 0 0;font-size:13.5px;line-height:1.65;color:#8A939A">Guests who first attend a Wednesday return at nearly twice the rate of Saturday first-timers. A low-cover Wednesday promoted to the Saturday list is the cheapest retention lever available.</p>
            </div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Format Comparison</div>
          <div style="display:grid;grid-template-columns:1.4fr .8fr .8fr .8fr .8fr .8fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Format</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Avg Heads</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Spend / Head</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Labour</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Cast Cost</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Margin</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Saturday Night Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">198</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$41.10</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">31%</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$2,200</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#2FE0C4">41%</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Guest headliner booking</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">238</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$59.30</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">28%</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$4,500</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#2FE0C4">43%</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Drag Karaoke with Marc</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">164</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$39.50</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">33%</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$450</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#2FE0C4">44%</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Pool Tournament Thursday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">71</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$30.10</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E8705A">41%</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#5B646B">—</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">28%</div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.compliance }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Owner</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Compliance Vault</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Upload Document</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:1.3fr 1fr;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Licences &amp; Certificates</x-import></div>
            <div style="margin-top:20px;display:grid;gap:10px">
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">Virginia ABC mixed beverage licence</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">RENEWS 30 JUN 2027</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CURRENT</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">Certificate of occupancy — 240</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">CITY OF VIRGINIA BEACH</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CURRENT</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid rgba(227,184,95,.34);border-radius:10px"><div><div style="font-size:14px">Fire inspection</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">DUE IN 21 DAYS</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">ACTION</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">Health department permit</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">KITCHEN · RENEWS 12 MAR 2027</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CURRENT</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">General liability &amp; liquor liability</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">CERTIFICATE ON FILE</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CURRENT</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Staff Training &amp; Acknowledgements</x-import></div>
            <div style="margin-top:22px;display:grid;gap:18px">
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Responsible alcohol service</span><span style="font-family:var(--font-mono);color:#2FE0C4">12 / 12</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Anti-harassment policy signed</span><span style="font-family:var(--font-mono);color:#E3B85F">15 / 17</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:88%;height:100%;background:#E3B85F"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">De-escalation — security</span><span style="font-family:var(--font-mono);color:#2FE0C4">4 / 4</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Food handler certification</span><span style="font-family:var(--font-mono);color:#2FE0C4">3 / 3</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span style="color:#8A939A">Performer W-9 on file</span><span style="font-family:var(--font-mono);color:#2FE0C4">5 / 5</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.tonight }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Saturday 22 August</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Run of Show</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Print Call Sheet</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Advance Cue</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto;display:grid;grid-template-columns:1.5fr 1fr;gap:16px">
        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Cue Sheet</x-import></div>
              <span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase"><span style="width:5px;height:5px;border-radius:50%;background:currentColor"></span>Cue 6 Live</span>
            </div>
            <div style="margin-top:22px;display:grid;gap:0">
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center;opacity:.5"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">16:00</span><span style="font-size:14px">Prep block — bar, kitchen line, stage and lighting check</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">COMPLETE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center;opacity:.5"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">18:30</span><span style="font-size:14px">Cast call — hair and makeup, room 2</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">COMPLETE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center;opacity:.5"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">19:00</span><span style="font-size:14px">Doors — 4 security posted, ID check at entry</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">COMPLETE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center;opacity:.5"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">21:00</span><span style="font-size:14px">DJ Airrick opens the floor</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">COMPLETE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center;opacity:.5"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">22:30</span><span style="font-size:14px">Show call — Kamilla Belladonna opens, three numbers</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">COMPLETE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:16px 14px;border-radius:10px;background:rgba(6,229,199,.07);border:1px solid rgba(47,224,196,.28);align-items:center"><span style="font:500 12px/1 var(--font-mono);color:#2FE0C4">23:35</span><span style="font-size:14px;font-weight:600">Chanel Clitopatra — set two, tip round called</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">ON STAGE</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">00:10</span><span style="font-size:14px">Jasmine Saville — closing set</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">QUEUED</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;border-bottom:1px solid #23282C;align-items:center"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">01:30</span><span style="font-size:14px">Last call</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">QUEUED</span></div>
              <div style="display:grid;grid-template-columns:78px 1fr 130px;gap:16px;padding:14px 0;align-items:center"><span style="font:500 12px/1 var(--font-mono);color:#5B646B">02:00</span><span style="font-size:14px">Teardown — cash drop, settlements, closing check-off</span><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">QUEUED</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">On Shift Tonight</x-import></div>
            <div style="margin-top:20px;display:grid;grid-template-columns:repeat(3,1fr);gap:10px">
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Devon Marsh</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">BAR 1 · IN 18:42</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Rosa Iglesias</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">BAR 2 · IN 18:38</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid rgba(227,184,95,.34);border-radius:10px"><div style="font-size:13.5px">Bar 3</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">UNSTAFFED</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Tyrell Banks</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">SECURITY LEAD</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Micah Ortega</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">DOOR · SCANNER 1</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Priya Raman</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">KITCHEN · CLOSES 00:30</div></div>
            </div>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Door</x-import></div>
            <div style="margin-top:16px;display:flex;align-items:baseline;gap:10px"><span style="font:500 44px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">187</span><span style="font-size:14px;color:#5B646B">/ 240 capacity</span></div>
            <div style="margin-top:14px;height:8px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:78%;height:100%;background:#2FE0C4"></div></div>
            <div style="margin-top:18px;display:grid;gap:9px;font-size:13px">
              <div style="display:flex;justify-content:space-between"><span style="color:#8A939A">Advance tickets scanned</span><span style="font-family:var(--font-mono)">124</span></div>
              <div style="display:flex;justify-content:space-between"><span style="color:#8A939A">Walk-up cover</span><span style="font-family:var(--font-mono)">51</span></div>
              <div style="display:flex;justify-content:space-between"><span style="color:#8A939A">Guest list &amp; comps</span><span style="font-family:var(--font-mono)">12</span></div>
              <div style="display:flex;justify-content:space-between"><span style="color:#8A939A">Refused at door</span><span style="font-family:var(--font-mono);color:#E8705A">3</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Incident Log</x-import></div>
            <div style="margin-top:18px;display:grid;gap:12px">
              <div style="padding:14px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-radius:10px"><div style="font-size:13.5px">Guest escorted out — refused service</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">23:04 · T. BANKS · NO POLICE</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Spill at bar 2 — cleared, no injury</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">22:18 · R. IGLESIAS</div></div>
            </div>
            <div style="margin-top:16px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" hint-size="100%,32px">Log Incident</x-import></div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Cast Settlement — Queued</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Kamilla Belladonna</span><span style="font-family:var(--font-mono);color:#E3B85F">$650</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Chanel Clitopatra</span><span style="font-family:var(--font-mono);color:#E3B85F">$650</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Jasmine Saville</span><span style="font-family:var(--font-mono);color:#E3B85F">$500</span></div>
            </div>
            <div style="margin-top:16px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="money" size="sm" full="{{ true }}" hint-size="100%,32px">Open Settlements</x-import></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.booking }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Booking Calendar</h1>
        </div>
        <div style="display:flex;align-items:center;gap:14px">
          <span style="font:500 11px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase;color:#8A939A">September 2026</span>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">New Booking</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:flex;gap:22px;margin-bottom:18px;font:500 10px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase;color:#5B646B">
          <span style="display:inline-flex;align-items:center;gap:7px"><span style="width:8px;height:8px;border-radius:2px;background:#2FE0C4"></span>Confirmed</span>
          <span style="display:inline-flex;align-items:center;gap:7px"><span style="width:8px;height:8px;border-radius:2px;background:#E3B85F"></span>Hold</span>
          <span style="display:inline-flex;align-items:center;gap:7px"><span style="width:8px;height:8px;border-radius:2px;background:#7CC2B7"></span>Resident night</span>
          <span style="display:inline-flex;align-items:center;gap:7px"><span style="width:8px;height:8px;border-radius:2px;background:#3A4046"></span>Closed</span>
        </div>

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="display:grid;grid-template-columns:repeat(7,1fr)">
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">SUN</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">MON</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">TUE</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">WED</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">THU</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">FRI</div>
            <div style="padding:14px 16px;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B;border-bottom:1px solid #23282C">SAT</div>

            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#5B646B">30</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#5B646B">31</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">1</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Game night</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">2</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">What It Do?!<br><span style="color:#5B646B">10:30 PM</span></div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">3</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Pool Tournament<br><span style="color:#5B646B">8 PM</span></div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">4</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Drag Karaoke<br><span style="color:#5B646B">9 PM · Marc</span></div></div>
            <div style="min-height:118px;padding:12px 14px;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">5</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #2FE0C4;background:rgba(47,224,196,.09);border-radius:4px;font-size:11.5px;line-height:1.35">Saturday Drag<br><span style="color:#5B646B">Doors 7</span></div></div>

            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">6</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Men Next Door</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C;background:#101315"><div style="font:500 12px/1 var(--font-mono);color:#3A4046">7</div><div style="margin-top:8px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#3A4046">CLOSED</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">8</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Game night</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">9</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">What It Do?!</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">10</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Pool Tournament</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">11</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Drag Karaoke</div></div>
            <div style="min-height:118px;padding:12px 14px;border-bottom:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">12</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #2FE0C4;background:rgba(47,224,196,.09);border-radius:4px;font-size:11.5px;line-height:1.35">Guest headliner<br><span style="color:#5B646B">Contract out</span></div></div>

            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">13</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Men Next Door</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C;background:#101315"><div style="font:500 12px/1 var(--font-mono);color:#3A4046">14</div><div style="margin-top:8px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#3A4046">CLOSED</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">15</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #E3B85F;background:rgba(227,184,95,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Private hire hold<br><span style="color:#5B646B">Expires 25 Aug</span></div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">16</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">What It Do?!</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">17</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Pool Tournament</div></div>
            <div style="min-height:118px;padding:12px 14px;border-right:1px solid #23282C"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">18</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #7CC2B7;background:rgba(124,194,183,.08);border-radius:4px;font-size:11.5px;line-height:1.35">Drag Karaoke</div></div>
            <div style="min-height:118px;padding:12px 14px"><div style="font:500 12px/1 var(--font-mono);color:#EAF0F0">19</div><div style="margin-top:8px;padding:7px 9px;border-left:2px solid #2FE0C4;background:rgba(47,224,196,.09);border-radius:4px;font-size:11.5px;line-height:1.35">Saturday Drag</div></div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Holds Expiring</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <div style="display:flex;align-items:center;justify-content:space-between;gap:14px;padding:14px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-radius:10px"><div><div style="font-size:13.5px">Private hire — 40th birthday, 15 Sep</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">DEPOSIT NOT RECEIVED</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">3 DAYS</span></div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:14px;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:13.5px">Guest headliner — 12 Sep</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">CONTRACT WITH ARTIST</div></div><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">SENT</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Resident Cast Availability</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Kamilla Belladonna</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ALL SEPTEMBER</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Chanel Clitopatra</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">AWAY 18–21</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Jasmine Saville</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ALL SEPTEMBER</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Amethyst Stone Douglas</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">WEDNESDAYS</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Jester Grimm</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">WEDNESDAYS</span></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.scheduling }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Week of 24 August</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Scheduling &amp; Shifts</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Copy Last Week</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Publish Rota</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Scheduled Hours" value="604" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Forecast Labour" value="29.8%" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Open Shifts</x-import></div><div style="margin-top:10px;font:500 30px/1 var(--font-mono);color:#E8705A">2</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Swap Requests" value="3" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="display:grid;grid-template-columns:170px repeat(7,1fr);font-size:12.5px">
            <div style="padding:14px 18px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Staff</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">MON 24</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">TUE 25</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">WED 26</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">THU 27</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FRI 28</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SAT 29</div>
            <div style="padding:14px 10px;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SUN 30</div>

            <div style="padding:12px 18px;border-bottom:1px solid #23282C;font-size:13px">Devon Marsh<div style="font:500 9.5px/1 var(--font-mono);color:#5B646B;margin-top:5px">BARTENDER</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">20–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">20–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">18–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">18–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:12px 18px;border-bottom:1px solid #23282C;font-size:13px">Rosa Iglesias<div style="font:500 9.5px/1 var(--font-mono);color:#5B646B;margin-top:5px">BARTENDER</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">20–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">19–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">18–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(227,184,95,.1);border-left:2px solid #E3B85F;border-radius:4px">18–02 OT</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">19–01</div></div>

            <div style="padding:12px 18px;border-bottom:1px solid #23282C;font-size:13px">Tyrell Banks<div style="font:500 9.5px/1 var(--font-mono);color:#5B646B;margin-top:5px">SECURITY LEAD</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">21–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">21–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">19–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">19–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">19–02</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">20–02</div></div>

            <div style="padding:12px 18px;border-bottom:1px solid #23282C;font-size:13px">Priya Raman<div style="font:500 9.5px/1 var(--font-mono);color:#5B646B;margin-top:5px">KITCHEN</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">17–00</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">17–00</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">17–00</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">16–00</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C"><div style="padding:6px 8px;background:rgba(47,224,196,.1);border-left:2px solid #2FE0C4;border-radius:4px">16–00</div></div>
            <div style="padding:10px;border-bottom:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:12px 18px;font-size:13px">Open — bar 3<div style="font:500 9.5px/1 var(--font-mono);color:#E8705A;margin-top:5px">UNFILLED</div></div>
            <div style="padding:10px;color:#3A4046">—</div>
            <div style="padding:10px;color:#3A4046">—</div>
            <div style="padding:10px;color:#3A4046">—</div>
            <div style="padding:10px;color:#3A4046">—</div>
            <div style="padding:10px"><div style="padding:6px 8px;background:rgba(232,112,90,.1);border-left:2px solid #E8705A;border-radius:4px;color:#E8705A">20–02</div></div>
            <div style="padding:10px"><div style="padding:6px 8px;background:rgba(232,112,90,.1);border-left:2px solid #E8705A;border-radius:4px;color:#E8705A">20–02</div></div>
            <div style="padding:10px;color:#3A4046">—</div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-left:3px solid #E3B85F;border-radius:16px;padding:24px 28px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Coverage Warning</x-import></div>
          <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Friday 28 and Saturday 29 are one bartender short against a 190-head forecast. Rosa Iglesias would cross into overtime if assigned. Two staff have flagged availability for Friday.</p>
          <div style="display:flex;gap:10px;margin-top:16px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Offer To Team</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">View Availability</x-import>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.boxoffice }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Saturday Night Drag Show</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Box Office</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Add Guest List</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Sell At Door</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:1.4fr 1fr;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Ticket Tiers</x-import></div>
            <div style="margin-top:20px;display:grid;gap:10px">
              <div style="display:grid;grid-template-columns:1.4fr .6fr .8fr .7fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div><div style="font-size:14px">General admission · advance</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">21+ · DOORS 7 PM</div></div>
                <div style="font-family:var(--font-mono);font-size:13px;color:#E3B85F">$15.00</div>
                <div style="font-family:var(--font-mono);font-size:13px">98 / 140</div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">ON SALE</div>
              </div>
              <div style="display:grid;grid-template-columns:1.4fr .6fr .8fr .7fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div><div style="font-size:14px">Front table — reserved, 4 seats</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">INCLUDES BOTTLE SERVICE</div></div>
                <div style="font-family:var(--font-mono);font-size:13px;color:#E3B85F">$120.00</div>
                <div style="font-family:var(--font-mono);font-size:13px">6 / 8</div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">2 LEFT</div>
              </div>
              <div style="display:grid;grid-template-columns:1.4fr .6fr .8fr .7fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div><div style="font-size:14px">Walk-up cover</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">NO COVER BEFORE 9 PM</div></div>
                <div style="font-family:var(--font-mono);font-size:13px;color:#E3B85F">$18.00</div>
                <div style="font-family:var(--font-mono);font-size:13px">51</div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">OPEN</div>
              </div>
              <div style="display:grid;grid-template-columns:1.4fr .6fr .8fr .7fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div><div style="font-size:14px">Comp — cast guests &amp; industry</div><div style="margin-top:5px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">MANAGER APPROVAL</div></div>
                <div style="font-family:var(--font-mono);font-size:13px;color:#5B646B">$0.00</div>
                <div style="font-family:var(--font-mono);font-size:13px">12</div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">TRACKED</div>
              </div>
            </div>
            <div style="margin-top:20px;padding:18px;background:#0F1214;border:1px solid #23282C;border-radius:12px;display:flex;justify-content:space-between;align-items:center">
              <span style="font-size:13.5px;color:#8A939A">Door revenue collected tonight</span>
              <span style="font:500 24px/1 var(--font-mono);color:#E3B85F">$3,180</span>
            </div>
          </div>

          <div style="display:grid;gap:16px;align-content:start">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Scanner Status</x-import></div>
              <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
                <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Scanner 1 — main door</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ONLINE</span></div>
                <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Scanner 2 — patio entry</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ONLINE</span></div>
                <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Duplicate scans blocked</span><span style="font-family:var(--font-mono);font-size:12.5px">4</span></div>
              </div>
            </div>
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Guest List</x-import></div>
              <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Kamilla Belladonna +2</span><span style="font:500 10px/1 var(--font-mono);color:#2FE0C4">ARRIVED</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Chanel Clitopatra +2</span><span style="font:500 10px/1 var(--font-mono);color:#2FE0C4">ARRIVED</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Jasmine Saville +2</span><span style="font:500 10px/1 var(--font-mono);color:#5B646B">1 OF 2</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>SADBrunch — promoter</span><span style="font:500 10px/1 var(--font-mono);color:#5B646B">PENDING</span></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.bar }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Live Service</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Bar, Kitchen &amp; POS</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" hint-size="auto,20px">3 Terminals Online</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Sales Tonight" value="$7,942" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Open Tabs" value="34" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Avg Ticket Time</x-import></div><div style="margin-top:10px;font:500 30px/1 var(--font-mono);color:#E8705A">4m 20s</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Comps &amp; Voids" value="$186" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Sales By Station</x-import></div>
            <div style="margin-top:20px;display:grid;gap:16px">
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Bar 1 — Devon</span><span style="font-family:var(--font-mono);color:#E3B85F">$3,410</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:100%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Bar 2 — Rosa</span><span style="font-family:var(--font-mono);color:#E3B85F">$3,168</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:93%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Bar 3 — unstaffed</span><span style="font-family:var(--font-mono);color:#5B646B">$0</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:0%;height:100%;background:#2FE0C4"></div></div></div>
              <div><div style="display:flex;justify-content:space-between;font-size:13.5px"><span>Kitchen</span><span style="font-family:var(--font-mono);color:#E3B85F">$1,364</span></div><div style="margin-top:8px;height:6px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:40%;height:100%;background:#7CC2B7"></div></div></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Top Sellers</x-import></div>
            <div style="margin-top:20px;display:grid;gap:9px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Well vodka soda</span><span style="font-family:var(--font-mono)">142</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Draft — house lager</span><span style="font-family:var(--font-mono)">118</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Loaded fries</span><span style="font-family:var(--font-mono)">64</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Slider trio</span><span style="font-family:var(--font-mono)">47</span></div>
              <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Cactus margarita</span><span style="font-family:var(--font-mono)">39</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Needs Manager Approval</x-import></div>
            <div style="margin-top:20px;display:grid;gap:10px">
              <div style="padding:14px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-radius:10px"><div style="font-size:13.5px">Void — table 4, $86 tab</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">R. IGLESIAS · WRONG TAB</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Comp — cast round, 3 drinks</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">D. MARSH · $34</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Refund — duplicate charge</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">CARD •••4417 · $22</div></div>
            </div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #4A3C1E;border-radius:16px;padding:26px 30px;display:flex;align-items:center;justify-content:space-between;gap:24px;flex-wrap:wrap">
          <div style="max-width:70ch">
            <div style="display:flex;align-items:center;gap:12px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Hardware</x-import></div>
              <span style="display:inline-flex;padding:4px 10px;border-radius:999px;border:1px solid rgba(199,154,69,.55);color:#E3B85F;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Coming Soon</span>
            </div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Tonight's service runs on three third-party terminals. The SpotlightSearch Terminal will add tap, tip prompt and ticket scan on one device at the rail — the software above does not change when it arrives.</p>
          </div>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Join Hardware Pilot</x-import>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.inventory }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Inventory</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Start Weekly Count</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Raise Purchase Order</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Stock On Hand" value="$18,240" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Pour Cost" value="21.4%" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Below Par</x-import></div><div style="margin-top:10px;font:500 30px/1 var(--font-mono);color:#E8705A">6</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Variance · Last Count" value="-$412" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Below Par — Order Before Wednesday</div>
          <div style="display:grid;grid-template-columns:1.5fr .8fr .6fr .6fr .8fr .8fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Item</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Supplier</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">On Hand</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Par</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Suggested</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Cost</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Well vodka — 1.75L</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Coastal Beverage</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E8705A">4</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">14</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">12</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$384</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">House lager — keg</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Tidewater Draft</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E8705A">1</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">4</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">4</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$620</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Lime — case</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Lynnhaven Produce</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">1</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">3</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">2</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$78</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Fry oil — 35lb</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Hampton Foods</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">2</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">5</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">3</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$142</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">Slider buns — 96ct</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Hampton Foods</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E8705A">0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">4</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">4</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$96</div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.workorders }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Maintenance</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Work Orders</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Filters</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Raise Work Order</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid rgba(232,112,90,.3);border-radius:16px;padding:22px"><div style="font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#E8705A">Blocking Service</div><div style="margin-top:10px;font:500 30px/1 var(--font-mono);color:#E8705A">1</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Open" value="7" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Past SLA" value="2" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Closed This Month" value="19" tone="signal" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px">
            <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">New</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);color:#5B646B">3</span>
            </div>
            <div style="display:grid;gap:10px">
              <div style="padding:16px;background:#0F1214;border:1px solid rgba(232,112,90,.34);border-left:3px solid #E8705A;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E8705A">WO-0318 · CRITICAL</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">23:12</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Ice machine not producing — back bar</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Raised by Devon Marsh. Bar 1 is buying bagged ice from the store next door. Photo attached.</div>
                <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap"><span style="padding:3px 8px;border-radius:99px;background:rgba(232,112,90,.12);color:#E8705A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">BLOCKS SERVICE</span><span style="padding:3px 8px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">EQUIPMENT</span></div>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">WO-0317 · LOW</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">21:40</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Patio string light section out</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Raised by Micah Ortega. Cosmetic, no trip hazard.</div>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">WO-0316 · MEDIUM</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">FRI</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Dressing room mirror bulb replacement</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Raised anonymously by a performer. Four of twelve bulbs dead.</div>
              </div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px">
            <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Assigned</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);color:#5B646B">2</span>
            </div>
            <div style="display:grid;gap:10px">
              <div style="padding:16px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-left:3px solid #E3B85F;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">WO-0309 · PAST SLA</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">6 DAYS</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Women's restroom — stall door latch</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Assigned to Coastal Facilities. Vendor has not confirmed a visit.</div>
                <div style="margin-top:12px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">SLA 72H · BREACHED</div>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">WO-0312 · MEDIUM</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">2 DAYS</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Stage monitor crackle on left side</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Assigned to DJ Airrick. Cable swap scheduled Wednesday before doors.</div>
              </div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px">
            <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Resolved · Awaiting Sign-off</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);color:#5B646B">2</span>
            </div>
            <div style="display:grid;gap:10px">
              <div style="padding:16px;background:#0F1214;border:1px solid rgba(47,224,196,.26);border-left:3px solid #2FE0C4;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">WO-0305 · FIXED</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">THU</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Walk-in cooler running warm</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Coastal Facilities replaced the thermostat. Invoice $340 posted to QuickBooks.</div>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid rgba(47,224,196,.26);border-left:3px solid #2FE0C4;border-radius:10px">
                <div style="display:flex;justify-content:space-between;gap:10px"><span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">WO-0301 · FIXED</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">TUE</span></div>
                <div style="margin-top:10px;font-size:14px;font-weight:600">Front entry door closer</div>
                <div style="margin-top:8px;font-size:12.5px;line-height:1.55;color:#8A939A">Adjusted in-house by Tyrell Banks. No cost.</div>
              </div>
            </div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Escalation Rules</x-import></div>
          <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-top:18px">
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E8705A">CRITICAL</div><div style="margin-top:10px;font-size:13px;line-height:1.6;color:#8A939A">Blocks service or is a safety risk. Manager on duty paged immediately, owner notified at two hours.</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">HIGH</div><div style="margin-top:10px;font-size:13px;line-height:1.6;color:#8A939A">Degrades service. Assigned before next doors, 24-hour SLA.</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">MEDIUM</div><div style="margin-top:10px;font-size:13px;line-height:1.6;color:#8A939A">Fix within the week, 72-hour SLA before escalation.</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">LOW</div><div style="margin-top:10px;font-size:13px;line-height:1.6;color:#8A939A">Batched into the monthly maintenance visit.</div></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.cases }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Restricted · Case Handler Access</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">HR Cases</h1>
        </div>
        <span style="display:inline-flex;align-items:center;gap:6px;padding:5px 12px;border-radius:999px;background:rgba(232,112,90,.1);border:1px solid rgba(232,112,90,.3);color:#E8705A;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Audit Logged</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="background:#15181B;border:1px solid #23282C;border-left:3px solid #2FE0C4;border-radius:16px;padding:24px 28px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Who Can See This Page</x-import></div>
          <p style="margin:12px 0 0;max-width:88ch;font-size:13.5px;line-height:1.7;color:#8A939A">Only named case handlers. A manager named in a report is automatically excluded from that case and cannot see it exists. Anonymous reports never expose identity to anyone, including the owner — only the case thread and the reporter's claim code.</p>
        </div>

        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Open Cases" value="4" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Anonymous" value="2" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Awaiting First Response" value="1" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Median Time To First Reply" value="9h" tone="signal" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Case Queue</div>
          <div style="display:grid;grid-template-columns:.7fr 1.6fr .9fr .9fr .8fr .8fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Ref</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Subject</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Category</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Disclosure</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Handler</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">CS-0042</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C">Repeated comments from a colleague during close</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#E8705A">Harassment</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Anonymous</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">External counsel</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E8705A">ESCALATED</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">CS-0041</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C">Rota conflict between two bar staff</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Interpersonal</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Named</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">GM</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">IN MEDIATION</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">CS-0040</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C">Guest conduct toward a performer at the rail</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#E3B85F">Guest conduct</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Confidential</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Security lead</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ACTION TAKEN</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">CS-0039</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C">Dressing room privacy — door does not lock</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Working conditions</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Anonymous</div>
            <div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">GM</div>
            <div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">AWAITING REPLY</div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1.3fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
              <div>
                <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">CS-0042 · Anonymous</x-import></div>
                <div style="margin-top:10px;font-weight:700;font-size:17px">Repeated comments from a colleague during close</div>
              </div>
              <span style="display:inline-flex;padding:5px 12px;border-radius:999px;background:rgba(232,112,90,.1);border:1px solid rgba(232,112,90,.3);color:#E8705A;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Harassment</span>
            </div>
            <div style="margin-top:22px;display:grid;gap:14px">
              <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">REPORTER · ANONYMOUS · 18 AUG 02:14</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#EAF0F0">Report body is visible to the assigned handler only. Identity is not stored against this thread and cannot be recovered by the venue.</p>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid rgba(47,224,196,.22);border-radius:10px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">HANDLER · EXTERNAL COUNSEL · 18 AUG 11:02</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Acknowledged within nine hours. Because the report names a shift supervisor, the case was routed outside the venue's management chain automatically.</p>
              </div>
              <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">REPORTER · VIA CLAIM CODE · 19 AUG 21:30</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Reporter replied using their claim code without revealing who they are.</p>
              </div>
            </div>
            <div style="margin-top:20px;display:flex;gap:10px">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Reply To Reporter</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Record Outcome</x-import>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Routing Policy</x-import></div>
            <div style="margin-top:20px;display:grid;gap:12px;font-size:13.5px;line-height:1.6">
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-weight:600">Maintenance or safety</div><div style="margin-top:6px;color:#8A939A">Becomes a work order. Visible to all managers.</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-weight:600">Interpersonal</div><div style="margin-top:6px;color:#8A939A">Goes to the GM, unless the GM is named.</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid rgba(232,112,90,.3);border-radius:10px"><div style="font-weight:600;color:#E8705A">Harassment or discrimination</div><div style="margin-top:6px;color:#8A939A">Routes to the owner and an external case handler. Never to a line manager, never to anyone named in the report.</div></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-weight:600">Guest conduct</div><div style="margin-top:6px;color:#8A939A">Goes to the security lead with the incident log attached.</div></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.myshift }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Devon Marsh · Bartender</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">My Shift</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" hint-size="auto,20px">Clocked In 18:42</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1060px;margin:0 auto;display:grid;gap:16px">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Tonight</x-import></div>
          <div style="margin-top:14px;font:800 30px/1.05 var(--font-display);letter-spacing:-.01em">Saturday Night Drag Show</div>
          <div style="margin-top:12px;font-size:14px;color:#8A939A">Bar 1 · 18:00 – 02:00 · Manager on duty: Alex Reyes</div>
          <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-top:24px">
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">HOURS SO FAR</div><div style="margin-top:10px;font:500 22px/1 var(--font-mono)">5h 12m</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">BREAK TAKEN</div><div style="margin-top:10px;font:500 22px/1 var(--font-mono)">30m</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">MY SALES</div><div style="margin-top:10px;font:500 22px/1 var(--font-mono);color:#E3B85F">$3,410</div></div>
            <div style="padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">TIP POOL SHARE</div><div style="margin-top:10px;font:500 22px/1 var(--font-mono);color:#E3B85F">$142</div></div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1.2fr 1fr;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Notes From The Manager</x-import></div>
            <div style="margin-top:18px;display:grid;gap:12px;font-size:13.5px;line-height:1.65">
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#EAF0F0">Ice machine is down.</span> <span style="color:#8A939A">Bagged ice is in the walk-in. Work order WO-0318 is open.</span></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#EAF0F0">Tip round is called after Chanel's second set.</span> <span style="color:#8A939A">Hold service during the announcement.</span></div>
              <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#EAF0F0">Front table 3 is a reserved four-top</span> <span style="color:#8A939A">with bottle service — do not seat walk-ups.</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px;display:flex;flex-direction:column">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Quick Actions</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" hint-size="100%,40px">Start Break</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" onClick="{{ go.workorders }}" hint-size="100%,40px">Raise Work Order</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" onClick="{{ go.swaps }}" hint-size="100%,40px">Request Swap</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" full="{{ true }}" onClick="{{ go.report }}" hint-size="100%,40px">Report An Issue</x-import>
            </div>
            <div style="margin-top:auto;padding-top:20px;font-size:12.5px;line-height:1.6;color:#5B646B">Reporting is available to every employee at any time, on or off shift.</div>
          </div>
        </div>

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">My Week</x-import></div>
          <div style="display:grid;grid-template-columns:repeat(7,1fr);gap:12px;margin-top:20px">
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">MON 24</div><div style="margin-top:10px;font-size:13px;color:#3A4046">Off</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">TUE 25</div><div style="margin-top:10px;font-size:13px">20:00–02:00</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">WED 26</div><div style="margin-top:10px;font-size:13px">20:00–02:00</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">THU 27</div><div style="margin-top:10px;font-size:13px;color:#3A4046">Off</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">FRI 28</div><div style="margin-top:10px;font-size:13px">18:00–02:00</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid rgba(47,224,196,.28);border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">SAT 29</div><div style="margin-top:10px;font-size:13px">18:00–02:00</div></div>
            <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">SUN 30</div><div style="margin-top:10px;font-size:13px;color:#3A4046">Off</div></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.timeclock }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Employee</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Clock &amp; Checklists</h1>
        </div>
        <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">On Premises · Verified</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1fr 1.5fr;gap:16px;align-items:start">
        <div style="background:#15181B;border:1px solid rgba(47,224,196,.24);border-radius:16px;padding:32px;text-align:center;box-shadow:0 0 40px rgba(6,229,199,.07)">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Clocked In</x-import></div>
          <div style="margin-top:20px;font:500 52px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">5:12</div>
          <div style="margin-top:10px;font:500 10px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">SINCE 18:42</div>
          <div style="margin-top:26px;display:grid;gap:10px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" hint-size="100%,40px">Start Break</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" full="{{ true }}" hint-size="100%,40px">Clock Out</x-import>
          </div>
          <p style="margin:20px 0 0;font-size:12.5px;line-height:1.6;color:#5B646B">Clock-out is blocked until the closing check-off is complete. A manager can override with a reason.</p>
        </div>

        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Opening Check-off · Bar 1</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">8 / 8 COMPLETE</span>
            </div>
            <div style="margin-top:18px;display:grid;gap:8px;font-size:13.5px">
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Till float counted and signed</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Wells stocked to par</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Glassware washed and racked</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Ice wells filled — bagged ice tonight</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Drains and mats clear</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Fridge temperatures logged</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Terminal paired and test charge cleared</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="color:#2FE0C4">✓</span><span style="color:#8A939A">Fire exits unobstructed</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Closing Check-off · Unlocks At Last Call</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">0 / 7</span>
            </div>
            <div style="margin-top:18px;display:grid;gap:8px;font-size:13.5px">
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Tabs closed or transferred</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Till counted, cash dropped to safe</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Card tips declared</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Bottles capped, speed rails wiped</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Glass washer drained</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Low stock flagged for the count</span></div>
              <div style="display:flex;gap:12px;align-items:center;padding:11px 14px;background:#0F1214;border:1px solid #23282C;border-radius:9px"><span style="width:14px;height:14px;border:1px solid #3A4046;border-radius:3px;flex:none"></span><span style="color:#8A939A">Anything broken raised as a work order</span></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.swaps }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Employee</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Swaps &amp; Availability</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Offer A Shift</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.2fr 1fr;gap:16px;align-items:start">
        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Shifts Up For Grabs</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid rgba(232,112,90,.28);border-radius:10px">
                <div><div style="font-size:14px">Friday 28 Aug · Bar 3 · 20:00–02:00</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E8705A">UNFILLED · POSTED BY MANAGER</div></div>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,30px">Claim</x-import>
              </div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid rgba(232,112,90,.28);border-radius:10px">
                <div><div style="font-size:14px">Saturday 29 Aug · Bar 3 · 20:00–02:00</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E8705A">UNFILLED · POSTED BY MANAGER</div></div>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,30px">Claim</x-import>
              </div>
              <div style="display:flex;align-items:center;justify-content:space-between;gap:16px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px">
                <div><div style="font-size:14px">Sunday 30 Aug · Door · 20:00–02:00</div><div style="margin-top:6px;font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">OFFERED BY MICAH ORTEGA</div></div>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Take It</x-import>
              </div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">My Requests</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Tuesday 25 Aug — drop shift</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">AWAITING MANAGER</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Wednesday 2 Sep — swap with Rosa</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">APPROVED</span></div>
            </div>
          </div>
        </div>

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">My Availability</x-import></div>
          <p style="margin:12px 0 0;font-size:13px;line-height:1.6;color:#8A939A">Availability feeds the rota builder. Managers cannot schedule you outside these windows without asking.</p>
          <div style="margin-top:20px;display:grid;gap:9px;font-size:13.5px">
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Monday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#3A4046">UNAVAILABLE</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Tuesday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">FROM 19:00</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Wednesday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">FROM 19:00</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Thursday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#3A4046">UNAVAILABLE</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Friday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ANY TIME</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Saturday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ANY TIME</span></div>
            <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Sunday</span><span style="font:500 10px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">ON REQUEST</span></div>
          </div>
          <div style="margin-top:18px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" hint-size="100%,32px">Edit Availability</x-import></div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.report }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Employee · Confidential</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Report an Issue</h1>
        </div>
        <span style="display:inline-flex;align-items:center;gap:6px;padding:5px 12px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Encrypted</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.4fr 1fr;gap:16px;align-items:start">
        <div style="display:grid;gap:16px">

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Step 1 · What kind of issue is this?</x-import></div>
            <div style="display:grid;grid-template-columns:repeat(2,1fr);gap:10px;margin-top:20px">
              <button onClick="{{ setCat.maintenance }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;background:{{ ct.maintenance.bg }};border:1px solid {{ ct.maintenance.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:#EAF0F0">Something is broken</div>
                <div style="margin-top:7px;font-size:12.5px;line-height:1.55;color:#8A939A">Equipment, fixtures, the building. Becomes a work order.</div>
              </button>
              <button onClick="{{ setCat.interpersonal }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;background:{{ ct.interpersonal.bg }};border:1px solid {{ ct.interpersonal.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:#EAF0F0">Conflict with a colleague</div>
                <div style="margin-top:7px;font-size:12.5px;line-height:1.55;color:#8A939A">Working relationships, scheduling disputes, conduct on shift.</div>
              </button>
              <button onClick="{{ setCat.harassment }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;background:{{ ct.harassment.bg }};border:1px solid {{ ct.harassment.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:#EAF0F0">Harassment or discrimination</div>
                <div style="margin-top:7px;font-size:12.5px;line-height:1.55;color:#8A939A">Routed outside the management chain. Never to anyone you name.</div>
              </button>
              <button onClick="{{ setCat.guest }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;background:{{ ct.guest.bg }};border:1px solid {{ ct.guest.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:#EAF0F0">Guest conduct or safety</div>
                <div style="margin-top:7px;font-size:12.5px;line-height:1.55;color:#8A939A">Goes to the security lead with tonight's incident log attached.</div>
              </button>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Step 2 · How do you want to be identified?</x-import></div>
            <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:20px">
              <button onClick="{{ setMode.named }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;text-align:center;background:{{ rm.named.bg }};border:1px solid {{ rm.named.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:{{ rm.named.fg }}">Named</div>
                <div style="margin-top:7px;font-size:12px;line-height:1.5;color:#8A939A">Your name is on the report</div>
              </button>
              <button onClick="{{ setMode.confidential }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;text-align:center;background:{{ rm.confidential.bg }};border:1px solid {{ rm.confidential.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:{{ rm.confidential.fg }}">Confidential</div>
                <div style="margin-top:7px;font-size:12px;line-height:1.5;color:#8A939A">Handler only, not the venue</div>
              </button>
              <button onClick="{{ setMode.anonymous }}" style="all:unset;cursor:pointer;padding:18px;border-radius:12px;text-align:center;background:{{ rm.anonymous.bg }};border:1px solid {{ rm.anonymous.bd }}">
                <div style="font-size:14.5px;font-weight:600;color:{{ rm.anonymous.fg }}">Anonymous</div>
                <div style="margin-top:7px;font-size:12px;line-height:1.5;color:#8A939A">No identity is ever stored</div>
              </button>
            </div>

            <sc-if value="{{ isNamed }}">
              <div style="margin-top:18px;padding:18px;background:#0F1214;border:1px solid #23282C;border-radius:12px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">WHAT HAPPENS</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Your name is attached. The handler can speak to you directly and follow up in person. Your report and any outcome are recorded against your file.</p>
              </div>
            </sc-if>
            <sc-if value="{{ isConfidential }}">
              <div style="margin-top:18px;padding:18px;background:#0F1214;border:1px solid #23282C;border-radius:12px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">WHAT HAPPENS</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Your identity is held by the assigned handler only and is not visible to managers, the owner, or anyone named in the report. It is disclosed further only with your written consent, or where the law requires it.</p>
              </div>
            </sc-if>
            <sc-if value="{{ isAnonymous }}">
              <div style="margin-top:18px;padding:18px;background:#0F1214;border:1px solid rgba(47,224,196,.24);border-radius:12px">
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">WHAT HAPPENS</div>
                <p style="margin:10px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">No identity is stored against this report — not your name, not your account, not your device. You receive a claim code that lets you read replies and add to the thread without ever revealing who you are. Nobody at the venue can reverse it.</p>
                <div style="margin-top:14px;display:flex;align-items:center;gap:12px;padding:14px;background:#15181B;border:1px dashed #3A4046;border-radius:10px">
                  <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">YOUR CLAIM CODE</span>
                  <span style="font:500 17px/1 var(--font-mono);letter-spacing:.12em;color:#EAF0F0">RC-7QM4-8XVD</span>
                  <span style="margin-left:auto;font-size:12px;color:#5B646B">Write this down. It cannot be reissued.</span>
                </div>
              </div>
            </sc-if>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:30px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Step 3 · Tell us what happened</x-import></div>
            <div style="margin-top:18px;display:grid;gap:14px">
              <div>
                <div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">When did it happen?</div>
                <div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;color:#5B646B">Saturday 22 August · during close</div>
              </div>
              <div>
                <div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">In your own words</div>
                <div style="min-height:150px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;line-height:1.7;color:#5B646B">Describe what happened, who was involved, and whether anyone else saw it. There is no word limit and no required format.</div>
              </div>
              <div style="display:flex;align-items:center;gap:12px;padding:16px;background:#0F1214;border:1px dashed #3A4046;border-radius:10px;font-size:13.5px;color:#5B646B">
                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#5B646B" stroke-width="1.8"><path d="M12 16V4m0 0L8 8m4-4 4 4"/><path d="M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-2"/></svg>
                Attach a photo, screenshot or document — metadata is stripped on upload
              </div>
            </div>
            <div style="margin-top:22px;display:flex;gap:10px;align-items:center">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" hint-size="auto,40px">Submit Report</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="md" hint-size="auto,40px">Save Draft</x-import>
            </div>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid rgba(47,224,196,.22);border-radius:16px;padding:26px;box-shadow:0 0 34px rgba(6,229,199,.06)">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Our Commitment</x-import></div>
            <div style="margin-top:18px;display:grid;gap:14px;font-size:13.5px;line-height:1.65;color:#8A939A">
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Every report is acknowledged within 24 hours.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Nobody you name in a report can see it, respond to it, or learn it exists.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Harassment and discrimination reports route to the owner and an external handler — never to a shift manager.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Retaliation for filing a report is itself a reportable offence.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>You can withdraw a named or confidential report at any time.</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Check On A Report</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Filed anonymously? Enter your claim code to read replies without identifying yourself.</p>
            <div style="margin-top:16px;padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font:500 15px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">RC-••••-••••</div>
            <div style="margin-top:12px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" hint-size="100%,32px">Open Thread</x-import></div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">If You Are In Danger Right Now</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Do not use this form. Find the security lead on the floor or call 911. The incident log can be completed afterwards.</p>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.mypay }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Devon Marsh · Bartender</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">My Pay &amp; Tips</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Download Pay Stub</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="This Period · Wages" value="$798" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Tips" value="$412" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Hours" value="38.0" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Pays On" value="28 Aug" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="display:grid;grid-template-columns:1.3fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
            <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Shift Breakdown</div>
            <div style="display:grid;grid-template-columns:1fr .8fr .6fr .7fr .7fr;font-size:13.5px">
              <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Date</div>
              <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Shift</div>
              <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Hrs</div>
              <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Wages</div>
              <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Tips</div>

              <div style="padding:14px 26px;border-top:1px solid #23282C">Tue 18 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bar 1 · 20–02</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">6.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$126</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$48</div>

              <div style="padding:14px 26px;border-top:1px solid #23282C">Wed 19 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bar 1 · 20–02</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">6.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$126</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$71</div>

              <div style="padding:14px 26px;border-top:1px solid #23282C">Fri 21 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bar 1 · 18–02</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">8.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$168</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$151</div>

              <div style="padding:14px 26px;border-top:1px solid #23282C">Sat 22 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C;color:#8A939A">Bar 1 · 18–02</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">8.0</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$168</div><div style="padding:14px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$142</div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">How Your Tips Are Calculated</x-import></div>
            <p style="margin:14px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Card tips are pooled across the night and split by the published rule. Your share is proportional to hours worked on the floor.</p>
            <div style="margin-top:20px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Pool tonight</span><span style="font-family:var(--font-mono);color:#E3B85F">$2,722</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Bar share — 70%</span><span style="font-family:var(--font-mono);color:#E3B85F">$1,905</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Your hours of bar hours</span><span style="font-family:var(--font-mono)">7.5%</span></div>
              <div style="display:flex;justify-content:space-between;padding:15px 14px;background:#0F1214;border:1px solid rgba(199,154,69,.3);border-radius:10px;font-weight:600"><span>Your share</span><span style="font-family:var(--font-mono);color:#E3B85F">$142</span></div>
            </div>
            <div style="margin-top:16px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="sm" full="{{ true }}" hint-size="100%,32px">Dispute A Calculation</x-import></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.bookings }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Kamilla Belladonna · Drag Artist · Hampton Roads</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">My Bookings</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Set Availability</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.4fr 1fr;gap:16px;align-items:start">
        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">My Venues</x-import></div>
              <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase;color:#5B646B">3 Active · 1 Applied</span>
            </div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A;max-width:70ch">Your account is yours. Each venue you work with is a portal — open one for its bookings, contracts and payments. Leaving a venue does not touch your profile, your rider or your history.</p>
            <div style="display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:20px">
              <button onClick="{{ go.venueportal }}" style="all:unset;cursor:pointer;display:block;padding:18px;background:#0F1214;border:1px solid rgba(47,224,196,.3);border-radius:12px">
                <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
                  <div style="font-family:var(--font-display);font-weight:800;font-size:15px;letter-spacing:.01em"><span style="color:#EAF0F0">The Rainbow </span><span style="color:#E8705A">C</span><span style="color:#E3B85F">A</span><span style="color:#2FE0C4">C</span><span style="color:#7CC2B7">T</span><span style="color:#9BA8E8">US</span></div>
                  <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">RESIDENT</span>
                </div>
                <div style="margin-top:10px;font-size:12.5px;color:#8A939A">Virginia Beach, VA · 4 dates booked · $934 due tonight</div>
                <div style="margin-top:14px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">OPEN PORTAL →</div>
              </button>
              <div style="padding:18px;background:#0F1214;border:1px solid #23282C;border-radius:12px">
                <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
                  <div style="font-size:15px;font-weight:700;color:#EAF0F0">Norfolk Social Club</div>
                  <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">GUEST</span>
                </div>
                <div style="margin-top:10px;font-size:12.5px;color:#8A939A">Norfolk, VA · 1 date booked · contract signed</div>
                <div style="margin-top:14px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">OPEN PORTAL →</div>
              </div>
              <div style="padding:18px;background:#0F1214;border:1px solid #23282C;border-radius:12px">
                <div style="display:flex;align-items:center;justify-content:space-between;gap:12px">
                  <div style="font-size:15px;font-weight:700;color:#EAF0F0">The Manor · Richmond</div>
                  <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">GUEST</span>
                </div>
                <div style="margin-top:10px;font-size:12.5px;color:#8A939A">Richmond, VA · brunch series · 2 dates held</div>
                <div style="margin-top:14px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">OPEN PORTAL →</div>
              </div>
              <button onClick="{{ go.opencalls }}" style="all:unset;cursor:pointer;display:block;padding:18px;background:#0F1214;border:1px dashed #3A4046;border-radius:12px">
                <div style="font-size:15px;font-weight:700;color:#8A939A">Find another room</div>
                <div style="margin-top:10px;font-size:12.5px;color:#8A939A">14 venues on SpotlightSearch are casting in Hampton Roads this month.</div>
                <div style="margin-top:14px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">BROWSE OPEN CALLS →</div>
              </button>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid rgba(47,224,196,.24);border-radius:16px;padding:30px;box-shadow:0 0 34px rgba(6,229,199,.06)">
            <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">Next Booking · Tonight · The Rainbow Cactus</x-import></div>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" dot="{{ false }}" hint-size="auto,20px">Confirmed</x-import>
            </div>
            <div style="margin-top:16px;font:800 28px/1.05 var(--font-display);letter-spacing:-.01em">Saturday Night Drag Show</div>
            <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-top:22px">
              <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">CALL TIME</div><div style="margin-top:9px;font-size:14px">18:30</div></div>
              <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SET</div><div style="margin-top:9px;font-size:14px">22:30 · opener</div></div>
              <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">NUMBERS</div><div style="margin-top:9px;font-size:14px">3</div></div>
              <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FEE</div><div style="margin-top:9px;font:500 14px/1 var(--font-mono);color:#E3B85F">$650 + tips</div></div>
            </div>
            <div style="margin-top:22px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px;line-height:1.65;color:#8A939A">Dressing room 2. Four mirror bulbs are out — work order WO-0316 is open. Music files were received Thursday and are loaded to DJ Airrick's rig.</div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Upcoming</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <div style="display:grid;grid-template-columns:1.2fr .9fr .7fr .8fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px">
                <div>Sat 29 Aug</div><div style="color:#8A939A">Saturday Drag Show</div><div style="font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CONFIRMED</div>
              </div>
              <div style="display:grid;grid-template-columns:1.2fr .9fr .7fr .8fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px">
                <div>Wed 2 Sep</div><div style="color:#8A939A">What It Do?!</div><div style="font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$300</div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">CONFIRMED</div>
              </div>
              <div style="display:grid;grid-template-columns:1.2fr .9fr .7fr .8fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-radius:10px;font-size:13.5px">
                <div>Sat 12 Sep</div><div style="color:#8A939A">Guest headliner support</div><div style="font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$800</div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">SIGN CONTRACT</div>
              </div>
              <div style="display:grid;grid-template-columns:1.2fr .9fr .7fr .8fr;gap:14px;align-items:center;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px">
                <div>Sat 19 Sep</div><div style="color:#8A939A">Saturday Drag Show</div><div style="font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#8A939A">HOLD</div>
              </div>
            </div>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Year To Date</x-import></div>
            <div style="margin-top:18px;display:grid;gap:12px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span style="color:#8A939A">Shows performed</span><span style="font-family:var(--font-mono)">61</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span style="color:#8A939A">Fees earned</span><span style="font-family:var(--font-mono);color:#E3B85F">$34,150</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:13.5px"><span style="color:#8A939A">Tips recorded</span><span style="font-family:var(--font-mono);color:#E3B85F">$11,480</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid rgba(199,154,69,.3);border-radius:10px;font-size:13.5px"><span style="color:#8A939A">1099 accrual</span><span style="font-family:var(--font-mono);color:#E3B85F">$34,150</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Blackout Dates</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.6;color:#8A939A">The booking team sees these before offering a date.</p>
            <div style="margin-top:16px;display:grid;gap:9px;font-size:13.5px">
              <div style="padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px">18 – 21 September · touring</div>
              <div style="padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px">24 December – 2 January</div>
            </div>
            <div style="margin-top:14px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" hint-size="100%,32px">Add Blackout</x-import></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.contracts }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Performer</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Contracts</h1>
        </div>
        <span style="display:inline-flex;align-items:center;gap:6px;padding:5px 12px;border-radius:999px;background:rgba(47,224,196,.12);border:1px solid rgba(47,224,196,.32);color:#2FE0C4;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">DocuSign Connected</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.4fr 1fr;gap:16px;align-items:start">
        <div style="background:#15181B;border:1px solid rgba(227,184,95,.3);border-radius:16px;padding:30px">
          <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Awaiting Your Signature</x-import></div>
            <span style="font:500 10px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SENT 20 AUG</span>
          </div>
          <div style="margin-top:16px;font:800 24px/1.15 var(--font-display);letter-spacing:-.01em">Performance Agreement — 12 September 2026</div>
          <div style="margin-top:22px;display:grid;gap:0;font-size:13.5px">
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Engagement</span><span>Guest headliner support · 2 numbers</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Call time</span><span>18:00 · sound check 19:15</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Guarantee</span><span style="font-family:var(--font-mono);color:#E3B85F">$800</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Tips</span><span>Retained in full by the performer</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Payment terms</span><span>Settled same night by 02:30</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Cancellation</span><span>7 days notice, or 50% of guarantee</span></div>
            <div style="display:flex;justify-content:space-between;padding:14px 0"><span style="color:#8A939A">Rider attached</span><span style="color:#2FE0C4">Yes — v3, 12 Aug 2026</span></div>
          </div>
          <div style="margin-top:24px;display:flex;gap:10px;align-items:center;flex-wrap:wrap">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" hint-size="auto,40px">Review &amp; Sign</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" hint-size="auto,40px">Request A Change</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="md" hint-size="auto,40px">Download PDF</x-import>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Signed &amp; On File</x-import></div>
            <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Resident cast agreement 2026</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SIGNED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>W-9 — tax year 2026</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SIGNED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Venue conduct policy</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SIGNED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Media &amp; likeness release</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SIGNED</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Payment Details</x-import></div>
            <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Method</span><span>Direct deposit</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Account</span><span style="font-family:var(--font-mono);font-size:12.5px">••••8140</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Cash option</span><span>Available at settlement</span></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.settlements }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Performer</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Settlements</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Export For Tax</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.3fr 1fr;gap:16px;align-items:start">
        <div style="background:#15181B;border:1px solid rgba(199,154,69,.32);border-radius:16px;padding:30px;box-shadow:0 0 30px rgba(199,154,69,.08)">
          <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Tonight's Settlement Sheet</x-import></div>
            <span style="display:inline-flex;padding:4px 10px;border-radius:999px;border:1px solid rgba(199,154,69,.5);color:#E3B85F;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase">Ready To Sign</span>
          </div>
          <div style="margin-top:18px;font-size:14px;color:#8A939A">Saturday Night Drag Show · 22 August 2026</div>
          <div style="margin-top:24px;display:grid;gap:0;font-size:14px">
            <div style="display:flex;justify-content:space-between;padding:15px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Guarantee</span><span style="font-family:var(--font-mono);color:#E3B85F">$650.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:15px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Card tips collected on your behalf</span><span style="font-family:var(--font-mono);color:#E3B85F">$284.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:15px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Cash tips — recorded, retained by you</span><span style="font-family:var(--font-mono);color:#8A939A">$310.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:15px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Deductions</span><span style="font-family:var(--font-mono);color:#8A939A">$0.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:20px 0;font-size:18px;font-weight:700"><span>Payable tonight</span><span style="font-family:var(--font-mono);color:#E3B85F">$934.00</span></div>
          </div>
          <div style="margin-top:12px;padding:16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:12.5px;line-height:1.65;color:#5B646B">Signing this sheet confirms the amounts above and releases payment. The signed copy is filed to your contract record and posted to QuickBooks as a contractor expense.</div>
          <div style="margin-top:20px;display:flex;gap:10px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="money" size="md" hint-size="auto,40px">Sign &amp; Accept</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" hint-size="auto,40px">Query An Amount</x-import>
          </div>
        </div>

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Settlement History</div>
          <div style="display:grid;grid-template-columns:1fr .8fr .7fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Date</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Paid</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

            <div style="padding:14px 26px;border-top:1px solid #23282C">15 Aug · Saturday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$891</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SETTLED</div>
            <div style="padding:14px 26px;border-top:1px solid #23282C">12 Aug · Wednesday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$418</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SETTLED</div>
            <div style="padding:14px 26px;border-top:1px solid #23282C">8 Aug · Saturday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$1,024</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SETTLED</div>
            <div style="padding:14px 26px;border-top:1px solid #23282C">5 Aug · Wednesday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$372</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SETTLED</div>
            <div style="padding:14px 26px;border-top:1px solid #23282C">1 Aug · Saturday</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$960</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SETTLED</div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.rider }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Performer</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Rider &amp; Media Kit</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Publish Update</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.2fr 1fr;gap:16px;align-items:start">
        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Technical Rider · v3</x-import></div>
              <span style="font:500 10px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">UPDATED 12 AUG</span>
            </div>
            <div style="margin-top:20px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Sound</span><span>Wireless handheld, monitor stage left</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Lighting</span><span>Follow spot for opening number</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Stage</span><span>Clear wing space stage right for a quick change</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Dressing room</span><span>Lockable, mirror lighting, two hanging rails</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Hospitality</span><span>Still water, no dairy</span></div>
              <div style="display:flex;justify-content:space-between;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Music delivery</span><span>WAV, uploaded 72 hours before doors</span></div>
            </div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Boundaries</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Visible to bookers before an offer is made. Editable by the performer only.</p>
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:20px">
              <div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">DISCUSS WITH ME FIRST</div>
                <div style="margin-top:12px;display:grid;gap:8px;font-size:13px">
                  <div style="padding:11px 13px;background:#0F1214;border:1px solid #23282C;border-radius:9px">Audience interaction segments</div>
                  <div style="padding:11px 13px;background:#0F1214;border:1px solid #23282C;border-radius:9px">Sets running past 01:00</div>
                </div>
              </div>
              <div>
                <div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E8705A">NOT AVAILABLE FOR</div>
                <div style="margin-top:12px;display:grid;gap:8px;font-size:13px">
                  <div style="padding:11px 13px;background:#0F1214;border:1px solid #23282C;border-radius:9px">Outdoor stages without cover</div>
                  <div style="padding:11px 13px;background:#0F1214;border:1px solid #23282C;border-radius:9px">Unpaid promotional appearances</div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Media Kit</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Used on the public event page and in flyer artwork. Approve before anything goes out.</p>
            <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Press photo — landscape</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">APPROVED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Press photo — square</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">APPROVED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid rgba(227,184,95,.3);border-radius:10px"><span>Flyer draft — 12 Sep</span><span style="font:500 9.5px/1 var(--font-mono);color:#E3B85F">REVIEW</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Short bio — 60 words</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">APPROVED</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Socials On File</x-import></div>
            <div style="margin-top:18px;display:grid;gap:9px;font-size:13px;color:#8A939A">
              <div style="padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px">instagram.com/</div>
              <div style="padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px">tiktok.com/</div>
              <div style="padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px">Booking email</div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.listing }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Public · therainbowcactus.gay/events</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Event Listing</h1>
        </div>
        <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Venue-Owned · No Third Party</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="height:230px;background:radial-gradient(90% 140% at 20% 0%,rgba(6,229,199,.14) 0%,transparent 60%),#0F1214;border-bottom:1px solid #23282C;display:flex;align-items:center;justify-content:center">
            <span style="font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#3A4046">Event Artwork · Uploaded By The Venue</span>
          </div>
          <div style="padding:32px;display:grid;grid-template-columns:1.5fr 1fr;gap:32px">
            <div>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tone="signal" theme="dark" hint-size="auto,12px">Saturday 29 August 2026</x-import>
              <h2 style="margin:16px 0 0;font:800 40px/1.05 var(--font-display);letter-spacing:-.015em">Saturday Night Drag Show</h2>
              <p style="margin:16px 0 0;font-size:15px;line-height:1.7;color:#8A939A;max-width:56ch">Kamilla Belladonna, Chanel Clitopatra and Jasmine Saville take the stage, with music by DJ Airrick. Doors at 7 PM, show at 10:30 PM. Kitchen open until midnight.</p>
              <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:28px">
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">DOORS</div><div style="margin-top:9px;font-size:14px">7:00 PM</div></div>
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SHOW</div><div style="margin-top:9px;font-size:14px">10:30 PM</div></div>
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">AGE</div><div style="margin-top:9px;font-size:14px">21+</div></div>
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">PARKING</div><div style="margin-top:9px;font-size:14px">Free on site</div></div>
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">VENUE</div><div style="margin-top:9px;font-size:14px">475 S. Lynnhaven Rd</div></div>
                <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">REFUNDS</div><div style="margin-top:9px;font-size:14px">No refunds</div></div>
              </div>
            </div>
            <div style="background:#0F1214;border:1px solid #23282C;border-radius:14px;padding:26px;align-self:start">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Tickets</x-import></div>
              <div style="margin-top:18px;display:grid;gap:10px">
                <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#15181B;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">General admission</div><div style="margin-top:5px;font:500 9.5px/1 var(--font-mono);color:#5B646B">42 LEFT</div></div><span style="font:500 16px/1 var(--font-mono);color:#E3B85F">$15</span></div>
                <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#15181B;border:1px solid #23282C;border-radius:10px"><div><div style="font-size:14px">Front table · 4 seats</div><div style="margin-top:5px;font:500 9.5px/1 var(--font-mono);color:#E3B85F">2 LEFT</div></div><span style="font:500 16px/1 var(--font-mono);color:#E3B85F">$120</span></div>
              </div>
              <div style="margin-top:18px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" full="{{ true }}" onClick="{{ go.checkout }}" hint-size="100%,40px">Get Tickets</x-import></div>
              <p style="margin:16px 0 0;font-size:12px;line-height:1.6;color:#5B646B">No per-ticket platform fee. Card processing is shown at checkout.</p>
            </div>
          </div>
        </div>

        <div style="margin-top:16px;display:grid;grid-template-columns:repeat(3,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">WED 26 AUG</div><div style="margin-top:12px;font-weight:600;font-size:15px">What It Do?!</div><div style="margin-top:8px;font-size:13px;color:#8A939A">Hosted by Amethyst Stone Douglas, Kamilla Belladonna and Jester Grimm. 10:30 PM.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">THU 27 AUG</div><div style="margin-top:12px;font-weight:600;font-size:15px">Pool Tournament</div><div style="margin-top:8px;font-size:13px;color:#8A939A">Free to play. 8 PM start, sign-up at the bar.</div></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:24px"><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;color:#5B646B">FRI 28 AUG</div><div style="margin-top:12px;font-weight:600;font-size:15px">Drag Karaoke with Marc</div><div style="margin-top:8px;font-size:13px;color:#8A939A">9 PM. Viewing party from 8 PM.</div></div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.checkout }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Public · Secure Checkout</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Checkout</h1>
        </div>
        <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Held For 8:00</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1060px;margin:0 auto;display:grid;grid-template-columns:1.3fr 1fr;gap:16px;align-items:start">
        <div style="display:grid;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Your Details</x-import></div>
            <div style="margin-top:20px;display:grid;grid-template-columns:1fr 1fr;gap:14px">
              <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Full name</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;color:#5B646B">As it appears on your ID</div></div>
              <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Email</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;color:#5B646B">Ticket is sent here</div></div>
              <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Mobile</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;color:#5B646B">+1</div></div>
              <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Date of birth</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font-size:14px;color:#5B646B">21+ event</div></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Payment</x-import></div>
              <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">PROCESSED ON A THIRD-PARTY TERMINAL RAIL</span>
            </div>
            <div style="margin-top:20px;display:grid;gap:14px">
              <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Card number</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font:500 14px/1 var(--font-mono);letter-spacing:.1em;color:#5B646B">•••• •••• •••• ••••</div></div>
              <div style="display:grid;grid-template-columns:1fr 1fr;gap:14px">
                <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">Expiry</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font:500 14px/1 var(--font-mono);color:#5B646B">MM / YY</div></div>
                <div><div style="font-size:12.5px;color:#8A939A;margin-bottom:8px">CVC</div><div style="padding:14px 16px;background:#0F1214;border:1px solid #23282C;border-radius:10px;font:500 14px/1 var(--font-mono);color:#5B646B">•••</div></div>
              </div>
            </div>
            <div style="margin-top:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" full="{{ true }}" onClick="{{ go.ticket }}" hint-size="100%,40px">Pay $32.24</x-import></div>
            <p style="margin:16px 0 0;font-size:12px;line-height:1.6;color:#5B646B">By completing this purchase you accept the venue's no-refund policy and 21+ entry requirement. Your ticket is valid for one entry.</p>
          </div>
        </div>

        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px;align-self:start">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Order Summary</x-import></div>
          <div style="margin-top:18px;font-size:14px;line-height:1.5">Saturday Night Drag Show<div style="margin-top:6px;font-size:13px;color:#8A939A">Sat 29 Aug · doors 7:00 PM</div></div>
          <div style="margin-top:22px;display:grid;gap:0;font-size:13.5px">
            <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">General admission × 2</span><span style="font-family:var(--font-mono);color:#E3B85F">$30.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Platform fee</span><span style="font-family:var(--font-mono);color:#2FE0C4">$0.00</span></div>
            <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Card processing</span><span style="font-family:var(--font-mono);color:#E3B85F">$1.17</span></div>
            <div style="display:flex;justify-content:space-between;padding:13px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Virginia admissions tax</span><span style="font-family:var(--font-mono);color:#E3B85F">$1.07</span></div>
            <div style="display:flex;justify-content:space-between;padding:18px 0;font-size:17px;font-weight:700"><span>Total</span><span style="font-family:var(--font-mono);color:#E3B85F">$32.24</span></div>
          </div>
          <div style="margin-top:8px;padding:16px;background:#0F1214;border:1px solid rgba(47,224,196,.22);border-radius:10px;font-size:12.5px;line-height:1.65;color:#8A939A">The same two tickets on the incumbent platform would total <span style="color:#EAF0F0;font-family:var(--font-mono)">$37.94</span>. The difference stays with the venue and the guest.</div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.ticket }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Guest</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Digital Ticket</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Add To Wallet</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1060px;margin:0 auto;display:grid;grid-template-columns:.9fr 1.1fr;gap:16px;align-items:start">
        <div style="background:#15181B;border:1px solid rgba(47,224,196,.26);border-radius:16px;padding:32px;box-shadow:0 0 40px rgba(6,229,199,.07)">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="signal" theme="dark" hint-size="auto,12px">The Rainbow Cactus</x-import></div>
          <div style="margin-top:14px;font:800 24px/1.15 var(--font-display);letter-spacing:-.01em">Saturday Night Drag Show</div>
          <div style="margin-top:8px;font-size:13.5px;color:#8A939A">Sat 29 Aug 2026 · doors 7:00 PM · 21+</div>
          <div style="margin-top:26px;aspect-ratio:1;background:#0F1214;border:1px solid #23282C;border-radius:12px;display:flex;align-items:center;justify-content:center">
            <span style="font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#3A4046">Rotating QR · Refreshes Every 30s</span>
          </div>
          <div style="margin-top:22px;display:grid;gap:0;font-size:13.5px">
            <div style="display:flex;justify-content:space-between;padding:12px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Admits</span><span>2 guests</span></div>
            <div style="display:flex;justify-content:space-between;padding:12px 0;border-bottom:1px solid #23282C"><span style="color:#8A939A">Order</span><span style="font-family:var(--font-mono);font-size:12.5px">RC-2026-08-4471</span></div>
            <div style="display:flex;justify-content:space-between;padding:12px 0"><span style="color:#8A939A">Status</span><span style="color:#2FE0C4">Valid — not yet scanned</span></div>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Before You Arrive</x-import></div>
            <div style="margin-top:18px;display:grid;gap:12px;font-size:13.5px;line-height:1.65;color:#8A939A">
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Bring photo ID. This is a 21+ event and everyone is checked at the door.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Parking is free on site at 475 S. Lynnhaven Road.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Kitchen serves until midnight — sliders and loaded fries are the house order.</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Tip the cast. Cash and card tipping are both available at the rail.</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manage</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px">
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" hint-size="100%,40px">Transfer A Ticket</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" full="{{ true }}" hint-size="100%,40px">Reserve A Table</x-import>
              <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="md" full="{{ true }}" hint-size="100%,40px">Contact The Venue</x-import>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.purchasing }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Vendor Portal · Coastal Beverage</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Purchase Orders</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Confirm Delivery Window</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Awaiting Confirmation" value="1" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="In Transit" value="2" tone="default" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Invoiced This Month" value="$14,820" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:22px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Paid" value="100%" tone="signal" theme="dark" size="md" hint-size="auto,64px"></x-import></div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Open Orders</div>
          <div style="display:grid;grid-template-columns:.8fr 1.4fr .9fr .8fr .8fr .9fr;font-size:13.5px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">PO</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Contents</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Requested</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Value</div>
            <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Terms</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">2214</div><div style="padding:15px 12px;border-top:1px solid #23282C">Well spirits, house lager kegs</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Wed 26 Aug · AM</div><div style="padding:15px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$3,940</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Net 30</div><div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">CONFIRM</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">2209</div><div style="padding:15px 12px;border-top:1px solid #23282C">Mixers and garnish</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Mon 24 Aug · AM</div><div style="padding:15px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$680</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Net 30</div><div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">IN TRANSIT</div>

            <div style="padding:15px 26px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">2205</div><div style="padding:15px 12px;border-top:1px solid #23282C">Premium tequila — event stock</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Mon 24 Aug · PM</div><div style="padding:15px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$1,240</div><div style="padding:15px 12px;border-top:1px solid #23282C;color:#8A939A">Net 30</div><div style="padding:15px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">IN TRANSIT</div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px">
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Delivery Rules</x-import></div>
          <p style="margin:12px 0 0;max-width:82ch;font-size:13.5px;line-height:1.7;color:#8A939A">Deliveries are accepted between 10:00 and 15:00 only — the venue is a live room after 16:00. Rear entrance on the west side. Every delivery is signed for in the platform by the manager on duty; the invoice posts to QuickBooks against this purchase order automatically.</p>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.receiving }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Manager · Back Of House</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Receiving</h1>
        </div>
        <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Delivery Window 10:00 – 15:00</span>
      </header>
      <div style="padding:32px 40px 80px;max-width:1180px;margin:0 auto;display:grid;grid-template-columns:1.3fr 1fr;gap:16px;align-items:start">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
          <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Checking In · PO 2209 · Coastal Beverage</x-import></div>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="caution" dot="{{ false }}" hint-size="auto,20px">2 Discrepancies</x-import>
          </div>
          <div style="margin-top:20px;display:grid;grid-template-columns:1.6fr .6fr .6fr .8fr;font-size:13.5px">
            <div style="padding:11px 0;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Item</div>
            <div style="padding:11px 0;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Ordered</div>
            <div style="padding:11px 0;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Received</div>
            <div style="padding:11px 0;border-bottom:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Note</div>

            <div style="padding:14px 0;border-bottom:1px solid #23282C">Tonic — 24 pack</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">8</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#2FE0C4">8</div><div style="padding:14px 0;border-bottom:1px solid #23282C;color:#5B646B">—</div>

            <div style="padding:14px 0;border-bottom:1px solid #23282C">Soda water — 24 pack</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">10</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">7</div><div style="padding:14px 0;border-bottom:1px solid #23282C;color:#E3B85F">Short 3 — credit raised</div>

            <div style="padding:14px 0;border-bottom:1px solid #23282C">Lime — case</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">2</div><div style="padding:14px 0;border-bottom:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#2FE0C4">2</div><div style="padding:14px 0;border-bottom:1px solid #23282C;color:#5B646B">—</div>

            <div style="padding:14px 0">Cocktail cherries</div><div style="padding:14px 0;font-family:var(--font-mono);font-size:12.5px">4</div><div style="padding:14px 0;font-family:var(--font-mono);font-size:12.5px;color:#E8705A">0</div><div style="padding:14px 0;color:#E8705A">Not delivered</div>
          </div>
          <div style="margin-top:22px;display:flex;gap:10px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="md" hint-size="auto,40px">Sign For Delivery</x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="md" hint-size="auto,40px">Reject Line Items</x-import>
          </div>
        </div>

        <div style="display:grid;gap:16px;align-content:start">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Today's Deliveries</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Coastal Beverage · 11:20</span><span style="font:500 9.5px/1 var(--font-mono);color:#E3B85F">CHECKING</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Hampton Foods · 13:00</span><span style="font:500 9.5px/1 var(--font-mono);color:#5B646B">EXPECTED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Lynnhaven Produce · 09:40</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">SIGNED</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Automatic On Sign-off</x-import></div>
            <div style="margin-top:16px;display:grid;gap:12px;font-size:13.5px;line-height:1.6;color:#8A939A">
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Stock levels update against par</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Invoice posts to QuickBooks as accounts payable</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Credit note requested for short or missing lines</span></div>
              <div style="display:flex;gap:11px"><span style="color:#2FE0C4">✓</span><span>Pour cost recalculated for the week</span></div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.door }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Platform</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Door &amp; Access</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" hint-size="auto,20px">All Devices Online</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="display:grid;grid-template-columns:1.2fr 1fr;gap:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Devices</x-import></div>
            <div style="margin-top:20px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Scanner 1 — main entrance</div><div style="color:#8A939A">Micah Ortega</div><div style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">ONLINE · 98%</div></div>
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Scanner 2 — patio entry</div><div style="color:#8A939A">Security floater</div><div style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">ONLINE · 71%</div></div>
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Terminal — bar 1</div><div style="color:#8A939A">Devon Marsh</div><div style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">ONLINE</div></div>
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Terminal — bar 2</div><div style="color:#8A939A">Rosa Iglesias</div><div style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">ONLINE</div></div>
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Terminal — bar 3</div><div style="color:#8A939A">Unassigned</div><div style="font:500 9.5px/1 var(--font-mono);color:#5B646B">IDLE</div></div>
              <div style="display:grid;grid-template-columns:1.4fr .9fr .7fr;gap:14px;align-items:center;padding:15px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div>Back-of-house door reader</div><div style="color:#8A939A">Badge access</div><div style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">ARMED</div></div>
            </div>
          </div>

          <div style="display:grid;gap:16px;align-content:start">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Occupancy</x-import></div>
              <div style="margin-top:16px;display:flex;align-items:baseline;gap:10px"><span style="font:500 44px/1 var(--font-mono);letter-spacing:-.02em;color:#EAF0F0">187</span><span style="font-size:14px;color:#5B646B">/ 240 certified</span></div>
              <div style="margin-top:14px;height:8px;background:#23282C;border-radius:99px;overflow:hidden"><div style="width:78%;height:100%;background:#2FE0C4"></div></div>
              <p style="margin:16px 0 0;font-size:12.5px;line-height:1.6;color:#5B646B">Scanners stop admitting at 235 and alert the security lead. The count is exportable for a fire inspection.</p>
            </div>
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Back Of House Access</x-import></div>
              <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Dressing rooms</span><span style="font:500 9.5px/1 var(--font-mono);color:#8A939A">CAST + GM</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Office &amp; safe</span><span style="font:500 9.5px/1 var(--font-mono);color:#8A939A">OWNER + GM</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Stock room</span><span style="font:500 9.5px/1 var(--font-mono);color:#8A939A">BAR + MANAGERS</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Rear delivery door</span><span style="font:500 9.5px/1 var(--font-mono);color:#8A939A">10:00–15:00</span></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.admin }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Platform</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Admin &amp; Roles</h1>
        </div>
        <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,32px">Invite A User</x-import>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
          <div style="padding:22px 26px 14px;font:500 10px/1 var(--font-mono);letter-spacing:.2em;text-transform:uppercase;color:#5B646B">Permission Matrix</div>
          <div style="display:grid;grid-template-columns:1.5fr repeat(5,.8fr);font-size:13px">
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Capability</div>
            <div style="padding:12px 10px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">OWNER</div>
            <div style="padding:12px 10px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">GM</div>
            <div style="padding:12px 10px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">SHIFT MGR</div>
            <div style="padding:12px 10px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">STAFF</div>
            <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">PERFORMER</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">View nightly financials</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#8A939A">Partial</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Approve payroll</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Publish the rota</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Comp or void a sale</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#8A939A">Request</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Raise a work order</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#2FE0C4">✓</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">File a report of any kind</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#2FE0C4">✓</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Read HR cases</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#8A939A">Handler only</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#8A939A">Handler only</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#3A4046">—</div>

            <div style="padding:13px 26px;border-top:1px solid #23282C">Sign a settlement</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#2FE0C4">✓</div><div style="padding:13px 10px;border-top:1px solid #23282C;color:#3A4046">—</div><div style="padding:13px 26px;border-top:1px solid #23282C;color:#2FE0C4">Own only</div>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:16px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Case Handlers</x-import></div>
            <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Who receives each report category. A handler named in a report is excluded automatically.</p>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Maintenance</span><span style="color:#8A939A">GM · shift managers</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Interpersonal</span><span style="color:#8A939A">GM</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid rgba(232,112,90,.3);border-radius:10px"><span>Harassment</span><span style="color:#E8705A">Owner + external counsel</span></div>
              <div style="display:flex;justify-content:space-between;padding:13px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Guest conduct</span><span style="color:#8A939A">Security lead</span></div>
            </div>
          </div>
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Connected Services</x-import></div>
            <div style="margin-top:18px;display:grid;gap:10px;font-size:13.5px">
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>QuickBooks</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">CONNECTED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>DocuSign</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">CONNECTED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Google Calendar</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">CONNECTED</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid rgba(199,154,69,.32);border-radius:10px"><span>SpotlightSearch Terminal</span><span style="font:500 9.5px/1 var(--font-mono);color:#E3B85F">COMING SOON</span></div>
              <div style="display:flex;justify-content:space-between;align-items:center;padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span>Third-party card terminals</span><span style="font:500 9.5px/1 var(--font-mono);color:#2FE0C4">3 PAIRED</span></div>
            </div>
          </div>
        </div>

        <div style="margin-top:16px;background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px;display:flex;justify-content:space-between;align-items:center;gap:24px;flex-wrap:wrap">
          <div style="font-size:12.5px;line-height:1.7;color:#5B646B;max-width:70ch">The Rainbow Cactus · 475 S. Lynnhaven Rd, Virginia Beach, VA 23452 · (757) 368-0441 · contactus@TheRainbowCactus.Gay — proudly serving Virginia Beach's LGBTQ+ community and allies since 1997.</div>
          <span style="font:500 10px/1 var(--font-mono);letter-spacing:.18em;text-transform:uppercase;color:#5B646B">Powered by SpotlightSearch.io</span>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.opencalls }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div>
          <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Artist Account · Network Wide</x-import></div>
          <h1 style="margin:8px 0 0;font:800 30px/1 var(--font-display);letter-spacing:-.02em;color:#EAF0F0">Open Calls</h1>
        </div>
        <div style="display:flex;gap:10px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Filters</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Newest First</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px 30px;display:flex;align-items:center;justify-content:space-between;gap:24px;flex-wrap:wrap">
          <div style="max-width:78ch">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tone="signal" theme="dark" hint-size="auto,12px">Your profile travels with you</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">Every venue on SpotlightSearch sees the same rider, boundaries, media kit and settlement history — you maintain it once. Venues never see what another venue pays you.</p>
          </div>
          <div style="display:flex;gap:28px">
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">PROFILE STRENGTH</div><div style="margin-top:10px;font:500 24px/1 var(--font-mono);color:#2FE0C4">92%</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">APPLICATIONS OUT</div><div style="margin-top:10px;font:500 24px/1 var(--font-mono);color:#EAF0F0">3</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">BOOKED RATE</div><div style="margin-top:10px;font:500 24px/1 var(--font-mono);color:#EAF0F0">64%</div></div>
          </div>
        </div>

        <div style="margin-top:16px;display:grid;gap:12px">
          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px;display:grid;grid-template-columns:1.6fr 1fr 1fr .9fr auto;gap:24px;align-items:center">
            <div>
              <div style="font-size:17px;font-weight:700">Friday Night Headliner · 8-week residency</div>
              <div style="margin-top:8px;font-size:13px;color:#8A939A">Norfolk Social Club · Norfolk, VA · 21+</div>
              <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap"><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">DRAG</span><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">HOSTING</span><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">LIP SYNC</span></div>
            </div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FEE</div><div style="margin-top:9px;font:500 15px/1 var(--font-mono);color:#E3B85F">$550 / night</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">DATES</div><div style="margin-top:9px;font-size:13.5px">Fridays from 18 Sep</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">CLOSES</div><div style="margin-top:9px;font:500 13px/1 var(--font-mono);color:#E3B85F">2 SEP</div></div>
            <div style="display:grid;gap:8px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,30px">Apply</x-import><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Details</x-import></div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px;display:grid;grid-template-columns:1.6fr 1fr 1fr .9fr auto;gap:24px;align-items:center">
            <div>
              <div style="font-size:17px;font-weight:700">Sunday Drag Brunch · rotating cast</div>
              <div style="margin-top:8px;font-size:13px;color:#8A939A">The Manor · Richmond, VA · all ages before 4 PM</div>
              <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap"><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">BRUNCH</span><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">FAMILY FRIENDLY SET</span></div>
            </div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FEE</div><div style="margin-top:9px;font:500 15px/1 var(--font-mono);color:#E3B85F">$400 + tips</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">DATES</div><div style="margin-top:9px;font-size:13.5px">6 &amp; 20 Sep</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">STATUS</div><div style="margin-top:9px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#2FE0C4">APPLIED · 21 AUG</div></div>
            <div style="display:grid;gap:8px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Withdraw</x-import><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Details</x-import></div>
          </div>

          <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px;display:grid;grid-template-columns:1.6fr 1fr 1fr .9fr auto;gap:24px;align-items:center">
            <div>
              <div style="font-size:17px;font-weight:700">Pride Kickoff · guest performer, one night</div>
              <div style="margin-top:8px;font-size:13px;color:#8A939A">Harbour Room · Newport News, VA · 18+</div>
              <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap"><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">DRAG</span><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">LIVE VOCAL</span></div>
            </div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FEE</div><div style="margin-top:9px;font:500 15px/1 var(--font-mono);color:#E3B85F">$900</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">DATES</div><div style="margin-top:9px;font-size:13.5px">5 Jun 2027</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">CLOSES</div><div style="margin-top:9px;font:500 13px/1 var(--font-mono);color:#8A939A">30 SEP</div></div>
            <div style="display:grid;gap:8px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" hint-size="auto,30px">Apply</x-import><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Details</x-import></div>
          </div>

          <div style="background:#15181B;border:1px solid rgba(227,184,95,.3);border-radius:16px;padding:26px;display:grid;grid-template-columns:1.6fr 1fr 1fr .9fr auto;gap:24px;align-items:center">
            <div>
              <div style="font-size:17px;font-weight:700">Guest headliner support · 12 September</div>
              <div style="margin-top:8px;font-size:13px;color:#8A939A">The Rainbow Cactus · Virginia Beach, VA · offered directly to you</div>
              <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap"><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">2 NUMBERS</span><span style="padding:4px 9px;border-radius:99px;background:#1B1F22;color:#8A939A;font:500 9px/1.4 var(--font-mono);letter-spacing:.1em">RIDER ACCEPTED</span></div>
            </div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">FEE</div><div style="margin-top:9px;font:500 15px/1 var(--font-mono);color:#E3B85F">$800</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">DATES</div><div style="margin-top:9px;font-size:13.5px">Sat 12 Sep</div></div>
            <div><div style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">STATUS</div><div style="margin-top:9px;font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#E3B85F">SIGN CONTRACT</div></div>
            <div style="display:grid;gap:8px"><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="primary" size="sm" onClick="{{ go.contracts }}" hint-size="auto,30px">Review</x-import><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,30px">Decline</x-import></div>
          </div>
        </div>
      </div>
    </sc-if>

    <sc-if value="{{ pg.venueportal }}">
      <header style="position:sticky;top:0;z-index:5;display:flex;align-items:center;justify-content:space-between;gap:24px;padding:18px 40px;background:rgba(12,14,16,.94);backdrop-filter:blur(10px);border-bottom:1px solid #1B1F22">
        <div style="display:flex;align-items:center;gap:14px">
          <button onClick="{{ go.bookings }}" style="all:unset;cursor:pointer;font:500 10px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">My Bookings ›</button>
          <div style="font-family:var(--font-display);font-weight:800;font-size:24px;letter-spacing:.01em"><span style="color:#EAF0F0">The Rainbow </span><span style="color:#E8705A">C</span><span style="color:#E3B85F">A</span><span style="color:#F2D06B">C</span><span style="color:#2FE0C4">T</span><span style="color:#7CC2B7">U</span><span style="color:#9BA8E8">S</span></div>
        </div>
        <div style="display:flex;align-items:center;gap:12px">
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Badge" status="healthy" hint-size="auto,20px">Resident Cast</x-import>
          <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" hint-size="auto,32px">Message The Venue</x-import>
        </div>
      </header>
      <div style="padding:32px 40px 80px;max-width:1320px;margin:0 auto">
        <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:28px 30px;display:flex;align-items:center;justify-content:space-between;gap:28px;flex-wrap:wrap">
          <div style="max-width:60ch">
            <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Venue Portal · Since March 2024</x-import></div>
            <p style="margin:12px 0 0;font-size:13.5px;line-height:1.7;color:#8A939A">475 S. Lynnhaven Rd, Virginia Beach · resident on Saturdays and alternate Wednesdays. This portal covers only your engagements here. Your profile, rider and network-wide history stay in your artist account.</p>
          </div>
          <div style="display:flex;gap:34px">
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Shows Here · YTD" value="47" theme="dark" size="md" hint-size="auto,64px"></x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Earned Here" value="$26,480" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import>
            <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Stat" label="Due Tonight" value="$934" tone="money" theme="dark" size="md" hint-size="auto,64px"></x-import>
          </div>
        </div>

        <div style="display:grid;grid-template-columns:1.4fr 1fr;gap:16px;margin-top:16px;align-items:start">
          <div style="display:grid;gap:16px">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
              <div style="padding:22px 26px 14px;display:flex;align-items:center;justify-content:space-between">
                <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Bookings At This Venue</x-import></div>
                <span style="font:500 9.5px/1 var(--font-mono);letter-spacing:.14em;color:#5B646B">NEXT 6 WEEKS</span>
              </div>
              <div style="display:grid;grid-template-columns:.9fr 1.3fr .7fr .8fr .8fr;font-size:13.5px">
                <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Date</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Engagement</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Call</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Fee</div>
                <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C;color:#2FE0C4">Tonight</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show · opener</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">18:30</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">ON TONIGHT</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">Sat 29 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">18:30</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">CONFIRMED</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">Wed 2 Sep</div><div style="padding:14px 12px;border-top:1px solid #23282C">What It Do?!</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">21:30</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$300</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">CONFIRMED</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">Sat 12 Sep</div><div style="padding:14px 12px;border-top:1px solid #23282C">Guest headliner support</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">18:00</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$800</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">SIGN CONTRACT</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">Sat 19 Sep</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px">18:30</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#8A939A">HOLD</div>
              </div>
            </div>

            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;overflow:hidden">
              <div style="padding:22px 26px 14px;display:flex;align-items:center;justify-content:space-between">
                <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Payments From This Venue</x-import></div>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="sm" onClick="{{ go.settlements }}" hint-size="auto,30px">All Settlements</x-import>
              </div>
              <div style="display:grid;grid-template-columns:.9fr 1.1fr .7fr .7fr .8fr;font-size:13.5px">
                <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Date</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">For</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Fee</div>
                <div style="padding:12px 12px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Tips</div>
                <div style="padding:12px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.16em;text-transform:uppercase;color:#5B646B">Status</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C;color:#E3B85F">Tonight</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$284</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">READY TO SIGN</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">15 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$241</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">PAID</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">12 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C">What It Do?!</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$300</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$118</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">PAID</div>

                <div style="padding:14px 26px;border-top:1px solid #23282C">8 Aug</div><div style="padding:14px 12px;border-top:1px solid #23282C">Saturday Drag Show</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$650</div><div style="padding:14px 12px;border-top:1px solid #23282C;font-family:var(--font-mono);font-size:12.5px;color:#E3B85F">$374</div><div style="padding:14px 26px;border-top:1px solid #23282C;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#2FE0C4">PAID</div>
              </div>
            </div>
          </div>

          <div style="display:grid;gap:16px;align-content:start">
            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Tonight At This Venue</x-import></div>
              <div style="margin-top:18px;display:grid;gap:9px;font-size:13.5px">
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Call time</span><span>18:30</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Your set</span><span>22:30 · 3 numbers</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Dressing room</span><span>Room 2</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Also on the bill</span><span>Chanel, Jasmine</span></div>
                <div style="display:flex;justify-content:space-between;padding:12px 14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><span style="color:#8A939A">Music</span><span style="color:#2FE0C4">Loaded to DJ Airrick</span></div>
              </div>
            </div>

            <div style="background:#15181B;border:1px solid rgba(227,184,95,.3);border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="money" theme="dark" hint-size="auto,12px">Needs You</x-import></div>
              <div style="margin-top:16px;display:grid;gap:10px">
                <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Sign the 12 September contract</div><div style="margin-top:6px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">SENT 20 AUG · $800</div></div>
                <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Approve the 12 Sep flyer artwork</div><div style="margin-top:6px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#E3B85F">AWAITING YOU</div></div>
                <div style="padding:14px;background:#0F1214;border:1px solid #23282C;border-radius:10px"><div style="font-size:13.5px">Confirm the 19 Sep hold</div><div style="margin-top:6px;font:500 9.5px/1 var(--font-mono);letter-spacing:.12em;color:#5B646B">EXPIRES 26 AUG</div></div>
              </div>
            </div>

            <div style="background:#15181B;border:1px solid #23282C;border-radius:16px;padding:26px">
              <div><x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Kicker" tick="{{ false }}" tone="neutral" theme="dark" hint-size="auto,12px">Raise Something Here</x-import></div>
              <p style="margin:12px 0 0;font-size:13px;line-height:1.65;color:#8A939A">Performers have the same reporting rights as staff at any venue they work.</p>
              <div style="margin-top:16px;display:grid;gap:10px">
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="secondary" size="sm" full="{{ true }}" onClick="{{ go.report }}" hint-size="100%,32px">Report An Issue</x-import>
                <x-import component-from-global-scope="SpotlightSearchIoDesignSystem_957fb6.Button" variant="ghost" size="sm" full="{{ true }}" hint-size="100%,32px">Leave This Venue</x-import>
              </div>
            </div>
          </div>
        </div>
      </div>
    </sc-if>

    <div id="ss-pages-end" style="height:1px"></div>
  </main>
</div>
</x-dc>
<script type="text/x-dc" data-dc-script data-props="{&quot;$preview&quot;:{&quot;width&quot;:1440,&quot;height&quot;:900},&quot;startPage&quot;:{&quot;editor&quot;:&quot;enum&quot;,&quot;options&quot;:[&quot;cover&quot;,&quot;command&quot;,&quot;tonight&quot;,&quot;report&quot;,&quot;listing&quot;],&quot;default&quot;:&quot;cover&quot;,&quot;tsType&quot;:&quot;string&quot;,&quot;section&quot;:&quot;Demo&quot;},&quot;disclosureDefault&quot;:{&quot;editor&quot;:&quot;enum&quot;,&quot;options&quot;:[&quot;named&quot;,&quot;confidential&quot;,&quot;anonymous&quot;],&quot;default&quot;:&quot;anonymous&quot;,&quot;tsType&quot;:&quot;string&quot;,&quot;section&quot;:&quot;Reporting&quot;}}">
class Component extends DCLogic {
  state = { page: null, mode: null, cat: 'harassment' };
  map = {
    cover:1, problem:1, platform:1, integrations:1, migration:1,
    command:1, financials:1, payroll:1, analytics:1, compliance:1,
    tonight:1, booking:1, scheduling:1, boxoffice:1, bar:1, inventory:1, workorders:1, cases:1,
    myshift:1, timeclock:1, swaps:1, report:1, mypay:1,
    bookings:1, opencalls:1, venueportal:1, contracts:1, settlements:1, rider:1,
    listing:1, checkout:1, ticket:1, purchasing:1, receiving:1,
    door:1, admin:1
  };
  _go = {};
  goTo(p){
    this.setState({ page: p });
    const el = document.getElementById('ss-main');
    if (el) el.scrollTop = 0;
  }
  renderVals(){
    const cur = this.state.page ?? (this.props.startPage || 'cover');
    const mode = this.state.mode ?? (this.props.disclosureDefault || 'anonymous');
    const nv = {}, pg = {}, go = {};
    Object.keys(this.map).forEach(k => {
      const on = k === cur;
      nv[k] = {
        bg: on ? 'rgba(6,229,199,.10)' : 'transparent',
        fg: on ? '#2FE0C4' : '#8A939A'
      };
      pg[k] = on;
      if (!this._go[k]) this._go[k] = () => this.goTo(k);
      go[k] = this._go[k];
    });
    const modes = ['named','confidential','anonymous'];
    const rm = {}, setMode = {};
    modes.forEach(m => {
      const on = m === mode;
      rm[m] = {
        bg: on ? 'rgba(6,229,199,.09)' : '#0F1214',
        bd: on ? 'rgba(47,224,196,.42)' : '#23282C',
        fg: on ? '#2FE0C4' : '#EAF0F0'
      };
      if (!this._go['m_'+m]) this._go['m_'+m] = () => this.setState({ mode: m });
      setMode[m] = this._go['m_'+m];
    });

    const cats = ['maintenance','interpersonal','harassment','guest'];
    const ct = {}, setCat = {};
    cats.forEach(c => {
      const on = c === this.state.cat;
      ct[c] = {
        bg: on ? 'rgba(6,229,199,.07)' : '#0F1214',
        bd: on ? 'rgba(47,224,196,.38)' : '#23282C'
      };
      if (!this._go['c_'+c]) this._go['c_'+c] = () => this.setState({ cat: c });
      setCat[c] = this._go['c_'+c];
    });

    const performerPages = ['bookings','opencalls','venueportal','contracts','settlements','rider'];
    const isPerformer = performerPages.indexOf(cur) !== -1;

    return {
      nv, pg, go, rm, setMode, ct, setCat,
      isPerformer, isVenue: !isPerformer,
      isNamed: mode === 'named',
      isConfidential: mode === 'confidential',
      isAnonymous: mode === 'anonymous'
    };
  }
}
</script>
</body>
</html>
