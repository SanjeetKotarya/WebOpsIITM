# Designing WebOps IITM: A Digital Identity for an Engineering Club

**Role:** Product Designer & Developer  
**Duration:** ~3-4 weeks (part-time)  
**Tools:** HTML5, CSS3, JavaScript, WebGL  
**Year:** 2023

---

## Introduction

As a Super Coordinator of the WebOps club at IIT Madras, I noticed a critical gap: our club, focused on web operations and development, had no digital presence. While we were actively building websites for other campus organizations, we lacked our own platform to showcase our work, recruit members, and establish our identity.

This case study documents my journey of designing and building the WebOps IITM website from scratch—a project that went beyond just creating a website. It became an exercise in understanding how to communicate a technical community's value proposition, create an engaging user experience, and design a platform that would serve both current members and prospective recruits.

---

## The Challenge

### Problem Statement

The WebOps club needed a website that could:

1. **Establish digital presence** - Showcase the club's identity and mission to the IIT Madras community
2. **Recruit members** - Attract students passionate about web development and operations
3. **Showcase work** - Display projects we've built for various campus organizations
4. **Provide information** - Make it easy for people to learn about the club and contact us
5. **Reflect our expertise** - Since we're a web-focused club, the website itself needed to demonstrate technical and design capabilities

### Constraints & Context

- **Limited resources:** As a student-led initiative, this was a solo project I took on voluntarily
- **Time constraints:** Needed to be completed while balancing academic responsibilities
- **Target audience:** Primarily IIT Madras students, but also potential external collaborators
- **Technical requirements:** Should work seamlessly across devices (desktop, tablet, mobile)
- **Performance:** Needed to load quickly even on slower campus networks

---

## Research & Discovery

### Understanding the Audience

Before diving into design, I spent time understanding who would visit this website:

**Primary Users:**
- **Prospective members:** Students curious about joining, especially first-year students during recruitment season
- **Current members:** Reference point and portfolio showcase
- **Campus organizations:** Potential clients looking for web development services
- **External visitors:** Alumni, potential collaborators, or curious web developers

**User Needs:**
- Quick understanding of what the club does
- Easy access to project examples
- Simple way to contact or join
- Professional appearance that builds trust

### Competitive Analysis

I analyzed similar club and organization websites to understand common patterns:

- **Tech club websites:** Often overwhelming with too much information
- **Portfolio sites:** Sometimes focus too much on aesthetics over usability
- **Corporate sites:** Too formal for a student club context

**Key Insight:** The sweet spot was a balance—professional enough to build credibility, but approachable enough to feel like a student community.

---

## Design Process

### Phase 1: Information Architecture

I mapped out the core content structure:

```
WebOps IITM Website
├── Hero Section (First Impression)
│   ├── Club introduction
│   ├── Key value proposition
│   └── Primary CTA
├── About Us
│   └── Mission and purpose
├── What We Offer
│   └── Services and opportunities
├── Projects Portfolio
│   └── Showcase of work
├── Team
│   └── Meet the members
├── Contact
│   └── Get in touch / Join form
└── Footer
    └── Links and copyright
```

**Decision Rationale:** A linear, scrollable layout made sense because:
- Users naturally scroll on the web
- It tells a story from introduction to action
- Easy to navigate without complex menus
- Mobile-friendly by default

### Phase 2: Visual Design System

#### Color Palette

I chose a dark theme with purple accents for several reasons:

