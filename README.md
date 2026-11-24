# Multi-Specialty Hospital Website

A single-file, responsive, production-ready website template for a multi-specialty hospital. Designed to feel calm, trustworthy, and accessible within seconds, built with semantic HTML, modern CSS, and vanilla JavaScript—no frameworks or build steps required.

---

## Features

### Design & Accessibility
- **Muted Visual System**: High-trust palette built around ivory (`#F5F3EE`), deep spruce (`#1E3A3C`), and muted brass (`#7A663C`), reserving muted brick (`#7A2F2F`) strictly for emergency elements.
- **Dark Mode**: Matching deep teal-black dark theme that respects `prefers-color-scheme` with a manual toggle persisted via `localStorage` (wrapped in `try/catch`).
- **Typography & Readability**: Pairs `Cormorant Garamond` for headings with `Manrope` for body copy, maintaining WCAG AA contrast, sub-75-character line lengths, and built-in `A−` / `A+` text-size controls.
- **Accessible by Default**: Includes a skip-to-content link, semantic landmarks, `aria-live` announcements for form errors and results, 44px minimum touch targets, safe-area insets for mobile devices, and responsive layouts down to 360px.
- **ECG Canvas Hero**: A `devicePixelRatio`-aware HTML5 canvas rendering a quiet P-QRS-T heartbeat trace that falls back to a static frame when `prefers-reduced-motion` is enabled.

### Patient & Clinical Workflows
- **Sticky Emergency Strip**: Always-visible tap-to-call numbers at the top of the viewport.
- **Hospital Information Strip**: Quick-reference hours (Emergency, Outpatient, Visiting, Pharmacy/Lab), address, map placeholder, and parking/accessibility notes.
- **Searchable Departments & Doctor Filtering**: 8 core specialties (*Cardiology, Neurology, Orthopaedics, Obstetrics & Gynaecology, Paediatrics, Oncology, Nephrology, Emergency & Critical Care*) with live search that dynamically filters the doctor roster.
- **Interactive Appointment Booking (Demo)**:
  - Dependent Department → Doctor dropdowns (also pre-filled via "Book with Dr. X" buttons).
  - Date picker restricted to today through 60 days ahead, validating against each doctor's consulting days.
  - Time slot picker with pre-booked disabled states.
  - Inline plain-language validation, including 10-digit Indian mobile number checks (starting with 6–9).
  - Live "Your visit" summary panel, "Please bring" checklist, and confirmation screen with a generated reference code.
- **Health Information Tools**:
  - **BMI Calculator**: Uses WHO Asia-Pacific cut-offs (Healthy: `18.5–22.9`, Overweight: `≥ 23`, Obese: `≥ 25`) with a dynamic visual scale marker.
  - **Reference Ranges**: Standard baseline values for blood pressure, fasting glucose, HbA1c, LDL, and resting heart rate.
  - **Expandable Warning Signs**: Clear guidance for Stroke (BE-FAST), Heart Attack, and urgent signs in babies and children.
- **Emergency Contacts**: Large tap-to-call tiles for Indian emergency services (`112`, `108`, `102`, `14416` Tele-MANAS, `181`, `1098`), a slot for the hospital's emergency desk, and a "While you wait for help" first-aid panel.

---

## Design Tokens

| Role | Light Theme | Usage |
| :--- | :--- | :--- |
| Background | `#F5F3EE` | Page canvas (Ivory) |
| Surface | `#FCFBF8` | Cards and panels |
| Primary | `#1E3A3C` | Hero panel, primary actions (Deep Spruce) |
| Ink | `#172428` | Primary body and heading text |
| Muted Text | `#556466` | Secondary copy and metadata |
| Sage Tint | `#E4EAE5` | Subtle callouts and highlights |
| Hairline | `#DDD8CC` | Borders and dividers |
| Accent | `#7A663C` | ECG trace and sparing highlights (Brass) |
| Emergency | `#7A2F2F` | Emergency strip and urgent alerts only |

---

## Getting Started

Because the entire site is self-contained in a single file (`hospital-website.html`), no installation or build tools are needed.

### Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git
   cd <your-repo-name>
