# Capítulo III: Requirements Specification

---

## 3.1. User Stories

---

### Epic 1: Landing Page (Static Web Site)

#### US001: View Value Proposition
As a visitor I want to read the main value proposition of VET-Smart on the home page so that I can understand the comprehensive care features the software offers.

**Scenario: Successfully display the main value proposition**
* **Given** a visitor accesses the main URL of the VET-Smart landing page
* **When** the home page loads completely in the web browser
* **Then** the system displays the main value proposition text, the **IoT feeding automation** summary, and the primary call-to-action buttons

#### US002: Select Veterinarian Segment
As a visitor of the veterinarian segment I want to access a specific section detailing clinical features so that I can evaluate specialized care tools relevant to my daily practice.

**Scenario: Successfully navigate to the veterinarian features section**
* **Given** the visitor is navigating the main navigation menu
* **When** the visitor clicks on the "For Veterinarians" link
* **Then** the system redirects the visitor to a dedicated section detailing the EHR, prescription features, and **nutritional control via IoT dispenser**

#### US003: Request Software Demo
As a visitor of the administrator segment I want to submit a contact form to request a software demo so that I can see how it helps manage my clinic operations.

**Scenario: Successfully submit a demo request form**
* **Given** the visitor has filled out the demo request form with valid contact information
* **When** the visitor clicks the "Submit Request" button
* **Then** the system registers the lead in the database, including interest in the **IoT dispenser integration**, and displays a success confirmation message

#### US004: View Pricing Plans
As a visitor I want to view the available subscription plans so that I can evaluate the financial cost of the software.

**Scenario: Successfully display pricing tiers**
* **Given** the visitor is on the pricing page
* **When** the page renders
* **Then** the system displays a comparative table with the features and monthly costs of the Basic, Pro, and Enterprise plans

#### US005: Access FAQ Section
As a visitor I want to read frequently asked questions so that I can resolve my basic doubts without contacting support.

**Scenario: Successfully expand an FAQ item**
* **Given** the visitor is in the FAQ section of the landing page
* **When** the visitor clicks on a specific question
* **Then** the system expands the container to reveal the corresponding text answer

#### US006: Read Client Testimonials
As a visitor I want to read testimonials from current clinics using VET-Smart so that I can build trust in the product.

**Scenario: Successfully render the testimonials carousel**
* **Given** the visitor scrolls down to the social proof section
* **When** the section becomes visible in the viewport
* **Then** the system displays a carousel of verified reviews from clinic administrators and veterinarians

#### US007: Subscribe to Newsletter
As a visitor I want to subscribe to the newsletter so that I can receive updates on new features and veterinary management tips.

**Scenario: Successfully register an email for the newsletter**
* **Given** the visitor enters a valid email address in the subscription footer
* **When** the visitor clicks the "Subscribe" button
* **Then** the system adds the email to the mailing list and shows a "Thank you" toast notification

#### US008: View Mobile Menu
As a visitor using a smartphone I want to use a responsive hamburger menu so that I can navigate the site easily on a small screen.

**Scenario: Successfully open the mobile navigation menu**
* **Given** the visitor is viewing the landing page on a device with a screen width under 768px
* **When** the visitor taps the hamburger menu icon
* **Then** the system opens a slide-out menu containing all navigation links

#### US009: Access Contact Information
As a visitor I want to find the company's contact email and phone number easily so that I can reach out for direct inquiries.

**Scenario: Successfully locate the contact details**
* **Given** the visitor navigates to the Footer section
* **When** the visitor looks at the "Contact Us" column
* **Then** the system displays the official support email, phone number, and physical address

#### US010: View Privacy Policy
As a visitor I want to access the Privacy Policy page so that I can understand how my data and my clinic's data will be handled.

**Scenario: Successfully load the legal documents page**
* **Given** the visitor is on the landing page
* **When** the visitor clicks the "Privacy Policy" link in the footer
* **Then** the system redirects to a static page containing the full text of the privacy policy

---

### Epic 2: Clinical Management - EHR (Veterinarian)

#### US011: Search Patient Profile
As a veterinarian I want to search for a patient using their name or owner's name so that I can access their medical record quickly.

