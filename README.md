# Mitho & Mool — Admin Dashboard

A responsive, custom-built admin dashboard interface for **Mitho & Mool**, designed specifically to manage inventory, batches, customer orders, and shop announcements. 

This project was built strictly using **CSS Grid** to achieve high layout precision, zero global window scrollbars, and independent vertical scrolling panels.

---

## 🎨 Visual Identity & Palette

The dashboard design reflects an earthy, warm aesthetic tailored to handcrafted nepali sweets (*Pustakari*) and postpartum traditional nutrient mixes (*Sutkeri Aushadhi*):

* **Primary Dark (`#3D2314`):** Rich roasted brown used for sidebar backgrounds and heavy headings.
* **Secondary Base (`#E0A32A`):** Warm gold accent used for borders, hover states, and active highlights.
* **Tertiary Light / Base (`#FAF7F2` / `#F3EFE6`):** Soft cream tones used for card backgrounds and main content regions.
* **Typography:** `Fraunces` (Headings) paired with `Plus Jakarta Sans` (Body text).

---

## 🛠️ Key Technical Features & Constraints

* **Strict Grid-Only Layout:** Built entirely without Flexbox or external framework dependencies to master advanced CSS Grid alignment, track placement, and nested sub-grids.
* **Fixed Viewport Architecture (`100vh`):** Locks the main layout to the screen window, preventing whole-page browser scrollbars while allowing card regions to scroll internally (`overflow-y: auto`).
* **Controlled Grid Tracks:**
  * **Body:** Split into `28rem 1fr` columns for sidebar and workspace.
  * **Workspace Grid:** Multi-column layout (`3fr 3fr 2.2fr`) balancing product card width with a dedicated side panel track.
* **Uniform Card Sizing:** Utilizes `grid-auto-rows: 1fr`, explicit `min-height`, and paragraph clamping to prevent variable content length from distorting card dimensions.
* **Visual Polish:**
  * 5px left accent borders (`#7A3E21`) on product cards with smooth hover elevation (`translateY(-3px)`).
  * Palette-tinted box shadows (`rgba(61, 35, 20, 0.25)`) for depth.
  * Item separators across announcement and trending side panels.

---

## 📁 Project Structure

```text
mitho-and-mool-dashboard/
├── index.html          # Main dashboard markup
├── style.css           # Pure CSS Grid layout & custom properties
├── images/             # Vector icons & branding graphics
│   ├── logo.svg
│   ├── header-icons/
│   └── sidebar-icons/
└── README.md