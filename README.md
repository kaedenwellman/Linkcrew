# ACP Link Crew — Informational Website

A self-guided, interactive website built for Arizona College Prep High School's Link Crew chapter. Designed to serve two distinct audiences from a single URL: prospective student applicants and newly selected Link Crew leaders.

---

## What This Site Does

### Public Section
The public-facing section introduces Link Crew to any ACP student considering applying. It covers what the program is, what leaders actually do, what they get out of it, and what to realistically expect before committing. The goal is to lower the barrier for strong applicants who might self-select out due to uncertainty, while setting honest expectations for everyone who applies.

Includes a placeholder section for application details to be filled in each cycle by the Link Crew advisor.

### Gated Leader Section
The second half of the site is locked behind a passcode delivered through the official acceptance email. Once unlocked, newly selected leaders get a practical walkthrough of everything they need before their first event:

- A full breakdown of Orientation Day, including an interactive demonstration of the Ball Juggling Game — the group activity used to teach freshmen about teamwork, name retention, and handling complexity together
- A detailed guide to the Engagement Series, including how the Fall Carnival booth works and how to use the "freshman advantage" as a natural recruiting conversation
- A behind-the-scenes look at how events are planned, supplied, and coordinated at the staff level by Sra. Michaelson

---

## How It Benefits the Organization

- **Reduces onboarding time.** New leaders arrive at their first training already familiar with the events, the purpose behind each activity, and what's expected of them.
- **Improves recruiting.** The public section gives undecided students a clear, honest picture of what Link Crew involves, which tends to attract applicants who are genuinely prepared to commit.
- **Preserves institutional knowledge.** Built from the direct experience of a former Link Crew Commissioner, the site captures event structures and leadership insights that would otherwise exist only in memory and need to be re-explained each year.
- **Scales without extra effort.** Once updated with current application details and the annual passcode, the site runs itself. No print materials, no repeated presentations for new cohorts.
- **Reusable year over year.** The structure and content are designed to stay accurate across cycles. Only the application details and passcode need updating each year.

---

## Technical Details

| Detail | Value |
|---|---|
| File type | Single-file HTML |
| Dependencies | None — fully self-contained |
| Fonts | Google Fonts (Playfair Display, Inter, Space Mono) via CDN |
| Logo | Base64-encoded PNG, embedded directly in the file |
| Passcode gate | Client-side JavaScript — current passcode is `KNIGHTS` |
| Interactive demo | Canvas-based JavaScript animation (Ball Juggling Game) |
| Hosting | GitHub Pages (static, no server required) |
| Browser support | All modern browsers |

### Updating the Passcode
Open `index.html` in any text editor and search for `KNIGHTS`. Replace it with the new code. The gate checks against this value client-side, so no backend is needed.

### Updating Application Details
Search for `Application details coming soon` and replace with the current cycle's dates and instructions.

### Swapping in Photos
Every photo placeholder is labeled with a comment in the HTML (e.g., `📸 Photo: Orientation Day games`). Replace the `div` with an `img` tag pointing to your photo file, or embed it as a base64 data URI the same way the logo is handled.

---

## Project Notes

Built by Kaeden, former Link Crew Commissioner at Arizona College Prep, as a training and recruitment resource for the ACP Knights Link Crew chapter. Content is based on direct experience running Orientation Day and the Engagement Series.

See the AI disclosure at the bottom of the site for details on how this project was created.
