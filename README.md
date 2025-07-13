
# **Freelance Project Hub**  
**Overview**  
Freelance Project Hub is a web-based Project Management System built using **ASP.NET Core MVC, and Entity Framework (Code First)**. This platform allows freelancers and clients to manage projects, track time, handle invoices, and collaborate in a centralized interface. It's designed to help independent professionals streamline their workflow, ensure timely payments, and maintain client relationships efficiently.

### **Key Features**  
**Project Management** – Create, edit, and track projects with deadlines and client details.  
**Time Tracking** – Log work hours with optional screenshots for transparency.  
**Invoice Generator** – Automatically create and send professional invoices with payment links.  
**Freelancer Profiles** – Showcase skills, portfolios, and client ratings.  
**Analytics Dashboard** – View earnings, project completion rates, and workload trends.  

### **Technologies Used**  
- **ASP.NET Core MVC**  
- **Entity Framework Core (Code First)**  
- **PostgreSQL Database**  
- ** HTML / CSS**  
- ** Razor Views**  
- **Stripe/PayPal API** (for payments)  

### **Entities and Relationships**  
| **Entity**       | **Key Fields**                     | **Relationships** |
|------------------|-----------------------------------|------------------|
| **Project**      | Title, Description, Budget, Deadline | One-to-many with TimeLog, Invoice |
| **Client**       | Name, Email, Company             | One-to-many with Project |
| **Freelancer**   | Name, Skills, Portfolio, Rate    | Many-to-many with Project |
| **TimeLog**      | Hours, Date, Description, ScreenshotURL | Belongs to Project and Freelancer |
| **Invoice**      | Amount, DueDate, Status, PaymentLink | Belongs to Project |
| **ProjectFreelancer** (join table) | ProjectId, FreelancerId | Links Freelancers to Projects |

### **MVP Features**  
**Project CRUD** – Add/edit/delete projects with client details.  
**Freelancer Profile** – Create and manage freelancer portfolios.  
**Time Tracking** – Log and submit work hours for projects.  
**Invoice Generation** – Auto-generate invoices with payment integration.  
**Dashboard Analytics** – View earnings and project statistics.  

**Perfect for:** Developers, designers, writers, and other independent professionals who want to **centralize their business operations** and focus more on their craft.  

