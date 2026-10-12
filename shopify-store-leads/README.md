# Shopify Store Leads: Apps, Products, Contacts $4/1k

Free sample output (6 rows, `sample.csv`) from the Apify actor **shopify-store-leads**.

Actor page: https://apify.com/transparent_meteorite/shopify-store-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Shopify store leads with 60+ installed apps and theme detected per store. Store name, myshopify domain, country, currency, product count, price range, vendors, activity, emails, phones and socials. Discover stores by niche keyword. $0.004 per store.

## Columns in sample.csv
`rowType`, `inputDomain`, `isShopify`, `detectionSignals`, `storeStatus`, `storeName`, `storeUrl`, `primaryDomain`, `myshopifyDomain`, `shopId`, `description`, `country`, `province`, `city`, `currency`, `shipsToCountriesCount`, `publishedProductsCount`, `publishedCollectionsCount`, `shopPayInstallments`, `themeName`, `themeCustomName`, `appsDetected`, `appCount`, `appCategories`, `productsSampled`, `priceMin`, `priceMedian`, `priceMax`, `productsOnSalePct`, `productsAvailablePct`, `topVendors`, `topProductTypes`, `topTags`, `lastProductPublishedAt`, `lastProductUpdatedAt`, `daysSinceLastProductUpdate`, `newProductsLast30Days`, `productCount`, `productsSampleComplete`, `topCollections`, `emails`, `phones`, `socials`, `instagram`, `facebook`, `tiktok`, `x`, `youtube`, `pinterest`, `contactEmail`, `contactPhone`, `errors`, `checkedAt`

## Data source and privacy
Public Shopify storefront data.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
