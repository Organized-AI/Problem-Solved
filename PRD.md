## Product Requirements Document (PRD): Buckled.io - Customer & Mechanic Service Matching Platform

**Document Version:** 1.1
**Date:** Sep, 19th 2025
**Author:** Jordaaan's AI Assistant
**Stakeholders:** Product, Engineering, Design, Marketing, Sales, Operations

---

### 1. Introduction

*   **1.1 Executive Summary:**
    Buckled.io is a platform designed to connect vehicle owners (customers) with suitable mechanic shops for repair and maintenance services. This document outlines the core user flows for both customer and mechanic shop onboarding, as well as the functionality for customers to look up services, find appropriate shops based on vehicle make/model and service needs, and receive mock pricing/labor estimates. The platform aims to simplify vehicle maintenance for customers and provide a lead generation channel for mechanic shops.

*   **1.2 Vision & Goals:**
    *   **Vision:** To be the most trusted and efficient platform for connecting vehicle owners with quality mechanic services.
    *   **Goals:**
        1.  **Onboard diverse mechanics:** Sign up X number of mechanic shops in Y regions within the first 6 months.
        2.  **Facilitate customer acquisition:** Attract Z number of customer sign-ups in the same period.
        3.  **Enable accurate matching:** Ensure 80% of service inquiries result in at least 3 relevant mechanic shop recommendations.
        4.  **Provide clear pricing transparency:** Successfully display mock parts and labor estimates for common services.

### 2. User Stories / Personas

*   **2.1 Target Audience / Personas:**
    *   **Vehicle Owner Victor (Customer):**
        *   **Description:** 25-55 years old, owns a car, needs routine maintenance or unexpected repairs. May be unfamiliar with local mechanics or unsure about fair pricing. Values convenience, transparency, and reliability.
        *   **Pain Points:** Difficulty finding trustworthy mechanics, uncertainty about service costs, inconvenience of calling multiple shops for quotes, limited knowledge of what services their car truly needs.
        *   **Goal:** Quickly find a reputable mechanic, understand service costs upfront, and book appointments with ease.
    *   **Mechanic Shop Mike (Mechanic Shop):**
        *   **Description:** Owner or manager of an independent mechanic shop or a small chain. Has skilled technicians and capacity for new business.
        *   **Pain Points:** Challenges in attracting new customers, managing appointment schedules, providing accurate quotes quickly, competing with larger chains.
        *   **Goal:** Increase shop visibility, acquire new customers, streamline quoting processes, and efficiently manage incoming service requests.

*   **2.2 User Stories:**
    *   **Customer Sign-up & Onboarding:**
        *   As a **Vehicle Owner**, I want to **easily create an account**, so that I can **save my vehicle information and service history**.
        *   As a **Vehicle Owner**, I want to **add my car's make, model, and year**, so that the platform can **tailor service recommendations for my specific vehicle**.
    *   **Mechanic Shop Sign-up & Onboarding:**
        *   As a **Mechanic Shop Owner**, I want to **register my shop**, so that I can **be listed on Buckled.io and acquire new customers**.
        *   As a **Mechanic Shop Owner**, I want to **provide details about my services and specialties**, so that customers can **find me for relevant repairs**.
        *   As a **Mechanic Shop Owner**, I want to **set my service area/radius**, so that I **only receive leads from nearby customers**.
    *   **Service Lookup & Matching:**
        *   As a **Vehicle Owner**, I want to **search for a specific service** (e.g., "oil change," "brake replacement"), so that I can **find mechanics who offer it**.
        *   As a **Vehicle Owner**, I want to **select my vehicle's make and model**, so that the service results are **accurate for my car**.
        *   As a **Vehicle Owner**, I want to **see mock pricing for parts and labor**, so that I can **understand potential costs upfront** before committing to a shop.
        *   As a **Vehicle Owner**, I want to **view a list of mechanic shops that fit my criteria**, so that I can **compare options and choose the best one**.
        *   As a **Vehicle Owner**, I want to **see basic information about each mechanic shop** (e.g., ratings, address, contact), so that I can **make an informed decision**.

### 3. Core User Flows (Detailed)

Here, we'll map out the key journeys as depicted or implied by your Figma boards, integrating the sign-up and service lookup needs.

#### 3.1 Flow 1: Customer Onboarding & Vehicle Registration
*   **Trigger:** New user lands on Buckled.io website/app.
*   **Goal:** Customer successfully creates an account and adds their first vehicle.
*   **Steps:**
    1.  **Landing Page / Call to Action:** User sees prominent "Sign Up" or "Get a Quote" button.
    2.  **Account Creation:**
        *   User provides Email & Password.
        *   User provides Name & Phone Number.
        *   User agrees to Terms & Conditions.
        *   *Option:* "Sign up with Google/Facebook."
    3.  **Welcome / Onboarding Prompt:** User is welcomed and prompted to add their vehicle.
    4.  **Add Vehicle Information:**
        *   User selects **Vehicle Make** (e.g., Toyota, Ford, Honda) from a dropdown/autocomplete.
        *   User selects **Vehicle Model** (e.g., Camry, F-150, Civic) from a dropdown/autocomplete based on make.
        *   User selects **Vehicle Year** from a dropdown.
        *   *Optional:* User can input **VIN** for more precise lookup.
        *   User confirms vehicle details.
    5.  **Dashboard / Next Step:** User is directed to their personalized dashboard, ready to search for services.