**Scenario: Successfully retrieve a patient profile**
* **Given** a patient named "Bobby" belonging to owner "Juan Perez" exists in the active database
* **When** the veterinarian types "Bobby" into the patient search bar
* **Then** the system retrieves and displays Bobby's profile in the search results list

#### US012: Record Vital Signs
As a veterinarian I want to register the weight and temperature during triage so that I can evaluate the patient's initial condition.

**Scenario: Successfully save triage vital signs**
* **Given** an active medical consultation for a patient
* **When** the veterinarian enters the numeric values "15.5" for weight and "38.2" for temperature and clicks save
* **Then** the system records the vital signs with the current date and time in the patient's clinical history

#### US013: View Allergy Alerts
As a veterinarian I want to see a visual alert if the patient has allergies so that I avoid prescribing harmful medication.

**Scenario: Successfully display a critical allergy alert**
* **Given** a patient has an active penicillin allergy registered in their profile
* **When** the veterinarian opens the patient's clinical history view
* **Then** the system displays a red, high-priority alert banner at the top of the screen

#### US014: Create Digital Prescription
As a veterinarian I want to generate a digital prescription and nutritional plans so that I can standardize the medication and care process.

**Scenario: Successfully generate a clinical prescription**
* **Given** the veterinarian is in the prescription module of an active consultation
* **When** the veterinarian selects a medication or **therapeutic diet for the IoT dispenser**, inputs the dosage, and clicks generate
* **Then** the system creates a structured digital prescription linked to the consultation ID

#### US015: Lock Clinical Record
As a veterinarian I want to lock the editing of a record once the consultation is finished so that I can guarantee its legal integrity.

**Scenario: Successfully restrict edition of a closed consultation**
* **Given** an open consultation with all clinical notes filled out
* **When** the veterinarian clicks the "Close Consultation" button
* **Then** the system changes the status to closed and sets all text fields to read-only mode

#### US016: Attach Lab Results
As a veterinarian I want to upload PDF files or images of lab results so that I have all diagnostic information in one place.

**Scenario: Successfully upload a PDF document**
* **Given** the veterinarian is in the attachments tab of a patient's record
* **When** the veterinarian uploads a valid PDF file under 10MB
* **Then** the system saves the file and displays a preview link inside the clinical history

#### US017: Schedule Vaccination Reminder
As a veterinarian I want to set a date for the next vaccination so that the system tracks the preventive health schedule.

**Scenario: Successfully save a future vaccination date**
* **Given** the veterinarian finishes applying a vaccine during a consultation
* **When** the veterinarian selects a future date in the "Next Vaccine" field and saves
* **Then** the system schedules a reminder event linked to the patient's profile

#### US018: Add Clinical Notes
As a veterinarian I want to write free-text clinical notes and daily care logs during the examination so that I can detail specific symptoms and appetite status.

**Scenario: Successfully save text in the anamnesis field**
* **Given** the veterinarian is in the physical exam section
* **When** the veterinarian types the symptoms into the anamnesis text area, reviews the **IoT dispenser logs**, and saves
* **Then** the system stores the text block exactly as written in the database

#### US019: View Medical History Timeline
As a veterinarian I want to view a chronological timeline of past visits so that I can understand the evolution of a chronic disease.

**Scenario: Successfully order past consultations**
* **Given** a patient has multiple past consultations
* **When** the veterinarian navigates to the "History" tab
* **Then** the system displays a list of past visits sorted from the most recent to the oldest

#### US020: Send Charges to Checkout
As a veterinarian I want to send the performed services and additional care consumption directly to the reception module so that I don't have to write physical payment notes.

**Scenario: Successfully transfer billing items to the ERP**
* **Given** the consultation includes a service fee and used supplies
* **When** the veterinarian clicks the "Send to Billing" button
* **Then** the system adds those items and the **IoT dispenser consumption** to the patient's pending account in the administrator's checkout module

---

### Epic 3: Administrative & Financial - ERP (Administrator)

#### US021: Perform Daily Cash Closing
As an administrator I want to execute a daily cash closing so that I can reconcile system income versus physical cash.

