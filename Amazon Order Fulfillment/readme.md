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
1. Customer selects product and places order
2. Order processing and stock check
3. Payment processing
4. Order confirmation
5. Fulfilment through either FBA or FBM
6. Shipping and delivery
7. Order status updates

## Diagram Specifications
1. **Order Initiation:**
- The process begins when a customer chooses a product from the Amazon website.
- The customer adds the item to the shopping cart and proceeds to checkout if they are done shopping.
- Shipping address is selected, and payment is made to confirm the order.
2. **Fulfillment Paths:**
- FBA Path:Customer → Amazon Warehouse (Pick/Pack) → Amazon Shipping → Delivery
- FBM Path:Customer → Merchant System (Pick/Pack) → Merchant Shipping → Delivery
3. **Key Decision Points:**
   | Gateway Type | Location | Decision Criteria |
   |--------------|----------|-------------------|
   | Exclusive (X)    | Done Shopping? (Customer)| If "Yes," proceed to checkout; if "No," continue shopping.|
   | Exclusive (X)     | Is the order valid? (Order Processing) |If "Yes," accept the order; if "No," cancel and notify the customer. |
   | Inclusive (+)  | Who fulfills the order? (Order Processing) | The order can be fulfilled either by Amazon or the merchant |
  | Exclusive (X)     | Delivery Confirmation (Customer) |If delivered, the customer can provide feedback. |

## 📂Files in this Repository
- `amazon_order_fulfillment.vsdx` – The original Visio BPMN diagram file.
- `image.png` – Screenshot of the BPMN diagram.
- `README.md` – Documentation of the project.

## 📥How to View the BPMN Diagram
To view or edit the BPMN diagram:
1. Download the `amazon_order_fulfillment.vsdx` file.
2. Open it using Microsoft Visio.

For a quick preview, refer to `image.png`.

