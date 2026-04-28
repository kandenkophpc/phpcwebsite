# Refactor: Remove Unused CSS/JS and Centralize Common Code

## Issues
- [x] Topbar, Header, Footer duplicated across ~20 HTML files
- [x] Two nearly identical CSS files (style.css & style1.css), both with 300+ lines of unused rules
- [x] Unused vendor libraries loaded on every page (FontAwesome, glightbox, isotope-layout)
- [x] main.js initializes all plugins unconditionally

## Plan

### Phase 1: Create Shared Components System
- [ ] Create `assets/js/components.js` — shared Topbar/Header/Footer injector

### Phase 2: Consolidate & Clean CSS
- [ ] Merge `style.css` + `style1.css` into one `style.css`
- [ ] Add `.hero-short` class for pages needing 50vh hero
- [ ] Remove ~300+ lines of unused CSS rules
- [ ] Delete `