**Scenario: Successfully calculate the end-of-day totals**
* **Given** there are multiple registered payment transactions for the current date
* **When** the administrator initiates the cash closing process
* **Then** the system calculates and displays the total income grouped by payment method (cash, card, transfer)

#### US022: Deduct Stock Automatically
As an administrator I want the inventory stock to decrease automatically when supplies are used so that I avoid manual counting errors.

**Scenario: Successfully update inventory after clinical usage**
* **Given** a medication "Nexgard" has an available stock quantity of 50 units
* **When** a veterinarian bills 1 unit of "Nexgard" or the **IoT dispenser** releases a portion during a consultation
* **Then** the system automatically updates the inventory database, leaving 49 units available

#### US023: Receive Low Stock Alert
As an administrator I want to receive an alert when products or supplies reach their minimum threshold so that I can reorder from suppliers on time.

**Scenario: Successfully trigger a stock warning**
* **Given** a product "Therapeutic Food" has a minimum threshold of 10 units
* **When** a transaction or **IoT dispenser usage** reduces the stock to 9 units
* **Then** the system triggers a low-stock alert notification on the administrator's main dashboard

#### US024: Void Billing Transaction
As an administrator I want to be able to void an incorrect billing record so that I can keep the accounting accurate.

**Scenario: Successfully reverse a payment record**
* **Given** a completed payment transaction with ID "TXN123"
* **When** the administrator selects the transaction, inputs a justification reason, and confirms the void action
* **Then** the system reverses the charge, updates the total balance, and logs the action in the audit trail

#### US025: Register Petty Cash Expense
As an administrator I want to record daily minor purchases so that they are accurately deducted from the final cash closing.

**Scenario: Successfully record an operational expense**
* **Given** the administrator is in the cash management module
* **When** the administrator inputs an expense amount of "20.00" for "Office Supplies" and saves the record
* **Then** the system records the expense and subtracts the amount from the available physical cash total

#### US026: Add New Inventory Product
As an administrator I want to add a new medication or item category to the system database so that it can be sold and prescribed by the doctors.

**Scenario: Successfully create a new product SKU**
* **Given** the administrator is in the Inventory module
* **When** the administrator fills out the product name, category (such as **IoT Food Type**), cost price, and retail price, then clicks save
* **Then** the system generates a unique SKU and adds the product to the active inventory list

#### US027: Apply Client Discount
As an administrator I want to apply a percentage discount to a bill so that I can reward frequent clients or handle complaints.

**Scenario: Successfully recalculate total with discount**
* **Given** an open invoice with a subtotal of "100.00"
* **When** the administrator inputs a "10%" discount in the discount field
* **Then** the system updates the total amount due to "90.00" before processing the payment

#### US028: Process Multi-Payment Method
As an administrator I want to accept mixed payments (e.g., half cash, half card) so that clients have flexibility when paying large bills.

**Scenario: Successfully split a transaction**
* **Given** an invoice with a total of "200.00"
* **When** the administrator assigns "100.00" to Cash and "100.00" to Credit Card
* **Then** the system registers both payment methods under the same invoice ID and marks it as paid

#### US029: Generate Monthly Sales Report
As an administrator I want to generate a sales report by date range so that I can analyze the clinic's financial growth.

**Scenario: Successfully render the sales data table**
* **Given** the administrator is in the Reports module
* **When** the administrator selects a start date of "March 1" and an end date of "March 31"
* **Then** the system retrieves and displays a table summarizing total revenue, taxes, and net profit for that period

#### US030: Calculate Doctor Commissions
As an administrator I want the system to calculate the production of each doctor so that I can easily pay their monthly commissions.

**Scenario: Successfully calculate commission totals**
* **Given** Doctor A has performed services totaling "1000.00" with a configured commission rate of "20%"
* **When** the administrator runs the Commission Report for Doctor A
* **Then** the system displays a calculated payout amount of "200.00"

---

### Epic 4: Technical Stories (Developer / Restful APIs)

#### TS001: Retrieve Patient History Endpoint
As a developer I want to create a GET endpoint in Node.js to retrieve a patient's medical history so that the frontend application can display it.

