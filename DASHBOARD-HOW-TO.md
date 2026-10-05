# How to Use Your Publicis Account Dashboard

## Quick Start: Opening the Dashboard

1. **Open the file in your browser** (pick one):
   - Finder: Go to `/Desktop/Ogury Sales assistant/Reference Files/outputs/`
   - Look for: `diana-dashboard.html`
   - Double-click it to open in your browser

2. **Bookmark it** (so you can find it fast next time):
   - When it opens, do Cmd+D (Mac) or Ctrl+D (Windows)
   - Save the bookmark to your Bookmarks Bar

That's it! The dashboard will load automatically with your current data.

---

## What's on the Dashboard

### The Top Bar (Blue)
- **Title:** "Diana's Publicis Account Dashboard"
- **"Last updated:"** Shows when data was last loaded
- **Three buttons:**
  - 🔄 **Reload Data** — Click to refresh if you think data has changed
  - ⬇️ **Export** — Downloads your data as a .json file (backup/archive)
  - 🗑️ **Clear Local** — Wipes out your local notes (red button; careful!)

### The Colored Boxes (Metrics)
Four big boxes showing:
- 🟢 **Active Actions** — Your to-do items (not marked done yet)
- 🔵 **Publicis Accounts** — How many accounts you're tracking
- 🔴 **Open Opportunities** — Pipeline deals in play
- 🔷 **Upcoming Meetings** — Client meetings on your calendar

Click on any tab below to see full details.

---

## The Seven Tabs

### 1. **Dashboard** (Default View)
Quick overview showing:
- Your top 3 most urgent actions
- Key tier-1 accounts
- Total pipeline value
- All in one place

Good for: Morning check-in, quick scan.

---

### 2. **Action Queue**
Your to-do list for this week and beyond.

**What you see:**
- Cards for each action you own
- Status badges: 🟦 AWAITING INTERNAL | 🟨 AWAITING CLIENT
- Due dates in bold (red if overdue)
- High Priority 🔴 flag

**What you can do:**
- **Search** — Type in the search box to find an action
- **Filter by Status** — Show only "Active", "Awaiting Client", etc.
- **Add Local Notes** — Click in the "Local Notes" box to write your own notes (saved locally on your computer)
- **Mark as Done / Defer / Dismiss** — Click the buttons to change status
  - **Done** ✓ — You completed it (hides from count)
  - **Defer** ⏸️ — Move it to later (still tracks but grayed out)
  - **Dismiss** ✕ — Remove it from view (you can always see dismissed items later)

**Everything in Local Notes stays saved** — Even if you close and reopen the dashboard, your notes are still there (stored on your computer, not in the cloud).

---

### 3. **Accounts**
Your Publicis account roster.

**What you see:**
A table with columns:
- **Account** — Company name
- **Agency** — Publicis agency/holding (Publicis Collective, Razorfish, Spark Foundry, etc.)
- **Priority** — 🔴 Tier 1 (strategic) | 🟡 Tier 2 (growth) | 🟢 Tier 3 (maintenance)
- **Status** — Active / Prospect / Handoff
- **Pipeline** — Total value and status (e.g., "$700K+", "in setup")
- **Next Action** — What needs to happen next

**What you can do:**
- **Search** — Find an account by name
- **Filter by Priority** — Show only Tier 1, or all tiers, etc.

---

### 4. **Pipeline**
All your open opportunities (deals in play).

**What you see:**
A table showing:
- **Opportunity** — Deal name
- **Client** — Who it's for (Microsoft, American Airlines, Verizon, etc.)
- **Amount** — Deal value
- **Stage** — 🟦 Proposal / RFP | 🟨 Negotiation | 🟢 Live
- **Close Date** — When it's supposed to close
- **Next Step** — Your next move

**What you can do:**
- **Search** — Find a deal by name
- **Filter by Stage** — Show only proposals, negotiations, or live deals

---

### 5. **Relationships**
Your key contacts and engagement status.

**What you see:**
Cards for each contact showing:
- **Name** and **Company**
- **Role** — What they do
- **Relationship** — (Client Lead, Manager, Team, etc.)
- **Last Engaged** — When you last interacted
- **Next Action** — What you should do next

Good for: Keeping relationships warm, prepping for calls.

---

### 6. **Meetings**
Your upcoming client meetings.

