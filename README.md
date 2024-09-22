# The Phone Shop - Shopify Store

Welcome to **The Phone Shop**! This is a demo e-commerce store built on Shopify, created for the purpose of a job application.

[Live Store](https://eb48b2-35.myshopify.com/)

## Features Being Tested
- Custom theme based on Dawn Shopify Liquid templates
- Responsive design for both mobile and desktop
- Product images toggle based on selected color swatches
- Custom swatch color management via HEX codes and image swatches
- Unique, product-specific accordions for "Compatible Devices," "Description," "Features," "Dimensions," and "Materials"
- Graphical banners with desktop and mobile variations, managed on a per-product basis
- Customized "You May Also Like" product recommendations, with manual or random product loading options


## Approach to Implementing Features

### 1. **Custom Theme Setup**
   - I started by selecting the **Dawn** theme as the base for this project due to its flexibility and clean code structure. I then created a custom version of the theme to allow for modifications that meet the specific test requirements.
   - Using Shopify's Liquid templating language, I modified the product template to support additional dynamic content and custom features.

### 2. **Product Image Swatch Toggle**
   - To implement the product image toggle based on color swatches, I utilized Shopify’s native Product Variant functionality.

### 3. **Custom Swatch Color Management**
   - The current implementation relies on Shopify's Product Variant options for color selection, allowing the store to display either image-based swatches or HEX code-based color swatches.
   - Due to time constraints, I was unable to fully implement a customizable toggle in the Shopify theme editor (customizer) that would allow the user to choose between displaying either HEX swatches or image swatches directly from the admin panel.

### 4. **Unique Product-Specific Accordions**
   - Each product needed to have unique content for the "Compatible Devices," "Description," "Features," "Dimensions," and "Materials" accordions.
   - I used the [Metafield Guru App](https://apps.shopify.com/metafields-editor-2?search_id=8be6e8f2-b212-460f-b322-374318dc96a2&surface_detail=metafields+guru&surface_inter_position=1&surface_intra_position=5&surface_type=search) to create fields that allow the client to easily manage accordion content directly from the product admin page. I structured the accordion layout in Liquid so that it pulls content dynamically based on the product’s metafields.

### 5. **Graphical Banners**
   - Below the product details, I added up to two custom graphical banners for each product, using once again the [Metafield Guru App](https://apps.shopify.com/metafields-editor-2?search_id=8be6e8f2-b212-460f-b322-374318dc96a2&surface_detail=metafields+guru&surface_inter_position=1&surface_intra_position=5&surface_type=search).
   - Banners were made to support different images for desktop and mobile views through the use of media queries.

### 6. **Customized "You May Also Like" Section**
  - I customized the "You May Also Like" section to display up to four recommended products using Shopify's native product recommendation logic. This automatically suggests products that are related by collection or similar attributes.
  - Ideally, I would enhance this feature by allowing manual selection of recommended products. This could be achieved by leveraging Shopify's Metafields, enabling precise control over which products to recommend on a per-product basis.

### 7. **Shopify CLI and Version Control**
   - I used the Shopify CLI to manage theme development and version control, committing all changes to a public Git repository to allow visibility into the development process.
   - I ensured that all custom code was modular, easy to understand, and well-commented for future developers or reviewers.

### 8. **Mobile Responsiveness**
   - Throughout the implementation, I tested the design on both mobile and desktop screens. I utilized Shopify’s built-in breakpoints and CSS flexbox for a fully responsive layout, ensuring that all features (image toggles, accordions, banners) perform smoothly across devices.

