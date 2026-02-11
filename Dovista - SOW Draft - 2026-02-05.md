| Prepared By: [Name] [Title] [email]@threekit.com February 5, 2026 SOW #Q-XXXXX | Prepared For: Dovista / Mockfjord Expiration: March 7, 2026 |     |
| :----------------------------------------------------------------------------- | ----------------------------------------------------------: | --- |

# **Threekit Statement of Work**

This Statement of Work ("**SOW**") describes a set of Professional Services, scope, schedule, and cost of services to be provided by ThreeKit, Inc. ("**We**", "**Us**", "**Our**", "**Service Provider**") to Dovista A/S ("**Customer**", "**You**", "**Your**") and shall be governed by the terms and conditions of the Professional Services Agreement ([https://www.threekit.com/hubfs/References_Shared/ThreeKit_PSA_04072022.pdf](https://www.threekit.com/hubfs/References_Shared/ThreeKit_PSA_04072022.pdf)).

# 1. Definitions

1. **Visual Discovery** is an interactive process where users provide inputs through a visually engaging interface—including uploading images of their own homes—enabling the Visual Discovery Agent to analyze preferences, detect existing windows, and deliver personalized product recommendations with visualizations rendered on the user's actual home.

2. **Visual Discovery Agent** refers to an AI-driven system designed to analyze user-provided inputs (Discovery Inputs) and images, detect windows in uploaded photographs, and surface tailored product recommendations. It functions as an intelligent intermediary, leveraging computer vision and recommendation algorithms to match user needs with relevant window and door products.

3. **Discovery Inputs** are predefined criteria or attributes presented to users in an interactive, point-and-click format, enabling them to easily specify their preferences and requirements. These inputs guide the user through the process of narrowing down product options, facilitating the discovery of the most suitable window configurations based on their home style, aesthetic preferences, and functional needs.

4. **Image-Based Visualization** refers to the AI-powered capability to detect windows in user-uploaded photographs of their homes and render recommended window products onto those images, showing a realistic before/after comparison of how new windows would appear on the user's actual home.

5. **Headless Delivery** refers to an implementation model where Threekit delivers backend AI services, APIs, and platform capabilities, while the Customer's designated Systems Integrator ("**SI**") is responsible for designing and building the front-end user interface.

6. **Systems Integrator (SI)** refers to the third-party development partner designated by Customer to build the front-end user interface that consumes the APIs and services delivered by Threekit.

Additional definitions of SOW terminology are located in our [Glossary](https://www.threekit.com/hubfs/References_Shared/Statement_of_Work_(SOW)_Glossary.pdf).

# 2. Scope

## 2.1 Solution Summary

This SOW is to deliver **Phase 1** of the Threekit AI Visual Discovery platform for Dovista's Mockfjord brand, targeting residential homeowners through a B2C direct sales model. Phase 1 focuses on the **AI Visual Discovery capabilities**—inspiration, image upload, window detection, recommendations, and visualization—delivered through a **headless/API-first architecture**.

**Delivery Model:** Threekit delivers backend AI services and APIs. Customer's designated Systems Integrator builds the front-end user interface.

The solution will enable two primary user paths: (1) an **Inspiration Path** where users explore style-based recommendations through a discovery quiz and inspirational gallery, and (2) an **Image Upload Path** where users upload a photograph of their home, enabling AI-powered window detection and visualization of recommended products rendered directly onto their home image.

The Visual Discovery Agent will analyze user interactions, style preferences, and uploaded images to recommend suitable window products from the Mockfjord catalog. Users can see their recommendations visualized on their home. The experience captures lead information with enriched session data sent to HubSpot for sales follow-up.

**Phase 1 Scope:** AI discovery, image analysis, visualization, recommendations, HubSpot integration, lead intelligence.

**Phase 2 Scope (Future SOW):** Product configuration engine, quote generation (PDF + interactive digital).

The platform will support **seven (7) languages** at the API level: Swedish (primary), Norwegian, Danish, English, French, Polish, and Finnish. The architecture is designed to support additional languages and scale across Dovista's 14 brands and 25 European markets in future phases.

## 2.2 Visual Discovery Agent Data

### 2.2.1 Structured Product Data

You will provide the core product information for Mockfjord windows and doors. This information can be delivered as a structured dataset (CSV, Excel) or by granting Us direct access to relevant systems. If direct access is provided, You will supply all necessary access credentials and documentation required for data extraction.

The product data must include, but is not limited to:

* **Identifiers:** SKU, Product ID, Model Number
* **Grouping:** Product Line, Collection, Category (Window Type, Door Type)
* **Descriptive Information:** Product Name, Description (Swedish), Image URLs
* **Specifications:** Dimensions (width/height ranges), U-values, Energy Certification
* **Attributes:** Frame Colors (interior/exterior), Materials, Glazing Types, Opening Types
* **Style Associations:** Architectural style tags (Traditional, Modern, 1970s-80s Brutalist, Contemporary)

We will organize, transform, and enrich this product data for use by the Visual Discovery Agent and recommendation engine.

### 2.2.2 Descriptive Content & Media

You will provide rich content that brings Your products to life. This includes:

* High-quality product photography and/or renderings
* Lifestyle/inspiration imagery showing windows in Swedish home contexts
* Long-form product descriptions (Swedish)
* Marketing copy and brochure content
* Technical specification sheets

We will curate and organize this content within Our platform to power the inspiration gallery and product recommendations.

### 2.2.3 Knowledge Base

You will provide documentation that enables the Visual Discovery Agent to function as a knowledgeable window expert for the Nordic market. This includes:

* Technical specification sheets for all in-scope products
* Installation guides and requirements
* Energy certification documentation
* FAQs and common customer questions
* Information about Swedish house types and architectural styles (Traditional, Modern, 1970s-80s Brutalist/Mexeltegel, Contemporary)

We will process and structure this documentation to form the Agent's knowledge base.

### 2.2.4 Sales Process & Logic

You will provide the expertise and business rules that Your sales experts use to guide customers to the right window solutions. This is gathered through:

1. **Initial Documentation:** You will provide existing materials including sales training content, discovery questionnaires, and any logic mapping customer needs to product recommendations.

2. **Collaborative Knowledge Workshops:** We will conduct up to two (2) structured workshops with Your designated subject matter experts to capture the decision-making criteria and recommendation logic not yet formally documented, including Nordic regional preferences and house style matching rules.

### 2.2.5 Visual Discovery Inputs

You will provide a list of up to ten (10) Discovery Inputs which will help users narrow down or discover the right products for their needs. These inputs will be presented via API for Your SI to implement in the user interface. For this pilot, the inputs will focus on concepts including:

* **House Style:** Visual selection of architectural styles (Traditional Swedish, Modern, 1970s-80s Brutalist, Contemporary)
* **Window Application:** Type of window needed (Replacement, New Construction)
* **Room/Location:** Where the window will be installed
* **Frame Color Preference:** Interior and exterior color preferences
* **Material Preference:** Wood, Aluminum-clad, etc.
* **Energy Priority:** Standard, Enhanced, Premium efficiency
* **Opening Type:** Fixed, Tilt-turn, Side-hung, Top-hung, etc.

We will provide consultation to refine these inputs and incorporate them into the Visual Discovery Agent instructions.

### 2.2.6 Input / Output Criteria

You will provide up to twenty (20) example scenarios. Each scenario will specify an example set of user answers to the Discovery Inputs and/or describe characteristics of an uploaded home image, along with the expected type of product recommendations that should result. We will use these scenarios to test, calibrate, and validate the performance of the Visual Discovery Agent during the QA process.

## 2.3 Image Analysis & Visualization

This section describes the AI-powered image analysis and visualization capabilities unique to this project.

### 2.3.1 AI Window Detection

We will configure and implement AI-powered window detection capable of analyzing user-uploaded photographs of homes. The system will:

* Detect and identify existing windows in uploaded exterior photographs
* Support residential homes with up to forty-four (44) windows per image
* Recognize common Swedish house types and architectural styles
* Generate window location data for use in visualization rendering
* Expose all capabilities via REST API for SI integration

You will provide a collection of reference images representing common Swedish house types to assist in training and validation of the detection system.

### 2.3.2 Visualization Rendering

We will implement a visualization rendering pipeline that displays recommended window products on user-uploaded home images. The visualization will include:

* Window placement with perspective matching to the uploaded photograph
* Lighting and shadow adjustment for realistic appearance
* Before/after comparison image generation
* Facade/siding color change capability (allowing users to visualize their home with different exterior colors)
* Support for multi-story buildings
* Close-up detail views of recommended windows
* All visualization capabilities exposed via REST API

**Does not include:**
* Photo-realistic 3D rendering (would require separate 3D asset development)
* Interior view rendering

## 2.4 APIs & SI Integration

This section describes the API deliverables for headless integration.

### 2.4.1 API Suite

We will develop and document a comprehensive REST API suite enabling Your SI to build the front-end user interface. The API suite will include:

**Discovery APIs:**
* Start session endpoint
* Submit discovery inputs endpoint
* Get recommendations endpoint
* Get inspiration gallery data endpoint

**Image Analysis APIs:**
* Upload image endpoint
* Get window detection results endpoint
* Get house style analysis endpoint

**Visualization APIs:**
* Generate visualization endpoint
* Generate before/after comparison endpoint
* Apply facade color change endpoint
* Generate close-up view endpoint

**Lead & Analytics APIs:**
* Create lead endpoint
* Get session summary endpoint
* Export to HubSpot endpoint

**Localization APIs:**
* Get content by language endpoint
* List available languages endpoint

### 2.4.2 API Documentation

We will provide comprehensive API documentation including:

* Complete API reference with all endpoints, parameters, and response formats
* Authentication and authorization guide
* Rate limiting and usage guidelines
* Error handling reference
* Sample API calls and response examples
* Postman collection for testing

### 2.4.3 SI Consulting & Integration Support

We will provide forty (40) hours of consulting and integration support for Your designated Systems Integrator, including:

* Two (2) technical workshop sessions to review API architecture and integration patterns
* Technical consultation for integration questions
* Troubleshooting support during SI development
* Best practices guidance for API consumption
* Webhook configuration support

You will identify and engage Your Systems Integrator prior to project kickoff. Your SI should be available to participate in technical workshops starting in Week 2 of the project.

## 2.5 User Journey (API-Supported)

The Visual Discovery user journey for Mockfjord homeowners will be implemented by Your SI using Our APIs. The journey will support the following sequence:

1. **Entry:** The user accesses the Visual Discovery experience from the Mockfjord.se website (SI-built UI).

2. **Path Selection:** The user chooses between two paths:
   * **Inspiration Path:** Begin with style discovery and recommendations
   * **Image Upload Path:** Upload a photo of their home to start with AI window detection

3. **Discovery Inputs (Inspiration Path):** The user answers a series of style and preference questions (SI-built UI consuming Discovery APIs).

4. **Image Upload (Image Upload Path):** The user uploads a photograph of their home exterior (SI-built UI consuming Image Analysis APIs). The AI system detects existing windows and identifies the house style.

5. **Inspirational Gallery & Recommendations:** Based on user inputs and/or uploaded image analysis, the Visual Discovery Agent returns recommended window products with confidence messaging (SI-built UI consuming Recommendations API).

6. **Visualization:** Recommended windows are rendered onto the user's uploaded home image, showing a before/after comparison (SI-built UI consuming Visualization APIs).

7. **Lead Capture:** The user submits contact information to be contacted by a Mockfjord sales representative (SI-built UI consuming Lead APIs).

**Note:** Product configuration and quote generation are **Phase 2** scope and not included in this SOW.

## 2.6 Analytics & Lead Intelligence

### 2.6.1 Threekit Analytics Package

The Visual Discovery APIs will be equipped with the Threekit Analytics package to capture detailed data on user interactions. You will provide the Key Performance Indicators (KPIs) and primary business questions You seek to answer with analytics.

We will implement and configure the Threekit Analytics package, which captures a comprehensive set of user journey events including:

* **Session Initiated:** When a user first lands on the experience
* **Path Selected:** Which discovery path the user chose (Inspiration vs. Image Upload)
* **Image Uploaded:** When a user uploads a home photograph
* **Discovery Input Answered:** Each response to discovery questions
* **Recommendation Displayed:** When product recommendations are shown
* **Visualization Generated:** When a visualization is rendered
* **Lead Submitted:** When a user submits the lead capture form

### 2.6.2 Lead Intelligence

Each submitted lead will be enriched with AI-powered lead intelligence designed to improve lead prioritization and sales readiness. We will implement Lead Enhancing AI to analyze the event data for each user session that results in a lead.

You will collaborate with Us to define up to eight (8) key data fields for AI-powered lead enhancement. The AI-generated fields will typically include:

* **Journey Summary:** Concise summary of the user's path and key interactions
* **Style Profile:** Identified style preferences (Traditional, Modern, Contemporary, etc.)
* **House Type:** Detected house style from uploaded image
* **Key Product Interests:** Top products engaged with
* **Project Scope:** Estimated project size (number of windows detected)
* **Engagement Score:** Quantitative score indicating depth of engagement
* **Recommended Next Steps:** AI-driven suggestions for sales follow-up

### 2.6.3 Basic Lead Export

We will implement a basic lead export capability that provides session data via API, including:

* User contact information
* Session summary
* Discovery inputs and preferences
* Uploaded image reference
* Recommendations viewed
* Lead intelligence fields

## 2.7 Integrations

### 2.7.1 HubSpot CRM Integration

We will provide an integration with Your HubSpot instance to support lead generation and sales enablement.

**Lead Creation:** When a lead is submitted via the Lead API, We will create a Contact and associated Deal in HubSpot containing:

* Standard contact fields (First Name, Last Name, Email, Phone)
* All AI-powered Lead Intelligence fields defined in *Section 2.6.2*
* Session summary and engagement data

**Custom Properties:** We will configure up to fifteen (15) custom HubSpot properties to store lead intelligence and session data.

**Sales Notifications:** We will configure automated notifications to alert sales representatives when high-value leads are submitted.

You will provide:
* Access to Your HubSpot instance (sandbox and production)
* API documentation, authentication credentials, and required permissions
* Mapping of all data fields to HubSpot properties
* Specifications for sales notification triggers and recipients

We will test the integration to verify data transfer and lead creation.

## 2.8 Multi-Language Support

### 2.8.1 i18n Framework

We will implement an internationalization (i18n) framework at the API level supporting seven (7) languages:

* Swedish (primary)
* Norwegian
* Danish
* English
* French
* Polish
* Finnish

The framework will include:

* API responses with language-specific content
* Content key structure for all localizable strings
* Language selection parameter for all relevant API calls
* Extensible architecture for adding languages in future phases

### 2.8.2 Localization Content

You will provide all localized content for the seven (7) supported languages, including:

* Product names and descriptions
* Discovery input labels and options
* Recommendation messaging
* UI strings (for SI implementation)

We will integrate the localized content into the API responses.

## 2.9 Feedback Cycles

You will review and provide feedback on all deliverables within three (3) business days of delivery. You will either (i) approve the deliverables in writing or (ii) provide feedback that is specific and prioritized to Us in writing. Each deliverable shall be deemed accepted by You unless the foregoing feedback is provided to Us within three (3) business days after Our submission. Feedback, revisions, and resolutions are limited to two (2) rounds per deliverable.

### 2.9.1 Approval Milestones

1. **AI Body of Knowledge:** Final approval of the consolidated and enriched dataset that will power the Visual Discovery Agent, as defined in *Section 2.2*.

2. **Window Detection & Visualization:** Approval of the AI window detection accuracy and visualization rendering quality based on test images.

3. **API Specification:** Approval of the API design and documentation prior to development.

4. **Recommendation Logic:** Approval of the relevance and accuracy of the product recommendations generated by the Agent based on test inputs.

5. **HubSpot Integration:** Final approval of the successfully tested integration with Your HubSpot instance.

6. **API Completion:** Final acceptance of the fully developed and documented API suite.

7. **Go-Live:** Final approval for production deployment upon Your SI's successful completion of integration testing.

## 2.10 Deployment

We will deploy the Visual Discovery APIs to a secure server. Your SI is responsible for building the front-end user interface and embedding it into Your Mockfjord.se website.

## 2.11 Training & Documentation

We will provide the following training and documentation:

* Two (2) virtual admin training sessions covering platform operation and content management
* Platform documentation for ongoing administration
* Content update guide for maintaining product data and imagery
* Complete API documentation and integration guide
* Support escalation process documentation

## 2.12 Assumptions

* This SOW covers **Phase 1** only: AI Visual Discovery, image analysis, visualization, recommendations, HubSpot integration. **Phase 2** (product configuration, quote generation) will be covered in a separate SOW.

* **Headless delivery model:** Threekit delivers backend APIs and services. Customer's designated Systems Integrator is responsible for all front-end UI design and development.

* Customer will engage a Systems Integrator prior to project kickoff and ensure SI availability for technical workshops starting in Week 2.

* While every effort is made to ensure that the Visual Discovery Agent and image analysis systems generate responses aligned with user expectations, variations in output quality may occur. Some level of response quality variability is inherent to AI-driven systems.

* The accuracy of window detection is dependent on image quality. Users should be guided to upload clear, well-lit exterior photographs.

* The visualization rendering provides an approximation of how windows will appear; it is not intended to replace professional measurement and installation planning.

* This project is focused on lead generation and qualification, not e-commerce. The experience will not include shopping cart, checkout, or payment processing.

* Localized content will be provided by Customer in seven (7) languages: Swedish, Norwegian, Danish, English, French, Polish, and Finnish. Additional languages beyond these seven are out of scope for this phase but can be added with minimal effort due to the extensible i18n architecture.

* Changes to the application's Discovery Inputs, or underlying AI systems to alter recommendation results after final project acceptance are out of scope and may incur additional costs.

* The following are explicitly **out of scope** for Phase 1:
  * Front-end UI design and development (SI responsibility)
  * Product configuration engine (Phase 2)
  * Quote generation - PDF and interactive digital (Phase 2)
  * B2B property manager flow (multi-story bulk quotes)
  * Languages beyond the seven included
  * Torit pricing integration (real-time pricing)
  * SAP/ERP integration
  * Photo-realistic 3D rendering
  * Interior view visualization
  * Additional Dovista brands beyond Mockfjord

## 2.13 Customer Provided Deliverables

Successful delivery of this project is highly dependent on the reference information delivered by You to Us. The project start date and timeline will be impacted if these deliverables are not provided on time.

**Within one (1) week of project kickoff, You will provide:**

* Product data in structured format (CSV or Excel) as specified in *Section 2.2.1*
* High-quality product imagery and lifestyle/inspiration photographs
* Mockfjord brand style guide (logos, fonts, color codes)
* Initial draft of Discovery Inputs and recommendation logic
* Reference images of Swedish house types for window detection training
* HubSpot sandbox access and API credentials
* Identification of Your designated Systems Integrator

**Within three (3) weeks of project kickoff, You will provide:**

* Complete product catalog data
* Technical specification sheets and knowledge base content
* Twenty (20) input/output validation scenarios as specified in *Section 2.2.6*
* Localized content in all seven languages (Swedish, Norwegian, Danish, English, French, Polish, Finnish)
* HubSpot production access and data field mapping

# 3. Schedule and Estimated Fees

## 3.1 Estimated Schedule

Professional Services shall begin on a date to be mutually agreed upon in writing after this SOW is fully executed. Professional Services shall begin no sooner than two (2) weeks from SOW signature provided prerequisites in *Section 2.13* have been met. The project start date and timeline will be impacted if Your deliverables referenced in *Section 2.13* are not provided to Us on time. The project timeline can be impacted by holidays and scheduled time off; upon kickoff, the project manager will create a project plan that most accurately reflects the project specific timeline including any known variables.

**Target Timeline:** 8-10 weeks from kickoff to go-live

**Key Milestones:**
* **Kickoff:** March 2, 2026 (target)
* **APIs Ready:** April 13, 2026 (target)
* **Go-Live:** Early May 2026 (target)

## 3.2 Rates and Estimated Professional Services Fees

### 3.2.1

The Professional Services described in this SOW are bid on a time and material basis. Estimated Professional Services fees pursuant to this SOW are **€98,972.82** (USD $117,900 × 0.8398, rate as of Feb 11, 2026). This estimate is based upon initial discovery performed prior to signature of the SOW; the actual cost and duration of this project may differ from this estimate.

| Role | Rate | Estimated Hours | Estimated Fees |
| ----- | :---- | :---- | :---- |
| Implementation | €188.96/hour (USD $225 × 0.8398) | 524 | €98,972.82 |
| **Total** |  | **524** | **€98,972.82** |

**Estimated hours by work area:**

| Work Area | Hours |
| ----- | :---- |
| Discovery & Planning | 32 |
| AI Body of Knowledge | 80 |
| AI Agent Configuration | 72 |
| Image Analysis & Visualization | 120 |
| Lead Intelligence & HubSpot Integration | 56 |
| Multi-Language (i18n Framework) | 60 |
| QA & Testing | 40 |
| SI Consulting & Integration Support | 40 |
| Training & Documentation | 24 |
| **Total** | **524** |

### 3.2.2

Any changes to the scope of work under a Statement of Work shall be made by written change order or amendment to the Statement of Work. Any work performed pursuant to a Change Order will be billed at a blended rate of €188.96 per hour (USD $225 × 0.8398) on a time and materials basis.

---

IN WITNESS WHEREOF, the parties have caused this SOW to be executed by their duly authorized representatives as identified below.

You                                    ThreeKit, Inc.

| Signature: \s1\    | Signature: \s2\  |
| :---- | :---- |
| Date: \d1\    | Date: \d2\  |
| Name (Print): \n1\   | Name (Print): \n2\  |
| Title: \t1\   | Title: \t2\  |
