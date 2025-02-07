# 📦Amazon Order Fulfillment BPMN Diagram

## 📌Requirements
Using Microsoft Visio, create a BPMN diagram for ordering product from Amazon Canada. To help you with the process, the order fulfillment process overview is shared below.

## Amazon Order Fulfillment Overview:
Once the customer places an order on amazon website, the order can be fulfilled (shipped) using either of the 2 different methods – Fulfilled by Amazon (FBA) or Fulfilled by Merchant (FBM). In FBA, the order is processed, packed, shipped, and delivered through Amazon Warehouse. In FBM, the order is processed, packed, shipped, and delivered by the Merchant. Hence, in FBM, Amazon only provides the digital infrastructure for receiving the order request, sending the notifications, and collecting the online payment. If at any point in the process, you are not sure of the step then please assume the step. This question is to check your understanding of BPMN diagramming and not to verify the real fulfillment process.


## Key Features
- 3 Pools: Customer, Amazon, Merchant
- 4 Different Swimlanes: Customer, Order Processing (Amazon), Amazon FBA, Merchant Fulfillment
- Dual process flows (FBA & FBM)
- 20+ Flow Objects (Tasks, Gateways, Events)
- Multiple gateway types (Exclusive, Parallel, Event-Based)
- Task types (User Task, Service Task, Send/Receive: Notification)

The BPMN diagram illustrates the end-to-end process of ordering a product from Amazon including:
- Customer actions for placing an order.
- Amazon's order processing workflow.
- Fulfillment by Amazon (FBA) where Amazon handles packing and shipping.
- Fulfillment by Merchant (FBM) where the merchant is responsible for packing and shipping.

## Diagram Specifications
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

## 📂Files in this Repository
- `amazon_order_fulfillment.vsdx` – The original Visio BPMN diagram file.
- `image.png` – Screenshot of the BPMN diagram.
- `README.md` – Documentation of the project.

## 📥How to View the BPMN Diagram
To view or edit the BPMN diagram:
1. Download the `amazon_order_fulfillment.vsdx` file.
2. Open it using Microsoft Visio.

For a quick preview, refer to `image.png`.

