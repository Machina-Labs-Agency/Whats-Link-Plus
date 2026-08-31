# Landing Page Design & Copywriting Documentation

## Overview

The "Whats Link+" landing page features a **Premium Dark Mode** aesthetic, designed to convey specific feelings of power, modernity, and speed. It heavily utilizes **Glassmorphism**, **Neon Accents** (primarily WhatsApp Green), and **Dynamic Micro-interactions** to create a high-conversion, trustworthy user experience.

---

## 1. Color System

### Primary Brand Colors

The core palette is built around the WhatsApp brand identity, enhanced for a dark theme ("Neon & Deep Dark").

| Variable | Hex Code | Usage |
| :--- | :--- | :--- |
| `--whatsapp-primary` | `#25d366` | Main action buttons, icons, highlights |
| `--whatsapp-glow` | `#00e676` | Hover states, blooming effects |
| `--whatsapp-dark` | `#128c7e` | Gradients, deeper backgrounds |
| `--whatsapp-deeper` | `#075e54` | Sticky bars, subtle borders |
| `--accent-red` | `#ff5252` | "Before" comparisons, error states, urgency |

### Neutral Palette (OLED Dark Mode)

A deep, neutral scale provides high contrast for the neon accents.

| Variable | Hex Code | Usage |
| :--- | :--- | :--- |
| `--neutral-950` | `#050505` | Deepest shadows, absolute black base |
| `--neutral-900` | `#0a0a0a` | **Main Page Background** |
| `--neutral-800` | `#121212` | Secondary Background (Cards, Sections) |
| `--neutral-700` | `#1f1f1f` | Card Backgrounds, Borders |
| `--neutral-600` | `#2d2d2d` | Input borders |
| `--neutral-400` | `#a3a3a3` | Subtext, inactive icons |
| `--white` | `#ffffff` | Primary Headings, Strong Text |

---

## 2. Typography

The typography system uses a tri-font stack to differentiate between display text, UI body text, and data/technical elements.

### Font Families

1. **Headings**: `Space Grotesk` (Sans-serif, geometric)
    * Used for: `h1`, `h2`, Section Titles.
    * Character: Modern, tech-forward, distinct.
2. **Body**: `Inter` (Sans-serif, highly legible)
    * Used for: Paragraphs, buttons, UI labels.
    * Character: Clean, neutral, versatile.
3. **Monospace**: `JetBrains Mono`
    * Used for: Input fields, code-like elements (e.g., generated links).
    * Character: Technical, precise.

### Text Styles

* **Hero Title**: `clamp(3rem, 6vw, 4.5rem)`, Weight 700, Tight leading (1.1).
* **Section Title**: `clamp(2rem, 4vw, 2.5rem)`, Weight 700, `Space Grotesk`.
* **Body Text**: `1rem` base size, `1.6` line-height for readability.

---

## 3. UI Components & Elements

### Buttons

* **Primary Button**:
  * **Background**: Linear Gradient (`135deg`, `--whatsapp-primary`, `--whatsapp-dark`).
  * **Shadow**: `0 4px 15px` colored shadow.
  * **Hover**: Transforms up (`-2px`), intensifies shadow.
  * **Animation**: `neon-glow` pulse effect on key CTAs.
* **Secondary Button**:
  * **Style**: Transparent background, 2px border (Solid `--whatsapp-primary`).
  * **Hover**: Subtle green tint background (`rgba(37, 211, 102, 0.1)`).

### Glassmorphism

Used heavily in the **Header**, **Sticky CTA**, and **Demo Cards**.

* **Background**: `rgba(20, 20, 20, 0.6)`
* **Backdrop Filter**: `blur(16px)`
* **Border**: `1px solid rgba(255, 255, 255, 0.08)` (Subtle white rim)

### Cards (Bento Grid)

* **Type**: Feature Cards, Testimonials.
* **Background**: `--neutral-800`
* **Interactive Effects**:
  * **Tilt Effect**: 3D perspective rotation on mouse move.
  * **Spotlight**: Radial gradient overlay following cursor position.
  * **Border Glow**: Highlights functional green on hover.

### Interactive "Try It Live" Demo

A functional simulation of the product within the Hero section.

* **Structure**: Input fields for simulated phone/message -> "Generate" Button -> Result Display.
* **Feedback**: Button changes state, result area slides in (`fadeIn`), mimics actual app behavior.
* **Visuals**: Tilted glass card, dark gradient background.

