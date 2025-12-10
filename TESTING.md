# iCook Website — Manual Testing Documentation

**Live site:** [https://hannagreentree.github.io/icook/](https://hannagreentree.github.io/icook/)  
**Test date:** 2025-11-13  
**Browsers tested:** Google Chrome, Microsoft Edge, Safari (iPhone)  
**Devices tested:** Desktop (1920px), Laptop (1366px), Tablet (768px), Mobile (375px)

---

## 1️⃣ Functionality Testing

| # | Feature / Link | Location | Test Action | Expected Result | Actual Result | Pass/Fail | Notes |
|---:|----------------|---------|-------------|-----------------|---------------|----------:|-------|
| 1 | Home | Top navigation | Click | Scroll to top / Home section | Works | ✅ Pass | Logo also returns to top |
| 2 | Menu | Top navigation | Click | Scrolls to Menu section | Works | ✅ Pass | Menu items visible |
| 3 | About | Top navigation | Click | Scrolls to About section | Works | ✅ Pass | Text & image load correctly |
| 4 | Contact | Top navigation | Click | Scrolls to Contact section | Works | ✅ Pass | Contact form visible |
| 5 | iCook Logo | Header / Top-left | Click | Scrolls to top / Home | Works | ✅ Pass | Standard UX behavior |
| 6 | Each Menu Item | Menu Section | Visual check | Items display correctly | Works | ✅ Pass | No broken links |
| 7 | Contact Form | Contact section | Fill fields & submit | Fields accept input | Works | ✅ Pass | Submit button functional (static) |
| 8 | Facebook link | Footer | Click | Opens in new tab | Works | ✅ Pass | `target="_blank"` + `rel="noopener noreferrer"` |
| 9 | Instagram link | Footer | Click | Opens in new tab | Works | ✅ Pass | Same as above |
| 10 | X (Twitter) link | Footer | Click | Opens in new tab | Works | ✅ Pass | Same as above |
| 11 | Back to Top | Footer | Click | Scrolls to top | Works | ✅ Pass | Optional |
| 12 | Mobile Menu | Small viewport | Tap menu icon | Opens menu, links clickable | Works | ✅ Pass | Smooth responsive behavior |
| 13 | Images | All sections | Visual check | Images load & scale correctly | Works | ✅ Pass | Alt attributes present |
| 14 | Internal anchor links | Various | Click | Scroll to section | Works | ✅ Pass | IDs match href |

**Summary:** All functionality tests passed; external links open in new tabs and the contact form is usable.

---

## 2️⃣ Usability Testing

| # | Feature / Area | Test Description | Expected User Experience | Actual Result | Pass/Fail | Notes |
|---:|----------------|----------------|-------------------------|---------------|----------:|-------|
| 1 | Navigation Menu | Check visibility & use | Menu clearly labeled, links work | Works | ✅ Pass | Intuitive navigation |
| 2 | Logo | Click returns home | Top of page / Home section visible | Works | ✅ Pass | Helps user orientation |
| 3 | Hero Section | First impression | Users understand purpose | Works | ✅ Pass | Headline clear |
| 4 | Menu Section | Clarity of items | Items readable & organized | Works | ✅ Pass | Easy to read |
| 5 | About Section | Text readability & layout | Text readable, image complements text | Works | ✅ Pass | Professional look |
| 6 | Contact Form | Filling & submission | Fields visible & functional | Works | ✅ Pass | Easy to use |
| 7 | Social Media Links | Recognizable & clickable | Open in new tab, clear icons | Works | ✅ Pass | Meets expectation |
| 8 | Footer | Info & icons clear | Footer readable, aligned | Works | ✅ Pass | Consistent design |
| 9 | Text Readability | Fonts & contrast | Text readable | Works | ✅ Pass | Accessible colors |
| 10 | Button Visibility | Hover & active states | Buttons respond visually | Works | ✅ Pass | Confirms interactivity |
| 11 | Layout Consistency | Sections | Layout spacing consistent | Works | ✅ Pass | Professional appearance |
| 12 | Mobile Menu | Toggle on mobile | Menu opens & links clickable | Works | ✅ Pass | Responsive behavior smooth |
| 13 | Scrolling Behavior | Click anchors | Smooth scroll to section | Works | ✅ Pass | No broken anchors |
| 14 | Accessibility Check | Images & headings | Alt text present, heading order correct | Works | ✅ Pass | Meets basic accessibility |
| 15 | Error Handling | Form submission | Errors handled if fields incomplete | Works | ✅ Pass | Static form behavior acceptable |
| 16 | Overall Navigation Flow | User tasks | User finds info quickly | Works | ✅ Pass | Good UX |

**Summary:** Navigation, readability, and interactivity are clear and intuitive across all devices.

---

## 3️⃣ Responsiveness Testing

| Section / Feature | Device Tested | Expected Behaviour | Actual Result | Pass/Fail |
|-------------------|---------------|------------------|---------------|-----------|
| Navigation Bar | Mobile 320–425px | Collapses or adjusts layout | Works | ✅ Pass |
| Hero Section | All | Image scales, text visible | Works | ✅ Pass |
| About Section | Tablet & Mobile | Text wraps, image adjusts | Works | ✅ Pass |
| Menu Section | Mobile | Columns stack properly | Works | ✅ Pass |
| Contact Section | Mobile | Form fields readable & aligned | Works | ✅ Pass |
| Footer | Mobile | Text & icons scale correctly | Works | ✅ Pass |
| Social Media Icons | All | Visible & clickable | Works | ✅ Pass |
| Images/Videos | All | No stretching or overflow | Works | ✅ Pass |

**Devices Tested:**  
- iPhone 13 (Safari) ✅  
- Samsung Galaxy S21 (Chrome) ✅  
- iPad (Safari) ✅  
- Windows Laptop (Edge, Chrome) ✅  
- MacBook Air (Safari) ✅  

**Summary:** iCook is fully responsive; layout, text, and images adjust correctly across all devices.

---

## 4️⃣ Internal Links Testing

| # | Link Text | Location | Target / Href | Test Action | Expected Result | Actual Result | Pass/Fail |
|---:|-----------|---------|---------------|-------------|----------------|---------------|-----------|
| 1 | Home | Top navigation | `index.html` | Click | Scroll to top / Home | Works | ✅ Pass |
| 2 | Menu | Top navigation | `#menu` | Click | Scrolls to Menu section | Works | ✅ Pass |
| 3 | About | Top navigation | `#about` | Click | Scrolls to About section | Works | ✅ Pass |
| 4 | Contact | Top navigation | `#contact` | Click | Scrolls to Contact section | Works | ✅ Pass |
| 5 | iCook Logo | Header | `index.html` | Click | Scrolls to top | Works | ✅ Pass |
| 6 | Back to Top | Footer | `#top` | Click | Scrolls to top | Works | ✅ Pass |
| 7 | Menu Item Anchors | Menu section | `#item-id` | Click | Scrolls to correct item | Works | ✅ Pass |

**Summary:** All internal links function correctly with smooth scrolling; no broken anchors or 404 errors detected.

---

## 5️⃣ Bugs Found, Fixes, and Outstanding Issues

| # | Bug / Issue | Location | How Found | Fix / Resolution | Status |
|---:|------------|---------|------------|-----------------|--------|
| 1 | External social links did not open in new tab | Footer | Clicked Facebook/Instagram/X links | Added `target="_blank"` and `rel="noopener noreferrer"` | ✅ Fixed |
| 2 | Mobile navigation menu initially overlapped content | Mobile view | Opened menu on small screens | Adjusted CSS to ensure menu displays above content | ✅ Fixed |
| 3 | Contact form fields misaligned on very small screens (<375px) | Contact section | Resized browser | Added CSS padding/margin adjustments | ✅ Fixed |
| 4 | Smooth scrolling not working in some browsers | Anchor links (Menu, About, Contact) | Clicked nav links | Added `scroll-behavior: smooth;` in CSS | ✅ Fixed |
| 5 | Some images lacked alt text | Menu, About sections | Manual inspection | Added descriptive `alt` attributes | ✅ Fixed |
| 6 | Minor spacing inconsistencies between sections | Entire site | Visual inspection | Adjusted CSS margins/padding | ✅ Fixed |
| 7 | Contact form submission does not trigger server response | Contact section | Clicked Submit | Static form (no backend implemented) | ⚠ Unfixed (Not required) |

**Summary:** All critical and visual bugs were fixed; outstanding issue (static contact form) is documented but does not impact usability.

---


# Bug 1
| **Problem** | The background video on the Home/Contact page wasn’t playing on iPhone and most Android devices.
| **Cause**   | Mobile browsers block autoplay unless the video is muted and uses `playsinline`. 
| **Fix**     | Added `autoplay`, `muted`, `playsinline`, `loop` attributes.
| **Status** |  ✅ Fixed   


<!-- Fix for mobile video autoplay behavior (solution from MDN docs) -->
<video autoplay muted loop playsinline class="background-video">


# Bug 2
| **Problem** | On mobile view, when the user clicked a menu item, the menu stayed open.
| **Cause**   | JavaScript did not remove the active class after clicking.
| **Fix**     | Added a small JS function to close it. 
| **Status**  | ✅ Fixed                                                               

// Close mobile menu after clicking a link (pattern inspired by W3Schools mobile nav menu)

document.querySelectorAll("nav a").forEach(link => {
  link.addEventListener("click", () => {
    document.querySelector(".menu").classList.remove("active");
  });
});

# Bug 3                                           
| **Problem** | Icons appeared too large or shifted on smaller screens. 
| **Cause**   | No responsive size constraints.   
| **Fix**     | Added max-width and responsive font-size.  
| **Status**  | ✅ Fixed 

# Bug 4
| **Problem** | Some recipe images stretched vertically.               
| **Cause**   | Missing `object-fit: cover`.                           
| **Fix**     | Added `object-fit: cover; width: 100%; height: 100%;`. 
| **Status**  | ✅ Fixed                                                

# Bug 5 
| **Problem** | Safari added extra padding to input fields. 
| **Cause**   | Default browser styles.                     
| **Fix**     | Added CSS reset for form inputs.            
| **Status**  | ✅ Fixed                                    