#### 3.2 Flow 2: Mechanic Shop Onboarding
*   **Trigger:** Mechanic shop owner lands on Buckled.io "For Mechanics" section.
*   **Goal:** Mechanic shop successfully creates a profile, ready to receive leads.
*   **Steps:**
    1.  **Mechanic Sign Up Page:** User sees prominent "Register Your Shop" button.
    2.  **Shop Information:**
        *   Shop Name, Address, Phone Number, Website.
        *   Shop Owner/Contact Person Name, Email, Password.
        *   Business Registration/License details (mock).
    3.  **Services Offered:**
        *   User selects **categories of services** (e.g., Oil Change, Brakes, Engine Repair, Tires).
        *   User can specify **specialties** (e.g., European cars, Classic cars).
    4.  **Service Area / Radius:**
        *   User defines geographical area they serve (e.g., by zip code, city, or radius around shop location).
    5.  **Payment/Subscription (Mock):**
        *   User selects a mock plan (e.g., Basic, Premium - for lead volume/features).
    6.  **Profile Review & Approval (Mock):**
        *   System (or mock admin) "reviews" shop profile for completeness.
    7.  **Mechanic Dashboard:** Shop owner accesses their dashboard to manage profile, view incoming requests (once live).

#### 3.3 Flow 3: Customer Service Lookup & Mechanic Matching
*   **Trigger:** Logged-in customer wants to find a service for their vehicle.
*   **Goal:** Customer finds relevant mechanics with mock pricing for their desired service.
*   **Steps:**
    1.  **Select Vehicle:**
        *   If multiple vehicles, user selects which vehicle needs service.
        *   If no vehicle added, system prompts to add one (links to Flow 1, Step 4).
    2.  **Search for Service:**
        *   User enters a **search term** (e.g., "oil change," "brakes," "tune-up").
        *   *System suggests services based on input and vehicle type.*
        *   User selects a specific service from suggestions (e.g., "Standard Oil Change," "Front Brake Pad & Rotor Replacement").
    3.  **Service Details & Mock Pricing Display:**
        *   System displays a **summary of the selected service**.
        *   **Mock Pricing:**
            *   Displays "Estimated Parts Cost: [Mock Value, e.g., $50 - $100]"
            *   Displays "Estimated Labor Hours: [Mock Value, e.g., 1.5 - 2.5 hours]"
            *   Displays "Estimated Labor Cost: [Mock Value, e.g., $150 - $250]"
            *   Displays "Total Estimated Cost: [Mock Value, e.g., $200 - $350]"
            *   *Disclaimer: "Prices are estimates and may vary. Actual quote provided by mechanic."*
        *   User confirms this is the service they need.
    4.  **Location/Availability Input:**
        *   System uses user's default location or prompts for a preferred service location (e.g., zip code).
        *   *Optional:* User can specify preferred date/time range (for filtering).
    5.  **Mechanic Shop Results Display:**
        *   System presents a list of **matching mechanic shops** based on:
            *   Service offered
            *   Vehicle make/model compatibility
            *   Geographical proximity to customer
            *   *Optional:* Ratings, specialties, availability.
        *   For each shop, display:
            *   Shop Name, Address, Contact Info.
            *   Average Customer Rating (mock).
            *   Distance from customer.
            *   Link to shop profile.
            *   **Call to Action:** "Request Quote" or "Book Appointment."
    6.  **Shop Selection / Action:**
        *   User can click on a shop to view more details.
        *   User selects "Request Quote" or "Book Appointment" for their chosen shop(s).

#### 3.4 Future Flow (Implied by Figma - "Buckled Funnels"): Service Booking & Tracking
*   This flow would follow from "Request Quote" or "Book Appointment."
*   **Customer:** Submits request -> receives quotes -> books -> tracks service status -> pays -> leaves review.
*   **Mechanic:** Receives request -> provides quote -> confirms booking -> updates service status -> receives payment -> manages reputation.

### 4. Features & Functionality (Derived from Flows)

*   **User Management:**
    *   Customer Account Creation (Email/Password, Social Login)
    *   Mechanic Shop Account Creation
    *   Profile Management (Customer: vehicles; Mechanic: services, location)
*   **Vehicle Management:**
    *   Add/Edit Vehicle Make, Model, Year, VIN.
    *   Ability to manage multiple vehicles.
*   **Service & Part Database (Mock Data):**
    *   Categorized list of common automotive services.
    *   System for associating parts and labor hours/costs with services (mock data initially).
    *   Ability to filter services by vehicle make/model.
*   **Search & Matching Engine:**
    *   Text search for services.
    *   Filter mechanics by service, location, vehicle compatibility.
    *   Display estimated parts/labor costs per service based on vehicle.
*   **Mechanic Shop Profiles:**
    *   Detailed view for each shop (address, hours, services, specialties).
    *   Mock rating/review system.
*   **Communication / Request Management:**
    *   Ability for customers to "Request Quote" from a mechanic.
    *   Ability for mechanics to "receive" and "respond" to quote requests (mock).

### 5. Wireframes / Mockups

*   **Customer Sign Up / Login:** Refer to relevant Buckled.io general sign-up flows.
*   **Add Vehicle Flow:** 
*   **Service Search Input:** 
*   **Service Details & Mock Pricing Display:** 
*   **Mechanic Shop Results List:** 
*   **Mechanic Sign Up Flow:** 

---

This framework should give you a solid foundation for your PRD, heavily focused on the user flows you need.

**What do you think? Shall we refine any of these flows, or would you like to dive into the specific UI elements from your Figma files for a particular flow? For example, we could detail the "Add Vehicle Information" screen.**