
PROJECT: Role-Based Access Control Interface (Pixel-Perfect Implementation)
Assessment ID: Dev_Specs_UI

ABOUT THE PROJECT
This codebase delivers a pixel-perfect, interactive implementation of the "Maintain Role Level Access Control" administration dashboard. Built exactly to the provided UI specification, it gives administrators a comprehensive view to search, audit, and modify field-level restrictions across different business lines (like NRI or Corporate banking) and specific request workflows (e.g., Address Updates or Stop Payment checks).


TECHNOLOGY STACK
To ensure maximum speed, lightweight portability, and compliance with the constraints, this project uses zero external dependencies:
- Structure : HTML5 (Semantic elements)
- Styles    : Native CSS3 (utilizing Flexbox & Grid layouts)
- Logic     : Modern Vanilla JavaScript (ES6+)
- Iconography: Native Unicode HTML Entities (No external icon packages required)
- Typography : System font stack (Segoe UI / Arial)

* No build tools, compilers, npm installs, or node_modules folders are required.



FOLDER ARCHITECTURE

output/
  ├── index.html       → The entire application layout, styles, and logic.
  └── ReadMe.txt       → This documentation file.


DIRECTIONS TO RUN
1. Unzip the archive if it is compressed.
2. Navigate into the "output" directory.
3. Open "index.html" directly inside any modern web browser (Chrome, Edge, or Firefox).

* Note: This application is completely self-contained and runs purely client-side without needing a local development web server.


DESIGN & BREAKPOINT SPECIFICATIONS
- Layout Grid     : 3-column responsive layout for form fields via CSS Grid.
- Mobile Adaptability: Drops down to a single column layout at a 768px width breakpoint.
- Left Navigation : Fixed width of 48px.
- Top Navbar      : Fixed height of 44px with sticky viewport positioning.
- Component Padding: 18px top/bottom, 20px left/right.
- Core Font Size  : 13px base.
- Custom Palette  :
    • Deep Indigo (Headers/Nav) -> #1a3a6e
    • Interactive Blue (Buttons) -> #2563c7
    • Muted Text                 -> #6b7a93
    • Dark Carbon (Body Text)    -> #333333
    • Border Lines               -> #dde2ea
    • Light Gray Background      -> #f0f2f5
    • Alert/Delete Crimson       -> #e0423a
    • Status Badges              -> Custom tint pairs matching NRI, Corporate, and Red warnings.


CORE KEY FEATURES
1. Persistent sidebar navigation with active status highlights.
2. Clean breadcrumb trail navigation showing current system location.
3. Search panel showcasing:
   - Dynamic interactive keyword filter for User Roles.
   - Access Control dropdown filter defaulting to "Field Level".
   - Multi-chip display UI for quick-removing selected Case Categories and Sub-categories.
   - Instant UI reset functionality via the Clear button.
4. Data Table display:
   - Contains 10 mocked rows strictly following the initial design layout.
   - Dynamic status badges with custom text colors.
   - Formatted monospace string masking (e.g., XXXX XXXX) mapping to secure attributes.
   - Actionable triggers for row deletion and record updates.
5. In-app interactive Toast alerting engine.
6. Inline JavaScript native browser prompt to confirm asset removal.



ENGINEERING NOTES
- The table utilizes predefined mock datasets designed to mirror the physical specification screens.
- In a production ecosystem, the search handler would process an async fetch request to a server endpoint and return this structure dynamically.