**What you see:**
- **Meeting title**
- **Date & Time**
- **Who's attending**
- **Location**
- **Agenda**
- Whether a prep brief is available (if 📋 shows, there's a pre-written brief)

Good for: Staying on top of your calendar, knowing what to prep.

---

### 7. **IDP & Goals**
Your Individual Development Plan tracking.

**What you see:**
- Your current level (Senior Account Executive)
- Progress toward Sales Director (percentage)
- Target promotion date
- Your three 90-day IDP priorities with:
  - What you're trying to do
  - How long it should take
  - Current status
  - Evidence of progress so far

Good for: Keeping your promotion goals visible, tracking momentum.

---

## How to Keep Your Data Fresh

### What the Dashboard Does Automatically
- Loads your latest actions, accounts, meetings, and pipeline from saved snapshots
- Shows the date/time of the last refresh in the header

### When Data Gets Outdated
The dashboard uses data from:
- Your daily emails and calendar (snapshots saved on 2026-10-05)
- Your reference files (Publicis Master Contacts, campaign trackers, etc.)
- Your IDP working plan

If things change outside this dashboard (Salesforce updates, new emails, calendar changes), the dashboard **won't see them** until you refresh.

### How to Refresh (Three Options)

**Option 1: Quick Reload (Easiest)**
- Click the 🔄 **Reload Data** button
- This reloads the same snapshot data (good if you just closed and reopened the browser)

**Option 2: Full Refresh with Live Data (Best)**
- Open Claude Code (this session)
- Run: `/refresh-dashboard`
- This skill will:
  - Check your live Gmail and Google Calendar for new emails/meetings
  - Check Salesforce for pipeline updates (if connected)
  - Re-fetch your Publicis account and contact data
  - Update the dashboard with fresh data
  - Save a new snapshot

**Option 3: Manual Update (If You Need Something Specific)**
- Reach out to Claude Code and say: "Add [account/action/meeting] to the dashboard"
- Provide the details, and it gets added

---

## Your Data is Local & Safe

### What This Means
- **Local:** The dashboard file lives on your computer (not in the cloud)
- **Safe:** Your notes, local status changes, and personal tracking stay on your computer only
- **Private:** No data is sent to external services unless you explicitly connect them

### What Stays on Your Computer
- Your action notes and status changes (Done/Defer/Dismiss)
- All the data shown (accounts, pipeline, relationships, meetings)
- Refresh history

### What's NOT Stored Here
- Salesforce records (read-only link; you can click to view in Salesforce)
- Email threads (view in Gmail)
- Calendar events (view in Google Calendar)

---

## Troubleshooting

### "Metrics show 0 — Where's my data?"
- Try refreshing: Press F5 in the browser, or click 🔄 **Reload Data**
- If still empty: Restart the browser
- Last resort: Click 🗑️ **Clear Local**, then reload

### "I lost my notes — Can I get them back?"
- If you cleared local data with the 🗑️ button, they're gone (can't recover)
- Notes are only stored on your computer, not backed up elsewhere
- Best practice: Export your data with ⬇️ **Export** to create a backup .json file periodically

### "The pipeline number looks wrong"
- Numbers come from Salesforce snapshot (as of 2026-10-05)
- To see real-time Salesforce: Click the Salesforce link in the card, or run `/refresh-dashboard`

### "Can I edit Salesforce from here?"
- **No.** The dashboard is read-only
- To update Salesforce, click the link or open Salesforce directly
- Changes you make in Salesforce won't show here until you run `/refresh-dashboard`

### "Can I export this to send to my manager?"
- Yes! Click ⬇️ **Export** to download a .json file
- It's your data snapshot as of that moment

---

## Tips for Power Users

### 1. Keyboard Shortcuts
- **F5** — Refresh the page
- **Cmd+D (Mac) / Ctrl+D (Windows)** — Bookmark the dashboard
- **Cmd+F (Mac) / Ctrl+F (Windows)** — Search on page (browser's find)

### 2. Mark Actions Done Early
- When you complete something, click ✓ **Done** immediately
- This keeps your active count honest and unclutters your queue

### 3. Use Local Notes for Context
- Write small notes about each action (blockers, next steps, context)
- They're always there when you reopen the dashboard
- Example: "Waiting on Angela's email response; will follow up Tue morning"

### 4. Filter Before Searching
- If you have a long action queue, filter by status first, then search
- Faster than scrolling through everything

### 5. Export Regularly
- Every week or before big meetings, click ⬇️ **Export**
- Creates a backup of your current data (just in case)
- Useful for archiving weekly snapshots

---

## Questions?

If something isn't working or you need help:
- **Dashboard isn't loading?** Close the browser, reopen the file
- **Data looks stale?** Run `/refresh-dashboard` from Claude Code
- **Need to add/change data?** Ask Claude Code (this session) to update it
- **Want to customize?** Tell Claude Code what you'd like to see

---

**Your dashboard is now live. Visit it whenever you need a quick view of your priorities, accounts, and next actions.**
