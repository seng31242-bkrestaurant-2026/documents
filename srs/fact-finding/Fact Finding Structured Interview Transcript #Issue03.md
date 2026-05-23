## **BK Restaurant Management System**

**Fact Finding Structured Interview Transcript**   
BK Restaurant Management System \- Client Interview Session   
---

---

* Module: SENG 31242 \- System Design Project  
* Client: Mr. Sanjeewa De Silva  
* Prepared By: Nethmi Rajapaksha  
* Date: 21/05/2026

**01.Interview Meta Data**

| Date Conducted | 21 st of May 2026 |
| :---- | :---- |
| Interviewer(s)  | Duvini Nimethra, Nethmi Rajapaksha , Dinuja Ranaweera,Sachin Lakshitha |
| Interviewee  | Mr. N. C. Sanjeewa De Silva  |
| Target Persona | Restaurant Owner  |
| Medium  | Whatsapp call |
| Objective  | Understand the current manual operations of BK Restaurant across all three branches and gather requirements for a unified digital management system covering orders, delivery, inventory, and employee management.  |

**02\. Introduction**

This interview was conducted to gather functional and non-functional requirements for the BK Restaurant Management System. 

**03\. Key Findings Summary**

 **(i) Primary Pain Point**

All orders, deliveries, inventory, and employee records are managed manually through WhatsApp, phone calls, and physical books, making centralized oversight impossible. 

 **(ii) Offline / Multi-Branch Access is Critical**

The owner needs to monitor all three branches (Ambalangoda & Kahawa) from a single dashboard. Branch managers need independent access to manage their respective operations. 

 **(iii) Required Inputs for Order Management**

Real-time digital order capture replacing WhatsApp, POS integration for walk-in orders, kitchen display for order communication, and order status tracking. 

 **(iv) Separate Workflows Identified**

'Inventory Requests to Suppliers' (procurement) and 'Daily Stock Usage' (consumption) must be distinct workflows. Delivery assignment and tracking must also be separate from order management. 

 **(v) Employee Management Needs**

Supervisors need a digital leave application and approval workflow, work schedule visibility, and attendance tracking to replace the current paper-based system.  
   
 **(vi) Issue / Alert Reporting**

The owner needs automated low-stock alerts and a way to receive real-time updates from branch managers without relying on informal phone calls or WhatsApp messages

**03\. Interview Transcript** 

**1.Interviewer:**

Hello Mr. Sanjeewa. Thank you for your time today. We are a group of software engineering students from the University of Kelaniya, and we are building the BK Restaurant Management System to replace the current manual process. I would like to ask a few questions about your daily operations to make sure the new system meets your needs.

**Mr. Sanjeewa:** 

Hello\! Yes, I am glad you are doing this. Right now, everything is done through WhatsApp and phone calls. It is very difficult to manage three branches this way.

**2.Interviewer:** 

I understand. What is your main goal for introducing this new system?

**Mr. Sanjeewa:** 

My main goal is to have one place where I can see everything \- all three branches, all orders, all stock, and all employees. Right now, I have no visibility. I depend on branch managers calling me with updates.

**3.Interviewer:** 

What are the biggest challenges you face with the current manual process?

**Mr. Sanjeewa:** 

There are many. First, orders come through WhatsApp and phone calls \- we miss orders, we lose track of them. Second, I cannot see where delivery riders are or if an order has been delivered. Third, all our records \- sales, inventory, employees \- are in physical books. If something is lost, we lose that data permanently. And managing three branches this way is very time consuming.

**4.Interviewer:** 

How are restaurant operations currently managed on a daily basis?

**Mr. Sanjeewa:** 

Every day, staff receive orders through WhatsApp or phone and write them on paper. The cashier tells the kitchen verbally what to prepare. Inventory is checked manually and written in a book. Riders are assigned by phone call. Branch managers handle attendance and schedules on paper. At the end of the day, I have no real report \- just whatever the branch manager tells me over the phone.

**5.Interviewer:** 

What are the biggest challenges in managing multiple branches?

**Mr. Sanjeewa:** 

I cannot see all three branches at the same time. I have no way to compare sales or check stock levels without calling each manager separately. Inventory requests to suppliers are done informally by each branch on their own. There is no coordination at all. Every business decision depends on someone calling me first.

**6.Interviewer:** 

How are customer orders currently received and recorded?

**Mr. Sanjeewa:** 

Customers call us or send a WhatsApp message. The staff write it down on paper or just try to remember it. There is no system. Sometimes orders are missed, especially when it is busy.

**7.Interviewer:** 

What problems usually occur during order handling?

**Mr. Sanjeewa:** 

Missed orders are the biggest problem. When many WhatsApp messages come at the same time, it is easy to overlook one. There is no order history, so if a customer follows up we have no record. And because orders are passed verbally to the kitchen, the wrong item is sometimes prepared. There is also no way to confirm order status with the customer.

**8.Interviewer:** 

We will build a POS system for the reception and kitchen, and a digital order management flow. How are orders communicated to the kitchen staff currently?

**Mr. Sanjeewa:** 

The cashier tells the kitchen verbally. If they are busy, sometimes the message is wrong or forgotten. It causes a lot of problems.

**9.Interviewer:** 

How are order changes or cancellations handled?

**Mr. Sanjeewa:** 

If a customer changes or cancels an order, the cashier has to go and tell the kitchen verbally again. If the food is already being prepared, it is usually too late. And if a rider has already been sent out, we have to call the rider on the phone to inform them. There is no proper process for this at all. It is very confusing.

