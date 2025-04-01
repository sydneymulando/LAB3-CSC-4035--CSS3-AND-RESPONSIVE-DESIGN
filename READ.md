                       PAGE DESCRIPTIONS


index.html (Home Page)

Description: The home page serves as the primary landing page for "WebPro Solutions," introducing visitors to the brand and its offerings. It features a professional hero section with a bold headline ("Professional Web Solutions"), a subtitle, and a call-to-action button linking to the Services page. Below, a two-column Flexbox layout presents an "About Us" section alongside a sidebar highlighting key benefits ("Why Choose Us"). The page is topped with a sticky navigation bar and ends with a simple footer.
Purpose: Welcomes users, establishes credibility, and encourages exploration of services.

services.html (Services Page)

Description: This page showcases the core services offered by WebPro Solutions, presented in a responsive CSS Grid layout. It includes four service cards (Web Design, Development, SEO, and Support), each with an image, heading, and brief description. The cards feature hover effects for interactivity. The page maintains the consistent sticky navigation bar and footer, with a centered heading ("Our Services") introducing the content.
Purpose: Highlights the company’s expertise and service offerings in a visually appealing, easy-to-scan format.

contact.html (Contact Page)

Description: The contact page provides a user-friendly interface for visitors to reach out to WebPro Solutions. It features a centered, responsive form with fields for name, email, subject, and message, styled with HTML5 validation and subtle focus animations. A prominent "Get in Touch" heading and a styled submit button with hover effects enhance usability. The page includes the shared sticky navigation bar and footer for consistency.
Purpose: Facilitates communication, encouraging inquiries or feedback in a professional manner.                       




              A BRIEF SUMMARY OF THE KEY FEATURES USED IN THE PROJECT

##Selectors

#Universal Selector (*): Resets box-sizing, margin, and padding for all elements to ensure consistent layout calculations.

#Element Selectors: Styles basic HTML elements like body, h1, h2, h3, p, a, main, header, and footer for consistent typography and structure.

#Class Selectors: Targets specific components like .navbar, .nav-links, .hero, .service-card, .contact-form, etc., for page-specific styling.

#Pseudo-Class Selectors: Uses :hover (e.g., a:hover, .service-card:hover) and :focus (e.g., .form-group input:focus) for interactive states, and .active for navigation highlighting.

#Attribute Selectors: Styles input[type="text"], input[type="email"] for form fields with specific types.

#Child and Descendant Selectors:
     # Examples like .form-group label and .service-card h2 target nested elements for precise control.


Media Queries (Responsive Design)

3 Breakpoints (as required):

#max-width: 1024px: Adjusts font sizes, hero heading, service grid column width, and flex container spacing for large tablets/small laptops.

#max-width: 768px: Switches navbar to a column layout, stacks home page flex content vertically, reduces service grid column size, and tweaks padding/margins for tablets.

#max-width: 480px: Further simplifies layout for mobile phones with a single-column service grid, centered navbar links stacked vertically, and reduced padding/font sizes.
Purpose: Ensures the site adapts smoothly across devices, enhancing usability and readability.


Flexbox and Grid

Flexbox:

#Navigation (.navbar): Uses display: flex with justify-content: space-between to align the logo and nav links horizontally (switches to column on smaller screens).
Nav Links (.nav-links): display: flex arranges links side-by-side, stacking vertically on mobile.
Home Content (.home-content-wrapper): display: flex creates a side-by-side layout for intro and sidebar, with flex: 3 and flex: 1 for proportional sizing (stacks on tablets).
Body Layout: body uses display: flex with flex-direction: column and min-height: 100vh to push the footer to the bottom, with main using flex-grow: 1.


Grid:

Services (.services-grid): display: grid with grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)) creates a responsive grid of service cards that adjusts column count based on screen width (down to 1fr on mobile).
##Animation Features


Transitions:

Applied to links (a), buttons (.cta-button, .submit-button), form fields (.form-group input), and service cards (.service-card) using transition for smooth changes in properties like color, background-color, border-color, transform, and box-shadow over --transition-speed (0.3s).
Examples: Hover effects on links/buttons, focus effects on form fields, and card elevation on hover.


Keyframes:
@keyframes fadeIn: Animates opacity from 0 to 1, used on the .hero section for a fade-in effect over 1.5s.
@keyframes slideInDown: Animates h1 elements from a 30px upward offset with opacity 0 to their final position with opacity 1 over 0.8s, adding a subtle entrance effect.