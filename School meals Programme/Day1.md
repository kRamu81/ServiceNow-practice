# Day 1 — Environment Setup & App Scaffolding
### Full Setup Notes — App Engine Studio Only 
---

## Part 1 — Get a Free ServiceNow Developer Instance

1. Go to **developer.servicenow.com**
2. Click **Sign up** (top right) and create a free account with your email.
3. Once logged in, go to your dashboard and click **Request Instance** (or **Manage → Instance**).
4. Choose the **latest general availability release** — avoid "early access" or preview releases, they can be unstable for a first build.
5. Wait 3–8 minutes while ServiceNow provisions your personal instance, something like:
   ```
   https://devXXXXX.service-now.com
   ```
6. Save these somewhere safe (password manager or a local notes file):
   - Your **instance URL**
   - Your **admin username** (usually `admin`)
   - Your **password** (shown once — write it down immediately)

> ⚠️ **Important:** Developer instances go to sleep after a few hours of inactivity, or after several idle days. If your instance stops loading later in the week, go back to the Developer portal and click **Wake up instance**, then wait a few minutes.

**Checkpoint:** You can open your instance URL in a browser and log in with your admin username and password.

---

## Part 2 — Open App Engine Studio

1. Log into your instance.
2. In the top navigation bar, click the **search icon** (magnifying glass) or the **All** menu.
3. Type **App Engine Studio** and click it.
4. This opens the Studio home — a visual dashboard for building apps without writing code (though you can add scripts later if you want to).

**Checkpoint:** You're looking at the App Engine Studio home page, which shows a list of apps (probably empty right now) and a **Create Application** or **+ New** button.

---

## Part 3 — Create Your App

1. Click **Create Application** (or **+ New App**).
2. You'll usually be asked to choose a starting point — choose **Create from scratch** (not a template), since we're building something specific.
3. Fill in the app details:
   - **Name:** `School Meals Programme`
   - **Description:** `Digitizes delivery verification, quality inspection, and complaint handling for the National School Meals Programme`
   - **Scope / Application ID:** Studio will usually auto-generate this from the name, something like `x_yourinstance_school_meals_programme`. You can leave the auto-generated one — you don't need to memorize it, just know it exists.
   - **Icon/Color (optional):** Pick anything — this is just cosmetic and won't affect functionality.
4. Click **Create** (or **Submit** / **Finish**, depending on your release version).
5. Wait a few seconds — Studio will provision the empty app shell.

**Checkpoint:** You land inside your new app's workspace in App Engine Studio, with the app name **School Meals Programme** shown at the top.

---

## Part 4 — Get Familiar With the Studio Layout

You don't need to build anything yet — just find these areas, since you'll use them constantly this week:

| Area | What it's for | You'll use it on |
|---|---|---|
| **Data (Tables)** | Where you create and edit tables — Kitchen, Delivery, Inspection, etc. | Day 2 |
| **Experiences / UI Builder / Service Portal** | Where you build the forms people actually fill in (delivery form, complaint form) | Day 3, Day 6 |
| **Process Automation / Flow Designer** | Where you build the automatic rules and alerts | Day 5 |
| **Roles & Security** | Controls who can see/edit what | Skim today, revisit if needed |
| **App Manager (top-level, outside Studio)** | Where you can see your app listed among all apps on the instance, activate/deactivate it, check version | Good to know exists, rarely used day-to-day |

Click into **Data** now just to see the (currently empty) table list — don't create anything yet, that's tomorrow.

**Checkpoint:** You can navigate to the Data/Tables section and the Experiences section inside your app without getting lost.

---

## Part 5 — Confirm Your App Is Real and Saved

1. Leave App Engine Studio and go to the main ServiceNow navigation.
2. In the search bar, type **System Applications → My Company Applications** (or simply search **"Application Manager"**).
3. Find **School Meals Programme** in the list.
4. Confirm it shows as **Active**.

This proves the app isn't just sitting half-created in Studio — it's properly registered on your instance.

**Checkpoint (this is your Day 1 milestone):** Your app appears in both App Engine Studio and the Application Manager, and shows as Active.
---

## End-of-Day 1 Checklist

- [ ] Free ServiceNow developer instance created and I can log in
- [ ] App Engine Studio opened successfully
- [ ] New app "School Meals Programme" created from scratch
- [ ] I can navigate to the Data/Tables section inside my app
- [ ] I can navigate to the Experiences/Service Portal section inside my app
- [ ] App confirmed as **Active** in Application Manager

