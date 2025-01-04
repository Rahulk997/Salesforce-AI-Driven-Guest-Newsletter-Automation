# Resort Newsletter Automation with Salesforce Prompt Builder

## Overview
This project demonstrates how to automate the creation of personalized resort guest newsletters using **Salesforce Prompt Builder**, **Flow Builder**, and **OpenAI GPT-4** integration. The solution dynamically personalizes newsletters based on reservation and event data, enhancing guest experiences through AI-powered content generation.

---

## Features
- **Dynamic Data Integration**: Utilizes Salesforce resources (Reservation and Experience objects) for real-time data personalization.
- **AI-Powered Prompt Template**: Generates newsletters using OpenAI GPT-4 integrated with Salesforce Prompt Builder.
- **Template-Triggered Flow**: Retrieves and formats multiple guest experiences using Flow Builder for dynamic content.
- **Merge Fields for Personalization**: Incorporates guest reservation details and experience data into the newsletter template.
- **Scalable & Flexible Design**: Allows future expansions for more data sources and experiences.

---

## Tools & Technologies
- **Salesforce Prompt Builder**
- **Salesforce Flow Builder**
- **OpenAI GPT-4 Integration**
- **Salesforce CRM Objects** (Reservation, Experience)
- **Template-Triggered Flows**

---

## Setup Instructions

### Step 1: Create Test Data
1. Navigate to **App Launcher** and search for **Experiences**.
2. Add two new experiences:
   - **Family Karaoke Night** with details like activity level, capacity, and location.
   - **Sunrise Yoga** with details including description, time, and location.

### Step 2: Create a Flex Prompt Template
1. Go to **Setup > Einstein Setup** and enable Einstein.
2. Navigate to **Prompt Builder** and create a new **Flex Prompt Template**:
   - Name: **New Guest Newsletter**
   - API Name: **New_Guest_Newsletter**
3. Add **Reservation** and **Experience** as data resources.
4. Create the newsletter prompt with placeholders for merge fields.

### Step 3: Add Merge Fields
Replace placeholders with dynamic merge fields from Reservation and Experience data sources.
- Examples:
  - `{Check-in Date}` → `Reservation > Check-in Date`
  - `{Experience Name}` → `Experience > Experience Name`
5. Select **OpenAI GPT-4** as the model and save the template.

### Step 4: Test the Prompt Template
1. Use test data to preview the template output.
2. Validate the personalized content generated for reservations and events.

### Step 5: Add a Flow for Dynamic Experiences
1. Create a **Template-Triggered Prompt Flow** in Flow Builder.
2. Define variables for **Reservation** and **Experience** objects.
3. Add elements to retrieve, loop, and format experience data.
4. Save and activate the flow.

### Step 6: Integrate Flow with Prompt Template
1. Replace static merge fields with dynamic flow data.
2. Save a new version of the template and activate it.

---

## Testing
- Use test reservation and experience data in the preview window.
- Verify that the newsletter includes details about all experiences.
- Ensure seamless integration between Flow Builder and Prompt Builder.

---


## Key Takeaways
- Leveraged **AI and Salesforce automation** for personalized guest communication.
- Demonstrated the integration of **Prompt Builder** and **Flow Builder**.
- Enhanced user experience with dynamic and scalable template-driven newsletters.

---