**10.Interviewer:** 

Understood. In the new system, orders will appear on a kitchen display in real time. How are deliveries currently assigned to riders?

**Mr. Sanjeewa:** 

We call the rider on the phone and tell them where to go. I have no way to see if they reached the customer. Sometimes customers call to ask where their order is and I cannot answer.

**11.Interviewer:** 

What challenges occur during the delivery process?

**Mr. Sanjeewa:** 

Once the rider leaves, I have no idea where they are. I cannot see if they are stuck in traffic, if they reached the customer, or if there was a problem. Riders also have no navigation help from us \- they use their own phones. Sometimes deliveries are delayed or go to the wrong address and we only find out when the customer complains.

**12.Interviewer:** 

How is delivery status currently monitored or communicated?

**Mr. Sanjeewa:** 

It is not monitored at all, honestly. The only way I know a delivery is complete is when the rider calls me back or returns to the restaurant. Customers have to call us directly if they want to know where their order is. It is embarrassing sometimes.

**13.Interviewer:** 

We will build a mobile app for riders with GPS tracking so you can monitor all deliveries from the dashboard. How is inventory managed currently?

**Mr. Sanjeewa:** 

Everything is in books. We do not know the exact stock until someone physically checks. When something runs out, we only find out when the kitchen cannot prepare an order. Then we call the supplier at the last minute.

**14.Interviewer:** 

What common problems occur in stock management?

**Mr. Sanjeewa:** 

Records are often outdated or wrong due to manual errors. We cannot see any trends in how fast items are being used. Each branch manages its own stock independently so there is no coordination between branches. And because everything is on paper, data can easily be lost.

**15.Interviewer:** 

How are stock shortages handled?

**Mr. Sanjeewa:** 

We only find out there is a shortage when the kitchen tells us they cannot make a certain dish. Then the branch manager calls the supplier urgently. It is always a last-minute situation. Sometimes the supplier cannot deliver in time and we have to remove items from the menu that day. It is very disruptive.

**16.Interviewer:** 

We will build automated low-stock alerts and a supplier request feature. When you need stock, you can send a digital request directly from the system. How do branches request inventory items from suppliers currently?

**Mr. Sanjeewa:** 

The branch manager calls the supplier on the phone or sends a WhatsApp message. There is no formal order. No record is kept of what was requested or whether it was delivered correctly. If there is a dispute with a supplier, we have no proof of what was agreed.

**17.Interviewer:** 

How do you manage employees and their schedules currently?

**Mr. Sanjeewa:** 

Schedules are done manually by the branch manager. Attendance is on paper. Leave requests are verbal or through WhatsApp. I have no central view of who is working where.

**18.Interviewer:** 

How is employee attendance currently recorded?

**Mr. Sanjeewa:** 

Attendance is marked on paper every day by the branch manager. Leave requests come through WhatsApp or verbally and are approved informally. I have no real-time visibility into attendance across all three branches. Everything depends on what the branch manager chooses to tell me.

**19.Interviewer:** 

What difficulties exist in managing employees?

**Mr. Sanjeewa:** 

I have no central view of who is working, who is on leave, or how employees are performing across branches. The leave approval process is inconsistent. Employees sometimes do not even know their own schedule and have to ask the manager. Keeping all these records manually is very time consuming for everyone.

**20.Interviewer:** 

Employees will be able to view their schedules and apply for leave through the system, and you will see all of this on your dashboard. What are your main requirements for the new system?

**Mr. Sanjeewa:** 

I need three main things. First, a web dashboard where I can see all three branches \- sales, inventory, employee activity, and delivery status \- all in one place. Second, a mobile app for my riders so they can receive orders, navigate to customers, and update delivery status. Third, a POS system at the counter and kitchen so orders are recorded digitally, bills are generated automatically, and everything syncs to my dashboard in real time.

**21.Interviewer:** 

What is your definition of done for this project?

**Mr. Sanjeewa:** 

For me, the project is done when the system is fully live at all three branches and my staff are actually using it. Orders should no longer come through WhatsApp. Riders should be using the mobile app. Inventory should be tracked automatically. Employees should be able to apply for leave through the system. And I should be able to generate a report for any branch at any time without calling anyone.

**22.Interviewer:** 

What would make you consider this system a success after it is implemented?

**Mr. Sanjeewa:** 

The day I stop using WhatsApp for orders \- that alone would be a huge success. And if I can open a dashboard and see all three branches at once: sales, stock, delivery status. That is what I need.

**Interviewer:** 

Thank you very much, Mr. Sanjeewa. Your answers are very helpful and will guide our system design directly.

**Mr. Sanjeewa:** 

Thank you. I look forward to seeing the system.

# **04\. Requirements Summary**

## **Functional Requirements**

* Online order management  
* POS system  
* Inventory tracking  
* Employee management  
* Delivery tracking  
* Rider mobile application  
* Leave management  
* Dashboard reporting

## **Non Functional Requirements**

* User friendly UI  
* Real-time synchronization  
* Multi-branch support  
* Secure authentication  
* System reliability

**05\. Problems in current system**

* Orders managed manually  
* No centralized database  
* Inventory not tracked properly  
* Employee attendance managed manually  
* No formal supplier management system

**06\. Conclusion**

The interview helped identify the major operational problems and system requirements of BK Restaurant. These findings will guide the development of the proposed restaurant management system. 