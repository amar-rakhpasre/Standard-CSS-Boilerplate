
# 🌐 Web Accessibility & UI/UX Standards  

This document provides **comprehensive guidelines** for building **accessible, performant, and SEO-friendly web applications**.  
It covers **WCAG 2.1 standards**, **GIGW 3.0 (India Govt guidelines)**, **SEO**, and **UI/UX performance practices**.  

---

## 📑 Table of Contents  

1. [Introduction](#introduction)  
2. [WCAG Accessibility Standards](#wcag-accessibility-standards)  
   - [Contrast Ratios](#contrast-ratios)  
   - [Levels (A, AA, AAA)](#levels-a-aa-aaa)  
   - [Examples](#examples)  
   - [Resources](#resources)  
3. [GIGW Guidelines (India)](#gigw-guidelines-india)  
4. [Accessibility Checklist](#accessibility-checklist)  
5. [SEO Best Practices](#seo-best-practices)  
6. [Performance Best Practices](#performance-best-practices)  
7. [Developer Actions](#developer-actions)  
8. [Testing & Evaluation](#testing--evaluation)  
9. [Resources & Tools](#resources--tools)  

---

## 📌 Introduction  

Modern web design must follow **international accessibility standards** and **national guidelines**.  
- **WCAG 2.1** – Global accessibility standards.  
- **GIGW 3.0** – Indian Government guidelines (aligned with WCAG, IS 17802).  
- **SEO** – Ensures search engine visibility.  
- **Performance** – Improves UX & Core Web Vitals.  

---

## ♿ WCAG Accessibility Standards  

### 🎯 Contrast Ratios  

| Element | WCAG AA | WCAG AAA |
|---------|---------|----------|
| **Normal text** (<18px, <14px bold) | **4.5:1** | **7:1** |
| **Large text** (≥18px or ≥14px bold) | **3:1** | **4.5:1** |
| **UI elements (icons, borders, focus)** | **3:1** | **4.5:1** |

📌 Contrast ratio = difference between foreground & background color.  

---

### 🎯 Levels (A, AA, AAA)  

- **Level A (Basic):**  
  - Minimum compliance.  
  - E.g., must support keyboard navigation.  

- **Level AA (Industry Standard):**  
  - Widely adopted, required for most organizations.  
  - E.g., text contrast 4.5:1, semantic headings, focus visible.  

- **Level AAA (Strictest):**  
  - Maximum accessibility (not always mandatory).  
  - E.g., text contrast 7:1, sign language for videos.  

---

### 🖼 Examples  

✅ Example 1 – Passing AA but failing AAA:  

```css
/* Background: #516FDF (blue), Text: #FFFFFF */
contrast-ratio: 5.64:1; 
Passes AA ✅ 
Fails AAA ❌
```

✅ Example 2 – Passing AAA:  

```css
/* Background: #121212, Text: #F1F1F1 */
contrast-ratio: 12.8:1; 
Passes AAA ✅
```

---

### 🔗 Resources  

- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)  
- [W3C WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)  
- [Colorable Contrast Tool](https://colorable.jxnblk.com/)  

---

## 🇮🇳 GIGW Guidelines (India)  

- First introduced in **2009 by NIC**.  
- **GIGW 3.0** aligns with **WCAG 2.1 (Level AA)**, **IS 17802**, **cybersecurity**, **AI analytics**.  

**Aim:**  
- Make government websites/apps:  
  - **User-friendly**  
  - **Consistent**  
  - **Secure**  
  - **Accessible**  

📌 While **mandatory for govt sites**, **private companies & startups** should adopt these for **better UX & inclusivity**.  

---

## ✅ Accessibility Checklist  

- [ ] Semantic HTML (use `<h1>–<h6>`, `<nav>`, `<main>`, `<footer>`)  
- [ ] Keyboard navigation (`tab`, `enter`, `esc`)  
- [ ] Focus visible styles (`:focus-visible`)  
- [ ] ARIA labels for non-text elements  
- [ ] Form fields have `<label>` (not just placeholder)  
- [ ] Alt text for all images  
- [ ] Captions for video/audio  
- [ ] Sufficient color contrast (AA or AAA)  
- [ ] Skip navigation link  
- [ ] Responsive, scalable text  

---

## 🔍 SEO Best Practices  

- ✅ Semantic HTML (use `<header>`, `<article>`, `<section>`).  
- ✅ One `<h1>` per page (descriptive).  
- ✅ Meta titles & descriptions.  
- ✅ Alt text for images.  
- ✅ Meaningful anchor text (`Read More` ❌ → `Read More About HR Infotech` ✅).  
- ✅ Use structured data (schema.org).  
- ✅ Optimize Core Web Vitals (LCP, FID, CLS).  

---

## ⚡ Performance Best Practices  

- ✅ Use modern image formats (WebP, AVIF).  
- ✅ Minify & bundle CSS/JS.  
- ✅ Use lazy-loading (`loading="lazy"` for images/iframes).  
- ✅ Implement caching & CDN.  
- ✅ Reduce unused CSS/JS.  
- ✅ Prefer `prefetch`, `preload`, `dns-prefetch`.  
- ✅ Avoid layout shifts (CLS).  

---

## 👨‍💻 Developer Actions  

- Build reusable **design tokens** (colors, spacing, typography).  
- Test with **screen readers** (NVDA, VoiceOver).  
- Ensure **keyboard access** for modals, dropdowns, menus.  
- Follow **progressive enhancement** (core functionality works without JS).  
- Implement **theme switching** (light/dark, high contrast).  

---

## 🧪 Testing & Evaluation  

- **Manual Testing**  
  - Navigate entire site with only keyboard.  
  - Zoom text to 200% (check readability).  
  - Check contrast with WebAIM.  

- **Automated Tools**  
  - [axe DevTools](https://www.deque.com/axe/)  
  - [Lighthouse](https://developers.google.com/web/tools/lighthouse)  
  - [WAVE Tool](https://wave.webaim.org/)  

---

## 📚 Resources & Tools  

- [W3C WCAG 2.1 Quick Reference](https://www.w3.org/WAI/WCAG21/quickref/)  
- [GIGW 3.0 Guidelines (NIC)](https://guidelines.india.gov.in/)  
- [WebAIM](https://webaim.org/)  
- [MDN Web Docs – Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility)  
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)  

---

## 📌 Summary  

- **AA compliance = must-have**  
- **AAA compliance = best practice**  
- **GIGW = govt-mandated, but useful for everyone**  
- **Performance + SEO + Accessibility = Better UX**  
