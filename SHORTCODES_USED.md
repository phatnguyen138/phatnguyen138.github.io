# Blowfish Shortcodes Used in This Site

This document lists all the Blowfish theme shortcodes currently used across the site, along with examples and their locations.

---

## Overview

Blowfish provides powerful shortcodes to enhance your content with interactive and visually appealing components. This site uses several of these to improve readability and user experience.

---

## Shortcodes in Use

### 1. **Timeline** (`timeline` and `timelineItem`)

**Location:** `content/resume.md`

**Purpose:** Creates a visual timeline for displaying career progression and work experience.

**Example:**
```markdown
{{< timeline >}}

{{< timelineItem icon="briefcase" header="DevOps Engineer" badge="Oct 2025 – Present" subheader="KMS Technology | Ho Chi Minh City, Vietnam" >}}
<ul>
  <li>Achievement 1</li>
  <li>Achievement 2</li>
</ul>
{{< /timelineItem >}}

{{< /timeline >}}
```

**Parameters:**
- `icon`: Icon to display (e.g., "briefcase", "code", "terminal")
- `header`: Main title (job title)
- `badge`: Display badge (date range)
- `subheader`: Secondary information (company, location)

**Note:** Use HTML lists (`<ul><li>`) inside timeline items instead of markdown lists for proper rendering.

---

### 2. **Lead** (`lead`)

**Location:** `content/about.md`, `content/resume.md`

**Purpose:** Emphasizes introductory text or important statements, making them stand out visually.

**Example:**
```markdown
{{< lead >}}
I am a **DevOps Engineer**, passionate about building scalable cloud infrastructure.
{{< /lead >}}
```

---

### 3. **Keyword & KeywordList** (`keyword`, `keywordList`)

**Location:** `content/about.md`, `content/resume.md`

**Purpose:** Displays skills, technologies, and tools as styled badges/tags for better visual organization.

**Example:**
```markdown
{{< keywordList >}}
{{< keyword icon="cloud" >}}AWS{{< /keyword >}}
{{< keyword icon="code" >}}Python{{< /keyword >}}
{{< keyword icon="docker" >}}Docker{{< /keyword >}}
{{< /keywordList >}}
```

**Parameters:**
- `icon` (optional): Icon to display alongside the keyword

**Benefits:**
- Clean, organized display of technical skills
- Visual consistency across pages
- Easy to scan

---

### 4. **Button** (`button`)

**Location:** `content/about.md`, `content/resume.md`

**Purpose:** Creates styled clickable buttons for calls-to-action and important links.

**Example:**
```markdown
{{< button href="mailto:email@example.com" target="_blank" >}}
{{< icon "email" >}} Email Me
{{< /button >}}
```

**Parameters:**
- `href`: URL destination
- `target`: Link target (`_blank` for new tab, `_self` for same page)
- `rel` (optional): Relationship attribute

---

### 5. **Icon** (`icon`)

**Location:** `content/about.md`, `content/resume.md`

**Purpose:** Displays SVG icons inline with text, scales to match font size.

**Example:**
```markdown
{{< icon "github" >}}
{{< icon "cloud" >}}
{{< icon "terminal" >}}
```

**Common Icons Used:**
- `github`, `linkedin`, `email` - Social/contact
- `cloud` - Cloud platforms
- `code`, `terminal` - Programming/scripting
- `docker`, `dharmachakra` (Kubernetes) - Container tech
- `chart-line` - Monitoring tools
- `briefcase` - Professional experience
- `wrench` - Configuration tools

---

### 6. **Alert** (`alert`)

**Location:** `content/resume.md`

**Purpose:** Highlights important information or calls-to-action in a styled message box.

**Example:**
```markdown
{{< alert icon="envelope" >}}
**Open to opportunities!** Feel free to reach out for collaboration.
{{< /alert >}}
```

**Parameters:**
- `icon` (optional): Icon to display
- `iconColor` (optional): Custom icon color
- `cardColor` (optional): Custom background color
- `textColor` (optional): Custom text color

---

## Additional Useful Shortcodes (Not Yet Used)

### **Badge** (`badge`)
Simple styled badge for metadata display.

### **Gallery** (`gallery`)
Image gallery with lightbox functionality.

### **TypeIt** (`typeit`)
Animated typing effect for dynamic text.

### **Mermaid** (`mermaid`)
Render diagrams and flowcharts using Mermaid syntax.

### **Chart** (`chart`)
Display data visualizations using Chart.js.

---

## Best Practices

1. **HTML Lists in Shortcodes**: When using markdown lists inside shortcodes (like `timelineItem`), use HTML `<ul><li>` tags instead of markdown `-` syntax for proper rendering.

2. **Icons**: Always use semantic icons that match the content context (e.g., `briefcase` for jobs, `code` for programming).

3. **Consistency**: Use the same shortcodes across similar content types for a cohesive look.

4. **Accessibility**: Provide meaningful text with icons, don't rely solely on icons for communication.

5. **Button Usage**: Reserve buttons for primary actions (contact, download) to maintain their visual impact.

---

## Resources

- [Blowfish Shortcodes Documentation](https://blowfish.page/docs/shortcodes/)
- [Icon Reference](https://blowfish.page/samples/icons/)
- [Blowfish Theme GitHub](https://github.com/nunocoracao/blowfish)

---

*Last updated: January 2025*