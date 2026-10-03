# Mistvale Store Notes

## 1. What I changed

- Reworked the earlier page into a responsive Mistvale Tea Co. storefront with product browsing, category filters, sorting, search, quick view, cart drawer, delivery check, FAQ, newsletter form, and SEO metadata.
- i have made sure that it will work acording to business rule as specified.
- Kept the store data and simulated API in the single HTML file. The current cart persists in browser storage, enforces stock and quantity limits, and calculates the coupon and shipping amounts from product data.
- Added product, hero, and logo image references under `images/`.


## 2. What the AI got wrong


- The Green filter used lowercase `green`, but product categories are `Green`; the All filter also compared against a category that no product has.
- Search used `indexOf` as a boolean, so it included non-matches and excluded matches. The image click handler also referenced the loop index after the loop had finished.
- The countdown targeted November 2025, which is already in the past.
- Checkout displayed an “Order placed” alert instead of populating and submitting the required checkout form.
- Cart quantity changes could concatenate strings, and removing an item with `splice(i)` removed that item and everything after it.



## 3. Images

The project contains `images/logo.png`, `images/hero-banner.png`, and product images `p101.png` through `p108.png`. i have not compressed any images and resize it

## 4. How I tested it

No browser, device-size, keyboard/screen-reader, or Lighthouse test results are recorded here. I inspected the HTML and compared key logic with the assessment requirements.
i have tested manually all the business flow
## 5. Questions for the team

- The earlier draft's banner says free shipping over ₹499, while the current page uses ₹599. Please confirm the correct threshold.
- What are the payment mode that the site is going to accept i.e cash/Upi/Internet banking

## 6. Time spent

3 hrs

## 7. Extra features I added

The current page includes quick-view product details, persistent cart and coupon state, coupon eligibility messaging, and asynchronous product search.

## 8. With more time I would…

Run the full shopping flow at desktop and narrow mobile widths, test keyboard and screen-reader access, verify all business rules with edge cases, and run Lighthouse. I would also confirm the shipping threshold and document the image-generation and optimization workflow. and i can also setup automated testing framework to test all the scenerios automatically.
and i would love to add payment integeration for seemless online ordering and payment