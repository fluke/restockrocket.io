---
layout: post
title:  "How to add the Notify me when Available button on collection pages?"
category: [Design]
teaser: "Learn more about how to add Restock Rocket's button on your collection pages"
image:
  path: '/assets/img/Banner.png'
  alt: Restock Rocket notifies customers when products are back in stock
---
To allow your customers with a quick and easy way to subscribe for back in stock notifications, you can add the "Notify me when Available" button on your collection pages.

Adding the button on your collection page is a simple 2 step process.

**Step 1:** In your admin dashboard, go to **Online Store** -> **Current Theme**, click on **Actions** and select **Edit Code**

**Step 2:** Go to the **snippets** folder and add the below mentioned line of code in the relevant section of your theme files, for example: In the case of the theme "Debut", add the below code in the **product-card-grid.liquid** file or in the case of "Dawn" in the **product-card.liquid** file.

If you can't find any files like the one mentioned above, please look for the liquid snippet that rends a product on the collection page of your store

Code to be inserted:
```
<!-- Restock Rocket Code START -->
<div class="restock-rocket-collection-button-container" style="display: none;" data-product-data="{{ "{{ product | json | escape " }}}}"></div>
<!-- Restock Rocket Code END -->
```

Incase you face any issues or challenges adding the button to your collection pages, please reach out through the Support widget in the bottom left corner of the app or through email at <a href="mailto:support@restockrocket.io">support@restockrocket.io</a>.
