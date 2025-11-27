# Meeting Time Converter ⏰🌍

A super-simple GitHub Actions tool that instantly converts your meeting time into **major cities worldwide** — perfect for scheduling international calls without doing time-zone math!

No installation · No dependencies · Just click and run.

### Live Demo
Just go to the **Actions** tab and run it:
→ https://github.com/kangwonlee/timezone-table/actions/workflows/meeting-time.yml

### How to Use

1. Click on the **Actions** tab
2. In the left sidebar, select **Meeting Time Converter**
3. Click the blue button **Run workflow** (top-right)
4. Fill in the form:
   - **Year** – e.g. `2025`
   - **Month** – `1` to `12`
   - **Day** – `1` to `31`
   - **Hour** – `0`–`23` (24-hour format)
   - **Minute** – `0`–`59`
   - **Timezone** – IANA name of the original time (default: `Europe/Paris`)
     Common examples:
     `Europe/Paris`, `Europe/London`, `America/New_York`, `America/Los_Angeles`, `Asia/Tokyo`, `Asia/Dubai`, etc.
   - **Duration** – meeting length in minutes (default: `60`)

5. Click the green **Run workflow** button (may take about 15 seconds)

The result appears immediately in the workflow run summary as a beautiful Markdown table:

| City         | Local Time          | Time Zone |
|--------------|---------------------|-----------|
| San Diego    | 05:00 – 06:00       | PST       |
| Chicago      | 07:00 – 08:00       | CST       |
| New York     | 08:00 – 09:00       | EST       |
| London       | 13:00 – 14:00       | GMT       |
| Paris        | 14:00 – 15:00       | CET       |
| Berlin       | 14:00 – 15:00       | CET       |
| New Delhi    | 18:30 – 19:30       | IST       |
| Sydney       | 00:00 – 01:00       | AEDT      |
| Dubai        | 17:00 – 18:00       | GST       |

You can copy-paste the table directly into Slack, Notion, emails, etc.

### Tech

- Python + built-in `zoneinfo` (no pytz, no bugs)
- Powered by [**uv**](https://github.com/astral-sh/uv) – the fastest Python tool on earth
- Pure GitHub Actions – zero setup

Just fork, star, or reuse in your own team/org repo!

Made with ❤️ for distributed teams.

(Got help from Grok on this one)
