# Component Strategy for StellantUI (SC Design System)

## Purpose

This document outlines the strategy for selecting, using, and styling components in the SC Design System, part of the StellantAI ecosystem. The goal is to create a responsive, accessible, and AI-augmented UI framework for clinical SaaS applications across web, tablet, and mobile platforms.

---

## Component Libraries Overview

We use a hybrid strategy combining **Syncfusion EJ2 Vanilla JS** components and **Shoelace Web Components**.

---

## 1. Syncfusion EJ2 (Vanilla JavaScript)

### ✅ Why Use It:
- Enterprise-ready component library
- Built-in accessibility and internationalization
- Fully customizable with SCSS themes
- Native support for Vanilla JS (no framework lock-in)
- Includes a Figma design kit for consistency with design

### 🔧 Use Cases:
- Forms (input, select, radio, checkbox)
- Layout (grids, accordions, cards)
- Navigation (menus, tabs, breadcrumbs)
- Data visualizations (charts, data grids)
- Dialogs, modals, toasts

### 🎨 Customization:
- Follow Syncfusion's [Theme Studio](https://ej2.syncfusion.com/themestudio/)
- SC uses a Material 3-inspired color palette with custom SC Blue tokens
- Components are themed using SCSS via Syncfusion's `appearance` API

---

## 2. Shoelace (Web Components)

### ✅ Why Use It:
- Framework-agnostic Web Components
- Native browser support (no transpilation required)
- Modern styling and animations
- Easily embedded in low-code and AI-generated UI workflows
- Easily animated with CSS (e.g., zoom-in modals)

### 🔧 Use Cases:
- Lightweight modals and drawers
- Toggle switches, tabs, and tooltips
- File uploads, steppers, and date pickers
- Quick prototyping and AI-generated UIs
- Dynamic in-chat UI elements

### 🎨 Customization:
- Styled via CSS variables (custom properties)
- Extendable using SC theme tokens and utility classes
- Animations can be created using CSS keyframes

---

## Component Selection Strategy

| Component Type      | Library     | Notes |
|---------------------|-------------|-------|
| Data-Heavy Tables   | Syncfusion  | EJ2 grid supports pagination, filtering |
| Charts              | Syncfusion  | Rich API and export support |
| Form Controls       | Syncfusion  | Accessible, styled via SCSS |
| Modal/Drawer        | Shoelace    | Lightweight, CSS animation-friendly |
| Alerts/Toasts       | Shoelace    | Easily themeable, minimal JS needed |
| Low-code Widgets    | Shoelace    | Good for AI-injected UIs |
| Design Tokens       | SC Tokens   | Color, spacing, typography, exposed in Figma and SCSS |

---

## AI Integration Strategy

SC components are designed for future in-app AI generation:

- All components follow semantic HTML structure for reasoning
- Shoelace components are dynamically insertable via `innerHTML`
- Syncfusion components can be initialized programmatically via `new ej.<Component>`
- AI agents can select components using metadata tags and a JSON schema registry

---

## Theming and Design Tokens

- Defined in `/ui-system/tokens/*.json`
- Compiled into SCSS variables
- Tokens include: `color`, `typography`, `spacing`, `borders`, `shadows`
- Used across both Shoelace and Syncfusion where possible

---

## Summary

SC uses Syncfusion EJ2 for enterprise-grade UI components and Shoelace for lightweight, dynamic UI needs. This hybrid strategy enables consistent design, strong accessibility, and future-ready AI-driven UI creation.

# Components

This project utilizes Vanilla JavaScript components from both Syncfusion EJ2 and Shoelace to build a flexible and modern UI.

## Syncfusion EJ2 Components

Syncfusion EJ2 provides a comprehensive suite of UI components that are:
- Highly customizable
- Performance-optimized
- Suitable for enterprise applications

These components are integrated into our project to ensure robust functionality and a seamless user experience.

## Shoelace Components

Shoelace offers a collection of professionally designed, accessible components that:
- Are framework-agnostic
- Provide a modern look and feel
- Enhance the visual appeal of the application

By combining Syncfusion EJ2 and Shoelace components, we achieve a rich and cohesive design system that supports our application's needs.