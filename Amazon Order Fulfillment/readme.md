# Amazon Order Fulfillment BPMN Diagram

## Project Description

A Business Process Model and Notation (BPMN) 2.0 diagram modeling Amazon's order fulfillment process, covering both Fulfilled-by-Amazon (FBA) and Fulfilled-by-Merchant (FBM) workflows. Created using Microsoft Visio.

## Key Features
- 3 Pools: Customer, Amazon, Merchant
- 4 Swimlanes across pools
- Dual process flows (FBA & FBM)
- 20+ Flow Objects (Tasks, Gateways, Events)
- Multiple gateway types (Exclusive, Parallel, Event-Based)
- Task types (User, Service, Send/Receive)

The BPMN diagram illustrates the end-to-end process of ordering a product from Amazon including:
- Customer actions for placing an order.
- Amazon's order processing workflow.
- Fulfillment by Amazon (FBA) where Amazon handles packing and shipping.
- Fulfillment by Merchant (FBM) where the merchant is responsible for packing and shipping.

## Diagram Specifications
Core Components:
1. **Order Initiation:**
- Customer selects product and places order
- Payment processing
- Order confirmation
2. **Fulfillment Paths:**
- FBA Path:Customer → Amazon Warehouse (Pick/Pack) → Amazon Shipping → Delivery
- FBM Path:Customer → Merchant System (Pick/Pack) → Merchant Shipping → Delivery
3. **Key Decision Points:**
   | Gateway Type | Location | Decision Criteria |
   |--------------|----------|-------------------|
   | Exclusive    | Stock Check | Item availability[1] |
   | Parallel     | Payment Processing | Multiple payment methods |
   | Event-Based  | Shipping Update | Tracking notifications |


## Conditions for the Project
The diagram adheres to the following conditions:
1. **Pools & Swimlanes:**
   - At least 3 pools: Customer, Amazon, Merchant.
   - At least 4 swimlanes across these pools.
2. **Process Coverage:**
   - Both FBA and FBM fulfillment processes are included.
3. **Flow Objects:**
   - At least 20 different flow objects, including:
     - Tasks/Activities
     - Gateways
     - Events
4. **Gateways & Activity Types:**
   - At least 3 different types of Gateways.
   - At least 3 different types of Activity/Task.


## Files in this Repository
- `amazon_order_fulfillment.vsdx` – The original Visio BPMN diagram file.
- `image.png` – Screenshot of the BPMN diagram.
- `README.md` – Documentation of the project.

## How to View the BPMN Diagram
To view or edit the BPMN diagram:
1. Download the `amazon_order_fulfillment.vsdx` file.
2. Open it using Microsoft Visio.

For a quick preview, refer to `image.png`.