**Scenario: Successfully return patient records via API**
* **Given** the Node.js API server is running and connected to the MySQL database
* **When** an authenticated GET request is made to /api/v1/patients/{id}/history with a valid patient ID
* **Then** the system queries the database and returns a 200 OK status with a JSON payload containing medical records and **IoT consumption history**

#### TS002: Update Stock Quantity Endpoint
As a developer I want to implement a PUT endpoint to update inventory quantities triggered by clinical events so that stock remains synchronized across the platform.

**Scenario: Successfully process a stock update request**
* **Given** a valid authentication token and a JSON payload with the new quantity
* **When** a PUT request is made to /api/v1/inventory/{sku}
* **Then** the system updates the MySQL record, reflecting clinical or **IoT dispenser usage**, and returns a 200 OK status response

#### TS003: Validate JWT Authentication
As a developer I want to implement JWT authentication middleware on all API routes so that only authorized users can access the system data.

**Scenario: Successfully reject an unauthorized API request**
* **Given** a client application without a valid JSON Web Token
* **When** the client makes a request to a protected RESTful endpoint
* **Then** the system blocks the request and returns a 401 Unauthorized HTTP status code

#### TS004: Create Consultation Transaction
As a developer I want to process consultation creation and related inventory movements within a single MySQL transaction so that data remains consistent if an error occurs.

**Scenario: Successfully rollback database changes on failure**
* **Given** a POST request to create a consultation that involves a medication or **IoT food stock deduction**
* **When** the database query for the stock deduction fails during the process
* **Then** the system rolls back the entire transaction, discarding the consultation creation, and returns a 500 Internal Server Error status

#### TS005: Create New Appointment Endpoint
As a developer I want to build a POST endpoint for scheduling appointments so that the frontend calendar can save new reservations.

**Scenario: Successfully insert a new appointment**
* **Given** a valid JSON payload containing patientId, doctorId, and dateTime
* **When** a POST request is made to /api/v1/appointments
* **Then** the system inserts the record into the database and returns a 201 Created status with the new appointment ID

#### TS006: Dashboard Metrics Aggregation
As a developer I want to create a GET endpoint that aggregates daily revenue and service usage so that the admin dashboard loads quickly.

**Scenario: Successfully return aggregated dashboard data**
* **Given** an authenticated request from an administrator account
* **When** a GET request is made to /api/v1/dashboard/summary
* **Then** the system executes a group-by query and returns a 200 OK status with a JSON object of the daily totals, including **IoT dispenser activities**

#### TS007: User Login & Token Generation
As a developer I want to implement a POST endpoint for user login so that the system can verify credentials and issue a JWT.

**Scenario: Successfully generate an access token**
* **Given** a valid email and password combination in the request body
* **When** a POST request is made to /api/v1/auth/login
* **Then** the system verifies the password hash and returns a 200 OK status with a signed JWT in the response payload

#### TS008: Soft Delete Voided Invoice
As a developer I want to implement a DELETE endpoint that performs a soft-delete on invoices so that voided records are hidden but kept for audits.

**Scenario: Successfully flag an invoice as voided**
* **Given** a valid invoice ID
* **When** an authenticated DELETE request is made to /api/v1/invoices/{id}
* **Then** the system updates the is_voided boolean to true in the database and returns a 204 No Content status

#### TS009: Query Low Stock Products
As a developer I want to create a GET endpoint that filters products below their minimum threshold so that the frontend can display alerts.

**Scenario: Successfully return a list of low-stock items**
* **Given** the database contains products where current_stock is less than or equal to min_stock
* **When** a GET request is made to /api/v1/inventory/alerts
* **Then** the system returns a 200 OK status with a JSON array containing only the affected products

#### TS010: Validate Token Endpoint
As a developer I want to create an endpoint that verifies if a JWT is still active so that the frontend can persist the user session upon page refresh.

**Scenario: Successfully validate an unexpired token**
* **Given** a client application sends an unexpired JWT in the Authorization header
* **When** a GET request is made to /api/v1/auth/verify
* **Then** the system decodes the token and returns a 200 OK status with the user's basic profile data

***
## 3.2. Impact Mapping

