# Prompt Engineering System for Website Sections

## Table of Contents
1. [Master Meta-Prompt](#master-meta-prompt)
2. [Section-Specific Prompts](#section-specific-prompts)
3. [Usage Instructions](#usage-instructions)
4. [Expected Outputs](#expected-outputs)

---

## Master Meta-Prompt

Use this as a foundation for generating any website section with consistent quality and styling.

```
You are an expert frontend developer specializing in modern, responsive web design. Create a [SECTION_NAME] component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Primary (#6366f1 - Indigo), Secondary (#0ea5e9 - Sky Blue), Neutral Grays
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Minimalist, professional, with subtle animations

**Technical Requirements:**
- Use semantic HTML5 elements
- Implement with Tailwind CSS utility classes (CDN version)
- Ensure full mobile responsiveness (mobile-first approach)
- Include smooth hover effects and transitions
- Add proper spacing and alignment
- Use flexbox/grid for layouts
- Ensure accessibility (ARIA labels, semantic structure)

**Responsive Breakpoints:**
- Mobile: < 640px (single column, stacked elements)
- Tablet: 640px - 1024px (optimized spacing)
- Desktop: > 1024px (full layout)

**Code Quality Standards:**
- Clean, well-indented code
- Descriptive class names
- Comments for major sections
- No inline styles (use Tailwind utilities)
- Include necessary CDN links

**Visual Requirements:**
- Consistent spacing (use Tailwind spacing scale)
- Proper contrast ratios for accessibility
- Smooth animations (use transition utilities)
- Professional color harmony
- Clear visual hierarchy

Now, create the [SECTION_NAME] with these specific requirements:
[INSERT SECTION-SPECIFIC REQUIREMENTS HERE]

Provide complete, production-ready HTML code with embedded Tailwind CSS CDN.
```

---

## Section-Specific Prompts

### 1. Navigation Bar Prompt

```
You are an expert frontend developer specializing in modern, responsive web design. Create a Navigation Bar component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Primary (#6366f1 - Indigo), Secondary (#0ea5e9 - Sky Blue), Neutral Grays
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Minimalist, professional, with subtle animations

**Technical Requirements:**
- Use semantic HTML5 <nav> element
- Implement with Tailwind CSS utility classes (include CDN in <head>)
- Ensure full mobile responsiveness with hamburger menu
- Include smooth hover effects and transitions
- Sticky navigation on scroll (use sticky positioning)
- Use flexbox for layout
- Ensure accessibility (ARIA labels for mobile menu)

**Navigation Elements:**
1. Logo/Brand Name: "TaskFlow" (left side)
   - Use bold, slightly larger text
   - Add hover effect (color change)

2. Desktop Menu Items (center/right):
   - Features
   - Pricing
   - About
   - Contact
   - Each link should have hover underline animation

3. CTA Button (right side):
   - Text: "Get Started"
   - Primary indigo background
   - White text
   - Rounded corners
   - Hover effect (slightly darker shade)

4. Mobile Menu:
   - Hamburger icon (3 horizontal lines) for screens < 768px
   - Sliding menu from right or dropdown from top
   - Smooth animation
   - Close icon (X) when menu is open
   - Overlay/backdrop when menu is open

**Layout Specifications:**
- Desktop: Logo left, menu center, CTA right
- Mobile: Logo left, hamburger icon right
- Height: 64px (h-16)
- Background: White with subtle shadow
- Padding: Consistent horizontal padding

**Responsive Breakpoints:**
- Mobile (< 768px): Show hamburger menu
- Desktop (>= 768px): Show full horizontal menu

**Interactive Features:**
- Hamburger menu toggles mobile menu
- Links change color on hover
- CTA button has hover and active states
- Smooth transitions (duration-300)

**Code Requirements:**
- Include complete HTML with <!DOCTYPE html>
- Include Tailwind CSS CDN in <head>
- Add basic JavaScript for mobile menu toggle
- Use data attributes for JS targeting
- Well-commented code

Provide complete, production-ready code that I can copy and paste directly into an HTML file.
```

---

### 2. Hero Section Prompt

```
You are an expert frontend developer specializing in modern, responsive web design. Create a Hero Section component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Primary (#6366f1 - Indigo), Secondary (#0ea5e9 - Sky Blue), Neutral Grays
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Minimalist, professional, with gradient background

**Technical Requirements:**
- Use semantic HTML5 <section> element
- Implement with Tailwind CSS utility classes
- Ensure full mobile responsiveness
- Include smooth animations on load
- Use flexbox/grid for layout
- Ensure accessibility (proper heading hierarchy)

**Hero Content:**
1. Main Headline:
   - Text: "Streamline Your Workflow with TaskFlow"
   - Large, bold text (text-5xl on desktop, text-3xl on mobile)
   - Dark text color
   - Fade-in animation

2. Subheading/Description:
   - Text: "The all-in-one platform to manage tasks, collaborate with teams, and boost productivity. Simple, powerful, and built for modern teams."
   - Medium gray text
   - text-xl on desktop, text-lg on mobile
   - Max width for readability

3. Call-to-Action Buttons:
   - Primary Button: "Start Free Trial"
     - Indigo background, white text
     - Larger size (px-8 py-4)
     - Rounded corners
     - Hover effect (shadow + slight scale)
   
   - Secondary Button: "Watch Demo"
     - Transparent with indigo border
     - Indigo text
     - Hover effect (background fill)

4. Hero Image/Illustration:
   - Right side on desktop
   - Below content on mobile
   - Use placeholder from Unsplash (dashboard/workspace theme)
   - URL: https://images.unsplash.com/photo-1551434678-e076c223a692?w=800
   - Rounded corners with shadow
   - Fade-in animation

**Layout Specifications:**
- Desktop: Two-column layout (60% content, 40% image)
- Mobile: Single column (content stacked above image)
- Vertical centering
- Large top and bottom padding (py-20 on desktop, py-12 on mobile)
- Background: Subtle gradient (from indigo-50 to white)

**Visual Effects:**
- Fade-in animation for text (stagger delays)
- Slide-in from left for content
- Slide-in from right for image
- Buttons have scale effect on hover
- Add decorative gradient blob/shape in background (optional)

**Responsive Breakpoints:**
- Mobile (< 768px): Stack vertically, center text
- Tablet (768px - 1024px): Adjust spacing
- Desktop (> 1024px): Two-column side-by-side

**Code Requirements:**
- Include complete HTML structure
- Include Tailwind CSS CDN
- Add subtle CSS animations
- Use proper semantic HTML
- Include image with alt text
- Well-commented code sections

Provide complete, production-ready code that creates a visually stunning, modern hero section.
```

---

### 3. Services/Features Section Prompt

```
You are an expert frontend developer specializing in modern, responsive web design. Create a Services/Features Section component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Primary (#6366f1 - Indigo), Secondary (#0ea5e9 - Sky Blue), Neutral Grays
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Card-based layout with icons

**Technical Requirements:**
- Use semantic HTML5 <section> element
- Implement with Tailwind CSS utility classes
- Ensure full mobile responsiveness
- Include hover effects on cards
- Use CSS Grid for layout
- Ensure accessibility (proper ARIA labels)

**Section Structure:**
1. Section Header:
   - Small label: "Features" (uppercase, indigo color, small text)
   - Main heading: "Everything you need to stay productive"
   - text-4xl on desktop, text-3xl on mobile
   - Subheading: "Powerful features designed to help your team work smarter, not harder."
   - Center-aligned
   - Generous spacing below (mb-16)

2. Feature Cards (6 items):
   Each card should have:
   - Icon (use Heroicons from CDN or simple SVG shapes)
   - Feature title (text-xl, bold)
   - Description (2-3 lines, gray text)
   - White background with shadow
   - Rounded corners
   - Padding: p-6
   - Hover effect: lift up slightly + increased shadow

   Features to include:
   a) **Task Management**
      - Icon: Checklist/clipboard
      - Description: "Create, organize, and track tasks with intuitive boards and lists"
   
   b) **Team Collaboration**
      - Icon: Users/people
      - Description: "Work together seamlessly with real-time updates and comments"
   
   c) **Time Tracking**
      - Icon: Clock/timer
      - Description: "Monitor time spent on tasks and optimize your workflow"
   
   d) **File Sharing**
      - Icon: Cloud/upload
      - Description: "Share documents and files securely with your team"
   
   e) **Analytics & Reports**
      - Icon: Chart/graph
      - Description: "Get insights with detailed analytics and progress reports"
   
   f) **Integrations**
      - Icon: Puzzle piece/link
      - Description: "Connect with your favorite tools and automate workflows"

**Layout Specifications:**
- Desktop: 3 columns (grid-cols-3)
- Tablet: 2 columns (grid-cols-2)
- Mobile: 1 column (grid-cols-1)
- Gap between cards: gap-8
- Container max width: max-w-7xl
- Background: Light gray (bg-gray-50)
- Section padding: py-20 on desktop, py-12 on mobile

**Card Design:**
- Background: White (bg-white)
- Shadow: shadow-md (hover: shadow-xl)
- Border radius: rounded-xl
- Transition: smooth transform and shadow
- Icon color: Indigo gradient
- Icon size: 48x48px or w-12 h-12

**Visual Effects:**
- Cards lift on hover (transform -translate-y-2)
- Shadow increases on hover
- Icons can have subtle animation
- Staggered fade-in on scroll (optional)

**Responsive Breakpoints:**
- Mobile (< 640px): 1 column
- Tablet (640px - 1024px): 2 columns
- Desktop (> 1024px): 3 columns

**Icon Implementation:**
Use simple SVG icons or Heroicons. For simplicity, use these Unicode symbols as placeholders:
- Task: ✓ or 📋
- Team: 👥
- Time: ⏰
- Files: 📁
- Analytics: 📊
- Integrations: 🔗

Or implement proper SVG icons in a circle with indigo background.

**Code Requirements:**
- Include complete HTML structure
- Include Tailwind CSS CDN
- Use CSS Grid for responsive layout
- Add hover transition effects
- Well-structured, semantic HTML
- Comments for each feature card

Provide complete, production-ready code for a modern, professional features section.
```

---

### 4. Contact/Lead Form Prompt

```
You are an expert frontend developer specializing in modern, responsive web design. Create a Contact/Lead Form component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Primary (#6366f1 - Indigo), Secondary (#0ea5e9 - Sky Blue), Neutral Grays
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Clean form with modern input styling

**Technical Requirements:**
- Use semantic HTML5 <form> element
- Implement with Tailwind CSS utility classes
- Ensure full mobile responsiveness
- Include basic HTML5 validation attributes
- Use flexbox for layout
- Ensure accessibility (proper labels, ARIA attributes)

**Section Structure:**
1. Section Header:
   - Small label: "Contact Us" (uppercase, indigo color)
   - Main heading: "Get Started Today"
   - text-4xl on desktop, text-3xl on mobile
   - Subheading: "Fill out the form below and our team will get back to you within 24 hours."
   - Center-aligned

2. Form Container:
   - Two-column layout on desktop
   - Left column: Form fields
   - Right column: Contact info/image
   - Background: White card with shadow
   - Max width: max-w-6xl
   - Centered on page

**Form Fields (Left Column):**
1. Full Name
   - Type: text
   - Required: yes
   - Placeholder: "John Doe"
   - Full width

2. Email Address
   - Type: email
   - Required: yes
   - Placeholder: "john@example.com"
   - Validation: HTML5 email pattern

3. Company Name
   - Type: text
   - Required: no
   - Placeholder: "Your Company"

4. Phone Number
   - Type: tel
   - Required: no
   - Placeholder: "+1 (555) 000-0000"

5. How did you hear about us?
   - Type: select dropdown
   - Options: "Select an option", "Search Engine", "Social Media", "Friend/Referral", "Advertisement", "Other"
   - Required: yes

6. Message
   - Type: textarea
   - Required: yes
   - Placeholder: "Tell us about your project..."
   - Rows: 5

7. Submit Button
   - Text: "Send Message"
   - Full width on mobile, auto width on desktop
   - Indigo background, white text
   - Large padding (px-8 py-4)
   - Rounded corners
   - Hover effect (darker shade + shadow)
   - Disabled state (gray, cursor not-allowed)

**Input Field Styling:**
- Border: 1px solid gray-300
- Rounded corners: rounded-lg
- Padding: px-4 py-3
- Focus state: indigo border + ring
- Placeholder: gray-400
- Transition: smooth border color change
- Full width: w-full
- Margin bottom: mb-4

**Label Styling:**
- Font weight: medium (font-medium)
- Color: gray-700
- Margin bottom: mb-2
- Small size: text-sm

**Contact Info Section (Right Column):**
Desktop only, hidden on mobile

Content:
- Icon + Email: contact@taskflow.com
- Icon + Phone: +1 (555) 123-4567
- Icon + Address: 123 Business St, San Francisco, CA 94105

Or use an illustration from Unsplash:
https://images.unsplash.com/photo-1423666639041-f56000c27a9a?w=600

**Layout Specifications:**
- Desktop: Two columns (grid-cols-2, gap-12)
- Mobile: Single column (form only)
- Container padding: p-8
- Background: Light gradient or solid white
- Section padding: py-20 on desktop, py-12 on mobile

**Validation Structure:**
- All required fields have `required` attribute
- Email field has `type="email"`
- Phone field has `type="tel"`
- Form has `novalidate` to allow custom styling of validation errors
- Add basic client-side validation feedback (red border on invalid)

**Responsive Breakpoints:**
- Mobile (< 768px): Stack form only, full width inputs
- Desktop (>= 768px): Two-column layout

**Visual Effects:**
- Input focus: border color change + subtle shadow
- Button hover: background darkens + shadow
- Smooth transitions on all interactive elements

**Code Requirements:**
- Include complete HTML structure
- Include Tailwind CSS CDN
- Form has proper action attribute (can be "#" for demo)
- Include basic JavaScript for form validation styling
- Accessible labels and ARIA attributes
- Well-commented code

Provide complete, production-ready code for a professional contact form.
```

---

### 5. Footer Prompt

```
You are an expert frontend developer specializing in modern, responsive web design. Create a Footer component with the following specifications:

**Design Context:**
- Theme: Modern SaaS/Tech Startup
- Color Scheme: Dark background (gray-900), white text, indigo accents
- Typography: Clean, modern sans-serif (use system fonts)
- Style: Multi-column layout with clear organization

**Technical Requirements:**
- Use semantic HTML5 <footer> element
- Implement with Tailwind CSS utility classes
- Ensure full mobile responsiveness
- Include hover effects on links
- Use flexbox/grid for layout
- Ensure accessibility (proper link labels)

**Footer Structure:**

1. Main Footer Content (4 Columns):
   
   **Column 1: Brand & Description**
   - Logo/Brand: "TaskFlow"
   - Brief description: "Streamline your workflow and boost productivity with our all-in-one task management platform."
   - Color: gray-400
   - Max width for readability

   **Column 2: Product Links**
   - Heading: "Product" (text-white, font-semibold, mb-4)
   - Links:
     - Features
     - Pricing
     - Integrations
     - Changelog
     - API Docs
   
   **Column 3: Company Links**
   - Heading: "Company" (text-white, font-semibold, mb-4)
   - Links:
     - About Us
     - Careers
     - Blog
     - Press Kit
     - Contact
   
   **Column 4: Legal Links**
   - Heading: "Legal" (text-white, font-semibold, mb-4)
   - Links:
     - Privacy Policy
     - Terms of Service
     - Cookie Policy
     - GDPR
     - Security

2. Social Media Icons (Below main content):
   - Platforms: Twitter, LinkedIn, GitHub, Facebook
   - Icons: Use simple SVG or Unicode symbols
   - Style: Circle with border, hover effect (fill indigo)
   - Size: 40x40px
   - Spacing: gap-4
   - Horizontal layout

3. Bottom Bar:
   - Copyright: "© 2024 TaskFlow. All rights reserved."
   - Small text (text-sm)
   - Gray color (text-gray-500)
   - Center-aligned on mobile, left-aligned on desktop

**Layout Specifications:**
- Desktop: 4 columns (grid-cols-4)
- Tablet: 2 columns (grid-cols-2)
- Mobile: 1 column (grid-cols-1)
- Background: Dark (bg-gray-900)
- Text color: White and gray shades
- Padding: py-12 on desktop, py-8 on mobile
- Max width container: max-w-7xl

**Link Styling:**
- Color: gray-400
- Hover: white (text-white)
- Transition: smooth color change (transition-colors duration-300)
- Display: block
- Margin: mb-3

**Column Spacing:**
- Gap between columns: gap-8
- Bottom margin on headings: mb-4
- Bottom margin on links: mb-3

**Responsive Breakpoints:**
- Mobile (< 640px): 1 column, centered text
- Tablet (640px - 1024px): 2 columns
- Desktop (> 1024px): 4 columns

**Social Icons:**
Use simple Unicode or SVG:
- Twitter: 𝕏 or Twitter SVG
- LinkedIn: in
- GitHub: GitHub logo
- Facebook: f

Or create circular divs with icon text inside.

**Visual Effects:**
- Links change color on hover
- Social icons fill with indigo on hover
- Smooth transitions (duration-200)

**Border/Divider:**
- Thin border at top: border-t border-gray-800
- Optional divider between main content and bottom bar

**Code Requirements:**
- Include complete HTML structure
- Include Tailwind CSS CDN
- Use semantic footer element
- Grid for responsive columns
- Proper link structure (href="#" for demo)
- Well-commented sections

Provide complete, production-ready code for a professional, modern footer.
```

---

## Usage Instructions

### How to Use These Prompts:

1. **For Meta-Prompt:**
   - Copy the Master Meta-Prompt
   - Replace `[SECTION_NAME]` with the section you're building
   - Replace `[INSERT SECTION-SPECIFIC REQUIREMENTS HERE]` with details from the individual prompts
   - Use with any AI coding tool (ChatGPT, Claude, Gemini)

2. **For Individual Prompts:**
   - Copy the complete prompt for the section you want to generate
   - Paste it directly into your AI tool
   - The AI will generate complete, production-ready HTML code
   - Copy the output and save as separate HTML files

3. **Iterating on Outputs:**
   - If the output isn't perfect, add specific feedback
   - Example: "Make the buttons larger and add more rounded corners"
   - Example: "Increase spacing between cards"
   - Example: "Make the mobile menu slide from the right instead of dropdown"

4. **Combining Sections:**
   - Generate each section separately
   - Copy the `<body>` content from each
   - Combine into one HTML file
   - Keep only one set of `<head>` tags (with CDN links)

---

## Expected Outputs

### Quality Standards:

Each generated section should have:

✅ **Clean HTML Structure:**
- Semantic HTML5 elements
- Proper nesting and indentation
- Descriptive class names

✅ **Responsive Design:**
- Mobile-first approach
- Works on all screen sizes
- Proper breakpoints

✅ **Professional Styling:**
- Consistent color scheme
- Proper spacing and alignment
- Modern visual effects

✅ **Accessibility:**
- Proper ARIA labels
- Semantic structure
- Keyboard navigation support

✅ **Performance:**
- Minimal dependencies (just Tailwind CDN)
- No external files needed
- Fast loading

### File Structure:

When generating, you'll create:
```
project/
├── 01-navigation.html
├── 02-hero.html
├── 03-features.html
├── 04-contact.html
├── 05-footer.html
└── index.html (combined final page)
```

---

## Prompt Engineering Best Practices

### Why These Prompts Work:

1. **Detailed Context**: Every prompt includes complete design context
2. **Specific Requirements**: Clear technical and visual specifications
3. **Consistent Theming**: All sections use the same color scheme and style
4. **Responsive by Default**: Mobile-first approach built into every prompt
5. **Reusability**: Can be used with any AI tool, any time
6. **Structured Format**: Easy to modify and customize

### Tips for Success:

- Always copy the COMPLETE prompt (don't truncate)
- Test prompts with different AI tools to ensure consistency
- If output isn't perfect, add specific refinement requests
- Keep the color scheme and style consistent across sections
- Generate one section at a time for best results

---

**Ready to generate your website sections!**

Use these prompts with Claude, ChatGPT, or any AI coding tool to create professional, responsive website components.