### Video Modal

* **Overlay**: Full-screen backdrop (`rgba(0,0,0,0.85)`) with blur.
* **Container**: Rounded corners (`16px`), standard 16:9 aspect ratio.
* **Logic**: Auto-plays on open, stops video on close (reset `src`), closeable via ESC/Click.

---

## 4. Layout & Spacing

### Grid System

* **Max Width**: `1280px` centered container.
* **Sections**: Vertical padding of `6rem` (`--section-padding`).
* **Grids**:
  * **Features**: 3-column grid (`1fr 1fr 1fr`).
    * Some items span 2 columns (`.feature-wide`) for broader visual emphasis.
  * **Testimonials**: Auto-fit grid (`minmax(400px, 1fr)`).

### Spacing Scale

Consistent spacing using CSS variables:

* `--space-4` (1rem) as base unit.
* `--space-8` (2rem) for component gaps.
* `--space-20` (5rem) for section separation.

---

## 5. Animations & Effects

### Key Animations

1. **`neon-pulse`**: Continuous breathing glow for primary CTAs.
2. **`aurora-spin`**: Subtle rotating conical gradient behind the Hero section for depth.
3. **`float-particle`**: Ambient moving dots in the background.
4. **`scroll-reveal`**: Elements fade in and slide up (`.animate-in`) as the user scrolls.

### Micro-interactions

* **Hover Lifts**: Buttons and cards lift `-5px` on hover.
* **Typewriter Effect**: Dynamic text replacement in the Hero subtitle ("Clientes", "Leads", "Qualquer Um").
* **Note Arrow**: Small arrows in footer links slide in on hover.

---

## 6. Responsive Design

* **Desktop (>1200px)**: 3-column feature grids, split Hero layout (Text Left, Demo Right).
* **Tablet/Laptop (<1200px)**:
  * Hero gap reduced.
  * Features switch to 2-column grid.
* **Mobile (<768px)**:
  * **Hero**: Stacked layout (Text Top, Demo Bottom).
  * **Grids**: All grids collapse to Single Column (`1fr`).
  * **Padding**: Reduced section padding (`--space-12`).
  * **Navigation**: Simplified, logo and actions stacked.
  * **Sticky CTA**: Text and button stacked vertically.

---

## 7. Copywriting & Content Strategy

### Core Messaging

* **Headline**: "O WhatsApp Web, com Superpoderes."
  * *Intent*: Immediately establishes familiarity (WhatsApp) while promising enhanced value/capability.
* **Subheadline**: "Pare de perder tempo salvando contatos inúteis. Fale com [Dynamic] em 1 clique, direto do navegador."
  * *Intent*: identified a common pain point (saving useless contacts) and offers an immediate solution (1-click).
* **Dynamic Keywords**: "Clientes", "Leads", "Entregadores", "Qualquer Um".
  * *Intent*: Broadens the use case appeal to different user personas (Sales, Support, Personal).

### Value Propositions (Pain vs. Gain)

* **Pain Points** (Negative Emotion):
  * "Salvar Contatos Temporários"
  * "Perder Tempo com Processos Manuais"
  * "Dificuldade para Compartilhar Seu WhatsApp"
* **Gains** (Positive Emotion):
  * "Mensagem Instantânea"
  * "Privacidade Avançada"
  * "Link Gerado & Aberto em Nova Aba"
  * "Economize 30+ Horas Por Ano"

### Micro-Copy & CTAs

* **Primary CTA**: "Adicionar ao Chrome" (Action-oriented).
* **Secondary CTA**: "Ver Demo" (Low-friction engagement).
* **Trust Badges**: "100% Gratuito", "Privacidade Total", "Junte-se a 5.000+ usuários".
* **Sticky Bar**: "Grátis para Sempre" (Objection handling).

### FAQ Strategy

* Addresses safety ("Meus dados estão seguros?").
* Addresses independence ("Oficial do WhatsApp?").
* Addresses core functionality ("Funciona com números internacionais?").

---

## 8. Icons & Assets

* **Library**: Phosphor Icons (`@phosphor-icons/web`).
* **Key Icons**:
  * `ph-download-simple` (Download/Install)
  * `ph-whatsapp-logo` (Brand recognition)
  * `ph-check-circle` (Success/Trust)
  * `ph-shield-check` (Privacy)