<img src="../assets/Impact_map_1.png" alt="Impact map 1">

<img src="../assets/Impact_map_2.png" alt="Impact map 2">



***
## 3.3. Product Backlog

---

*Order of User Stories and Technical Stories*

A continuación se presenta el Product Backlog del proyecto. El orden ha sido determinado estrictamente por el valor para el negocio, priorizando la Landing Page en los primeros sprints para asegurar la presencia web y captación temprana de leads. Las historias técnicas y de seguridad (como autenticación y JWT) se han planificado estratégicamente luego de definir el core de valor de negocio, previniendo así un enfoque incorrecto de desarrollo.

| Order | ID | User Story / Technical Story      | Story Points | Bounded Context |
| :--- | :--- |:----------------------------------| :--- | :--- |
| 01 | US001 | View Value Proposition            | 3 | Landing Page |
| 02 | US002 | Select Veterinarian Segment       | 3 | Landing Page |
| 03 | US003 | Request Software Demo             | 5 | Landing Page |
| 04 | US004 | View Pricing Plans                | 3 | Landing Page |
| 05 | US005 | Access FAQ Section                | 2 | Landing Page |
| 06 | US006 | Read Client Testimonials          | 3 | Landing Page |
| 07 | US007 | Subscribe to Newsletter           | 3 | Landing Page |
| 08 | US008 | View Mobile Menu                  | 5 | Landing Page |
| 09 | US009 | Access Contact Information        | 2 | Landing Page |
| 10 | US010 | View Privacy Policy               | 2 | Landing Page |
| 11 | US011 | Search Patient Profile            | 5 | Clinical Management |
| 12 | US012 | Record Vital Signs                | 3 | Clinical Management |
| 13 | US014 | Create Digital Prescription       | 5 | Clinical Management |
| 14 | US018 | Add Clinical Notes                | 3 | Clinical Management |
| 15 | TS001 | Retrieve Patient History Endpoint | 5 | Clinical API |
| 16 | US020 | Send Charges to Checkout          | 5 | Clinical Management |
| 17 | US026 | Add New Inventory Product         | 3 | Administrative & ERP |
| 18 | US022 | Deduct Stock Automatically        | 5 | Administrative & ERP |
| 19 | TS002 | Update Stock Quantity Endpoint    | 5 | Inventory API |
| 20 | US021 | Perform Daily Cash Closing        | 5 | Administrative & ERP |
| 21 | US028 | Process Multi-Payment Method      | 5 | Administrative & ERP |
| 22 | US013 | View Allergy Alerts               | 3 | Clinical Management |
| 23 | US015 | Lock Clinical Record              | 3 | Clinical Management |
| 24 | US016 | Attach Lab Results                | 5 | Clinical Management |
| 25 | US017 | Schedule Vaccination Reminder     | 3 | Clinical Management |
| 26 | US019 | View Medical History Timeline     | 5 | Clinical Management |
| 27 | US023 | Receive Low Stock Alert           | 3 | Administrative & ERP |
| 28 | TS009 | Query Low Stock Products          | 3 | Inventory API |
| 29 | US024 | Void Billing Transaction          | 3 | Administrative & ERP |
| 30 | TS008 | Soft Delete Voided Invoice        | 3 | Billing API |
| 31 | US025 | Register Petty Cash Expense       | 3 | Administrative & ERP |
| 32 | US027 | Apply Client Discount             | 3 | Administrative & ERP |
| 33 | US029 | Generate Monthly Sales Report     | 5 | Administrative & ERP |
| 34 | US030 | Calculate Doctor Commissions      | 5 | Administrative & ERP |
| 35 | TS004 | Create Consultation Transaction   | 5 | Clinical API |
| 36 | TS005 | Create New Appointment Endpoint   | 5 | Scheduling API |
| 37 | TS006 | Dashboard Metrics Aggregation     | 5 | Reporting API |
| 38 | TS007 | User Login & Token Generation     | 5 | IAM / Security |
| 39 | TS003 | Validate JWT Authentication       | 5 | IAM / Security |
| 40 | TS010 | Validate Token Endpoint           | 3 | IAM / Security |
