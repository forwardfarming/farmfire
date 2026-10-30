# 🔥 FarmFire

A map-based fire safety app for farms.

- **Map** your fire hazards (fuel, chemicals, straw stacks, LPG…), water sources (hydrants, pumps, tanks, ponds, bowsers) and safety points (assembly point, shut-offs, gates).
- **Choose who sees what** – each item can be shown to your employees, neighbouring farms and/or the fire service.
- **REPORT FIRE button** – alerts every farm within **2 miles** and lets you tick what help you need (water bowser, hydrant, tractor & plough for a firebreak, extra people…). Neighbours can reply with what they can bring.
- **Safety plan** for employees – procedure, contacts, assembly point, plus a list of water sources with directions.
- **Equipment log** – hydrants, extinguishers etc. with last test and expiry dates, colour-coded overdue / due soon / OK, and CSV export.
- **Fire service view** – sees everything farms have shared with the fire service, plus live alerts.

> ⚠️ Always call **999** first. This app alerts neighbours – it does not call the fire service.

---

## Trying the demo

Use the **"View as"** menu at the top to switch between being the owner of a farm, an employee, or the fire service.

To test an alert:
1. View as **Owner – Manor Farm**, press **REPORT FIRE**, tick some help and send.
2. Switch to **Owner – Hill Top Farm** – you'll see the red alert banner and can press **Offer help**.
3. Switch back to Manor Farm and open **Alerts** to see the reply.

Tip: open the app in **two browser tabs**, set one to Manor Farm and one to Hill Top Farm – alerts appear in the other tab straight away.

### What this version can and can't do
This is a **working prototype**. Everything is saved in the browser on the device you're using, so:
- Alerts only reach other "farms" inside the same browser – not real phones yet.
- Data isn't shared between devices.

To make it live for real farms, the next step is adding a backend (e.g. **Supabase** or **Firebase**) for user accounts, shared data, and push/SMS notifications so alerts reach neighbours' phones.

---

## Putting it on GitHub (first time)

### 1. Create an account
Go to **github.com** and sign up (free).

### 2. Create a repository (a project folder)
1. Click the **+** in the top right → **New repository**.
2. Name it, e.g. `farmfire`.
3. Choose **Public** (needed for free hosting – only the code is public, not anyone's farm data).
4. Tick **Add a README file**, then click **Create repository**.

### 3. Upload the files
1. In your new repository, click **Add file** → **Upload files**.
2. Drag in `index.html` and `README.md` (replace the README if asked).
3. At the bottom, type a short note like "First version" and click **Commit changes**.

### 4. Turn it into a website (GitHub Pages)
1. Go to **Settings** (top of your repository) → **Pages** (left menu).
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Set branch to **main** and folder to **/ (root)**, then **Save**.
4. Wait 1–2 minutes and refresh – a link appears like  
   `https://YOUR-USERNAME.github.io/farmfire/`

Open that link on your phone. You can add it to your home screen (Share → Add to Home Screen on iPhone, or ⋮ → Add to Home screen on Android) so it opens like an app.

### Making changes later
Click `index.html` in your repository → the ✏️ pencil icon → edit → **Commit changes**. The website updates within a minute or two.

---

## Tech
Single file: `index.html` (HTML, CSS, JavaScript). Map by [Leaflet](https://leafletjs.com), satellite imagery from Esri, street map from OpenStreetMap.
