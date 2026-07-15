# Shopify Custom Banner Section

A custom Shopify theme section built using Liquid, HTML, and CSS as part of my Shopify development practice.

## What it does

Displays a customizable banner (e.g., for promotions or announcements) that merchants can edit directly from the Shopify theme editor — no code required.

## Features

- **Merchant-editable settings** via Shopify's schema system:
  - `text` input for the heading
  - `textarea` input for the subtext
  - `color` picker for the background color
- **Liquid objects** (`{{ }}`) used to dynamically render both content and CSS styling
- **Flexbox layout** for responsive centering
- **Presets** configured so the section can be added directly from the theme editor

## How it works

The section is built as a single `.liquid` file containing:
1. HTML markup with Liquid objects pulling data from `section.settings`
2. Inline `<style>` block using Liquid to dynamically set the background color
3. A `{% schema %}` block defining the editable settings and presets

## Tested on

Integrated and tested on a live Shopify development store using the Horizon theme.
