# Shopify: Product page
![Preview](https://github.com/qcyGH/Shopify--Product-page/blob/main/preview.gif "Preview")

## Description

This is a Shopify product page. Project included product section, assets (css and js), snippets and product page template. Section have 5 tabs: all about project, characteristics, reviews, questions and gallery.

In this project i used [Swiper](https://swiperjs.com/), [breadcrumbs snippet](https://github.com/qcyGH/Shopify--Breadcrumbs-snippet) and Bootstrap.

Settings:

- Zoom image in slider on hover
- Show breadcrumbs
- Show is stock
- Show rating: Shopify doesn`t include this function. Add some rating app for this.
- Show style: Works only if styles more that one.

    Reviews settings:

    - Max reviews load: Choice max questions load in one time


    Question settings:

    - Max questions load: Choice max questions load in one time


    Gallery settings:

    - Zoom image in gallery on hover

## How to use

1. Download this project.
2. Past all files from `product page` folder to your theme folder.
3. Connect [bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/#quick-start) to your project or rewrite some elements.
4. If you dont use Swiper in your project, you need to connect the `swiper-bundle.min.css` and `swiper-bundle.min.js` files in `layout/theme.liquid` like this:

```liquid
<head>
 ...some code

 {{ 'swiper-bundle.min.css' | asset_url | stylesheet_tag }}

 ...some code

 <script src="{{ 'swiper-bundle.min.js' | asset_url }}"></script>

 ...some code
</head>
```
4. How to use it in your store:
    - If you wanna test this product page template, you need to choose `qcy` theme template in product settings.
    - If you wanna use this product page template by default, just rename file (in templates folder) from this `product.qcy.json` to this `product.json`. After this check which theme template using in product settings.
5. If your store has apps for reviews, questions, you can integrate them. This section has an HTML layout for this.
6. If you want to show product characteristics. You need to put it in the end of product description (in admin panel, 'Show HTML'):
```liquid
<div class="product-сharacteristics">
  <h2 class="product-сharacteristics__title">Characteristics <span>Varmilo Beijing Opera</span>
</h2>
  <div class="product-сharacteristics__body">
    <dl class="characteristics">
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Keyboard type</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>Mechanical</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Interface</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>USB</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Connecting</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>Wired</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Cable length, m</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>1.8</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Features</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>Skeleton</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Keyboard illumination</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>White</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Form</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>80%</span>	<!-- value -->
        </dd>
      </div>
      <!-- duplicate it for more char. -->
      <div class="characteristics__wrapper">
        <dt class="characteristics-key">
          <span>Color</span> <!-- key -->
        </dt>
        <dd class="characteristics-value">
          <span>Multicolor</span>	<!-- value -->
        </dd>
      </div>
    </dl>
  </div>
</div>
```

P.s. if you found any issues in this project, please let me know about this issues in `Issues` tab. Thank`s
