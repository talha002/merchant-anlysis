# Merchant Analysis

I've made merchant and order analysis with using a data set tried to answer questions down below:

## Analysis Questions

- Review and clean data if necessary
- What characteristics do the most successful merchants share?
- What are the top two shipping carriers? Why should or shouldn’t we try to use those two for all orders?
- Print Providers control the print quality, stock of items, and production time (the time from ordered to fulfilled). We want to provide a discount to the two best Print Providers and end our contracts with the worst two. Which do you choose and why?

## Data

There is two dataframe, one of them is order_df and the other one is line_df
 
### Order DF

- MERCHANT_ID: Unique ID of merchant
- ORDER_ID: Unique ID of order coming from merchant
- SHOP_ID: Unique ID of merchant's shop
- ADDRESS_TO_COUNTRY: Country to where the order is shipped
- ADDRESS_TO_REGION: Region to where the order is shipped
- ORDER_DT: Timestamp when order has been created
- FULFILLED_DT: Timestamp when order has been printed
- SALES_CHANNEL_TYPE_ID: ID of sales channel from which merchant generated order
- TOTAL_COST: Amount of money collected for product (cents)
- TOTAL_SHIPPING: Amount of money collected for shipping services (cents)
- MERCHANT_REGISTERED_DT: Timestamp when merchant has registered in the platform
- SUB_IS_ACTIVE_FLAG: Has merchant currently subscribed to any subscription plan
- SUB_PLAN: What is the subscription plan that the merchant has subscribed to
- SHIPMENT_CARRIER: Shipping carrier chosen for shipment of the order
- SHIPMENT_DELIVERD_AT: Timestamp when shipment has been delivered

### Line DF

- ORDER_ID: Unique ID of order coming from merchant
- PRINT_PROVIDER_ID: Unique ID of a print provider that is printing this specific line item
- PRODUCT_BRAND: Brand of blank product
- PRODUCT_TYPE: Product type
- QUANTITY: Ordered quantity of specific line item
- REPRINT_FLAG: If line item needed to be reprinted