**Primary Colors:**
- **Dark backgrounds (#121212, #000000):** Modern, reduces eye strain, stands out from typical light websites
- **Purple accent (#4D16BE):** Vibrant, tech-forward, creates strong brand recognition
- **White/Light gray:** Excellent contrast for readability

**Why this palette:**
- Dark themes are popular in developer communities—signals we understand our audience
- Purple suggests creativity and innovation
- High contrast ensures accessibility and readability
- Professional yet distinctive

#### Typography

**Font Selection:**
- **Poppins (body text):** Modern, highly readable, friendly yet professional
- **Josefin Sans (headings):** Geometric, impactful, creates clear hierarchy

**Typography Scale:**
- H1: 40-50px (section titles)
- H2: 20-25px (subheadings)
- Body: 14-18px (readable without being too small)

**Decision:** Sans-serif fonts feel modern and tech-appropriate. The two-font system creates clear visual hierarchy without feeling cluttered.

#### Spacing & Layout

- **Consistent border-radius:** 15px, 25px, and 50px (pill shapes)
- **Generous whitespace:** Prevents information overload
- **Container widths:** 70-90% on desktop (doesn't feel stretched on large screens)
- **Card-based design:** Easy to scan and understand at a glance

### Phase 3: Key Design Decisions

#### 1. Fixed Navigation with Glassmorphism Effect

**What I did:** Created a fixed navigation bar that stays visible while scrolling, with a dark background and subtle hover effects.

**Why:** 
- Always accessible navigation improves UX
- The pill-shaped design with border creates a modern "floating" effect
- Stays out of the way but easily accessible

**Design detail:** Added a box-shadow on hover that creates depth, giving users visual feedback that it's interactive.

#### 2. Hero Section with Split Layout

**What I did:** Divided the hero into 30% text content and 60% visual element (video background on desktop, abstract graphic).

**Why:**
- Large visuals immediately communicate what the club is about
- Text content is scannable without overwhelming
- Creates visual interest that encourages scrolling

**Challenge:** Finding the right balance between visual impact and page load performance. Solved by using optimized video formats and providing fallbacks.

#### 3. Interactive Project Showcase

**What I did:** Created a horizontal scrolling section for projects with cards that have hover effects (expanding colored "bulb" backgrounds).

**Why:**
- Horizontal scroll is unexpected and engaging—shows we're not afraid to experiment
- Cards provide clear visual separation between projects
- Hover effects make it feel interactive and modern
- Embedded screenshots let users preview projects immediately

**Design challenge:** Making it clear the section is scrollable. I solved this by:
- Using partial visibility of adjacent cards
- Smooth scrolling behavior
- Visual indicators through the design itself

#### 4. 3D Card Flip Animation for Team Section

**What I did:** Implemented CSS 3D transforms so team member cards flip on hover to reveal detailed information.

**Why:**
- Creates an "aha" moment—users discover information through interaction
- Efficiently uses space (information is hidden until needed)
- Showcases technical capability in an elegant way
- Makes team section more engaging than typical static cards

**Consideration:** I ensured the flip animation is smooth and not jarring, using CSS transitions for 0.6s duration.

#### 5. Neumorphic Contact Form

**What I did:** Designed input fields with soft shadows that create an embossed/debossed effect (neumorphism).

**Why:**
- Modern design trend that shows awareness of current design movements
- Creates tactile, interactive feeling
- Differentiates the form from typical flat designs
- Purple accent on icons maintains brand consistency

**UX detail:** Input fields have clear focus states—background turns white when active, making it obvious which field is selected.

#### 6. Application Page with WebGL Fluid Simulation

**What I did:** Built a full-page interactive canvas where users can interact with a fluid simulation powered by WebGL.

**Why:**
- Demonstrates advanced technical capabilities
- Creates memorable, "wow factor" experience
- Shows we can work with cutting-edge web technologies
- Differentiates us from typical club websites

**Technical challenge:** Ensuring performance across devices. Implemented:
- Texture downsampling for lower-end devices
- Efficient shader programs
- Performance monitoring

---

## User Experience Decisions

### Navigation Flow

I designed the site as a single-page application with smooth scrolling because:

1. **Reduces friction:** No page reloads, faster navigation
2. **Tells a story:** Linear flow from introduction to call-to-action
3. **Mobile-friendly:** Single page works better on mobile than multi-page navigation
4. **SEO benefits:** All content is immediately accessible

### Call-to-Action Strategy

I placed multiple CTAs strategically:

- **Hero section:** "Contact Us" button (immediate action for curious visitors)
- **Navigation:** "Join Us" button (always accessible)
- **About section:** "Join Us" button (after understanding the club)
- **Contact section:** Direct contact form (lower commitment action)

**Rationale:** Different users are ready to engage at different points. Multiple CTAs ensure no one falls through the cracks.

### Mobile-First Responsive Design

**Breakpoint Strategy:**
- Desktop: Full experience with all visual effects
- Mobile (max-width: 768px): Simplified navigation, stacked layouts, optimized images

**Key Adaptations:**
- Navigation becomes hamburger menu
- Split layouts become single column
- Font sizes adjust for readability
- Touch targets enlarged (minimum 44px)
- Video background replaced with static image on very small screens

**Why this matters:** Most students browse on mobile. A great mobile experience was non-negotiable.

---

## Technical Implementation Highlights

### Component-Based Architecture

I structured the site with separate HTML/JS files for each section:

```
index.html (main entry)
├── nav.html/js (navigation)
├── intro.html/js (hero)
├── about.html/js (about section)
├── wwd.html/js (what we offer)
├── project.html/js (projects)
├── team.html/js (team)
├── contact.html/js (contact)
└── footer.html/js (footer)
```

**Benefits:**
- Easy to maintain and update individual sections
- Modular approach allows for future expansion
- Clean separation of concerns

### Performance Optimizations

1. **Lazy loading:** Sections load asynchronously (though could be improved further)
2. **Optimized assets:** Compressed images, efficient video formats
3. **Minimal dependencies:** Vanilla JavaScript, no heavy frameworks
4. **CSS efficiency:** Inline styles per component (could be optimized into separate files)

### Accessibility Considerations

**What I implemented:**
- Semantic HTML structure
- Keyboard navigation support
- Smooth scroll behavior
- Responsive design for all screen sizes
- Clear focus states

**Areas for improvement (acknowledged):**
- ARIA labels for interactive elements
- More explicit color contrast validation
- Alt text for all images
- Screen reader optimization

---

## Challenges & Solutions

### Challenge 1: Creating a Memorable First Impression

**Problem:** How do we stand out among dozens of club websites on campus?

**Solution:** Combined multiple visual techniques:
- Abstract 3D graphics in hero section
- Video background (autoplay, muted)
- Statistics overlay for credibility
- Large, bold typography

**Result:** Visitors immediately understand this isn't a typical club website.

### Challenge 2: Showcasing Projects Without Overwhelming

**Problem:** We have multiple projects but wanted to showcase them without creating a cluttered layout.

**Solution:** Horizontal scrolling cards with:
- Numbered system (.01, .02, etc.) for easy reference
- Embedded screenshots for instant preview
- Consistent card design that's scannable
- "Visit Website" CTAs on each card

**Result:** Users can quickly browse projects while maintaining focus.

### Challenge 3: Making Team Section Engaging

**Problem:** Team sections are often boring—just photos and names.

**Solution:** 3D card flip interaction:
- Hover reveals detailed information (roll number, phone, projects)
- Maintains visual interest
- Efficiently uses space
- Shows technical sophistication

**Result:** Team section became one of the most interactive parts of the site.

### Challenge 4: Balancing Aesthetics with Performance

**Problem:** Rich visuals (video, WebGL) could slow down the site.

**Solution:** 
- Optimized video formats and compression
- Conditional loading (WebGL only on application page)
- Efficient CSS animations (using transforms, not layout properties)
- Progressive enhancement approach

**Result:** Site loads quickly even on slower connections while maintaining visual quality.

---

## User Testing & Iterations

### Initial Feedback

I showed the website to:
- Current club members
- Friends from other departments
- First-year students (target audience)

**Key Feedback:**
- "The dark theme is cool but is it too dark?" → Kept it, it differentiates us
- "Can you add more project details?" → Added embedded screenshots
- "The team cards are really cool!" → Validated the 3D flip interaction
- "How do I join?" → Made CTAs more prominent

### Iterations Based on Feedback

1. **Enhanced CTAs:** Made "Join Us" buttons more visible with stronger borders
2. **Added project screenshots:** Visual previews helped users understand our work better
3. **Improved mobile menu:** Refined hamburger menu animation for smoother experience
4. **Contact form enhancements:** Added neumorphic design to make form more engaging

---

## Results & Impact

### Quantitative Metrics

- **Website launched:** Successfully deployed and accessible to entire IIT Madras community
- **Projects showcased:** 5 major projects displayed with links
- **Team members featured:** 13 team members (2 Core, 3 Super Coordinators, 8 Coordinators)
- **Page performance:** Fast load times even with rich media content
- **Responsive design:** Works seamlessly across all device sizes

### Qualitative Impact

**For the Club:**
- Established professional digital presence
- Provided central hub for recruitment
- Showcased technical capabilities effectively
- Created pride and ownership among members

**For Users:**
- Easy way to learn about the club
- Quick access to project portfolio
- Simple contact/join process
- Memorable user experience

**Personal Impact:**
- Validated ability to work on full-stack design projects
- Gained experience in user-centered design thinking
- Built confidence in both design and development skills
- Created portfolio piece demonstrating range of capabilities

---

## Design System Documentation

### Color Tokens

```
Primary Brand Color: #4D16BE (Purple)
Dark Background: #121212, #000000, #0E161B
Light Background: #FFFFFF, #E8E8E8, #F5F5F5
Text Colors: #000000, #FFFFFF, #A5B2C0
Border Colors: #1B2328, #4D16BE
```

### Component Patterns

**Buttons:**
- Primary: Black background, white text, purple border on hover
- Secondary: White background, black text, purple border
- CTAs: Large, prominent, rounded corners (25px radius)

**Cards:**
- White background (or dark in projects section)
- Subtle shadow for depth
- Rounded corners (15px)
- Hover states for interactivity

**Navigation:**
- Fixed position
- Pill-shaped container (50px radius)
- Dark background with light text
- Smooth transitions

---

## Lessons Learned

### What Went Well

1. **Component-based approach:** Made development and updates much easier
2. **Strong visual identity:** Consistent color and typography created cohesive experience
3. **Interactive elements:** Engagement was higher than expected, especially team section
4. **Mobile-first thinking:** Ensured site works well for primary audience

### What I'd Do Differently

1. **Accessibility from start:** Would build in ARIA labels and screen reader support from the beginning
2. **Design system documentation:** Would create more formal design tokens upfront
3. **User research:** Would conduct more structured interviews before designing
4. **Performance monitoring:** Would implement analytics earlier to track real usage
5. **Progressive enhancement:** Would design for no-JS fallback from the start

### Key Takeaways

- **Balance matters:** Professional yet approachable, modern yet accessible, impressive yet performant
- **Details make a difference:** Small animations and interactions significantly improve perceived quality
- **Know your audience:** Understanding that most visitors are students on mobile influenced many decisions
- **Technical and design go hand-in-hand:** Being able to implement designs myself allowed for more creative freedom

---

## Future Improvements

### Short-Term Enhancements

1. **Accessibility audit:** Add ARIA labels, improve color contrast, enhance keyboard navigation
2. **Form backend:** Replace mailto: with proper backend service for contact form
3. **Loading states:** Add spinners/loading indicators for async content
4. **Complete application form:** Finish the "Coming Soon" application page

### Medium-Term Enhancements

1. **CMS integration:** Allow non-technical members to update content
2. **Blog section:** Share club updates, tutorials, project stories
3. **Member portal:** Dashboard for current members
4. **Project case studies:** Detailed pages for each project

### Long-Term Vision

1. **Interactive project demos:** Embedded live demos of projects
2. **Member contributions:** Showcase individual member portfolios
3. **Recruitment portal:** Streamlined application and interview process
4. **Analytics dashboard:** Track engagement and optimize based on data

---

## Reflection

Building the WebOps IITM website was more than a design project—it was an opportunity to apply design thinking to a real problem. As someone interested in product design, this project taught me:

**About Design:**
- The importance of understanding your audience before designing
- How visual design communicates values and personality
- The balance between aesthetics and usability
- How small interactions can significantly impact user experience

**About Process:**
- The value of iteration and feedback
- Importance of considering technical constraints early
- How modular thinking helps both design and development
- The need to balance ambition with practicality

**About Product Thinking:**
- How to identify core problems and user needs
- The importance of multiple CTAs for different user journeys
- How every design decision should have rationale
- The value of creating documentation and systems

This project demonstrated my ability to take a project from problem identification through research, design, development, and launch. It showcases not just design skills, but also technical capability, project management, and user-centered thinking.

---

## Conclusion

The WebOps IITM website successfully achieved its goals: establishing a digital presence, showcasing the club's work, and creating an engaging platform for recruitment. More importantly, it became a case study in thoughtful design—every decision, from color palette to interaction patterns, was made with the user and the club's goals in mind.

As I continue to grow as a product designer, this project serves as a reminder of what's possible when you combine user empathy, design principles, and technical execution. It's a foundation I'm excited to build upon as I tackle more complex design challenges in my career.

**The website is live at:** https://sanjeetkotarya.github.io/WebOpsIITM/

---

*This case study reflects the design process and decisions behind the WebOps IITM website. All design work, research, and development was done independently as part of my role as Super Coordinator of the WebOps club at IIT Madras.*

