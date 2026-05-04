### 📊 Data Dictionary and Column Descriptions

This project utilizes four primary tables to track ad delivery and user interactions. Below is a breakdown of the columns and their descriptions:

#### 1. `ad_events` Table
This table captures granular interaction data for every instance a user engages with an advertisement.

| Column Name   | Description |
| :---          | :--- |
| **event_id**    | A unique identifier for each specific interaction/event. |
| **ad_id**       | Foreign key linking to the specific advertisement shown. |
| **user_id**     | Unique identifier for the user who interacted with the ad. |
| **timestamp**   | The exact date and time when the event occurred. |
| **day_of_week** | The specific day (e.g., Monday, Tuesday) the interaction happened. |
| **time_of_day** | Categorization of the event time (e.g., Morning, Evening, Night). |
| **event_type**  | The nature of the interaction (e.g., Impression, Click, Purchase). |

#### 2. `ads` Table
This table contains the metadata and targeting configuration for each individual advertisement.

| Column Name         | Description |
| :---                | :--- |
| **ad_id**             | Unique identifier for each advertisement (Primary Key). |
| **campaign_id**       | Foreign key connecting the ad to its parent marketing campaign. |
| **ad_platform**       | The social media platform where the ad was displayed (e.g., Instagram, Facebook). |
| **ad_type**           | The format of the creative used (e.g., Story, Video, Static Image). |
| **target_gender**     | The intended gender demographic for the ad (e.g., Male, Female, All). |
| **target_age_group**  | The specific age bracket targeted (e.g., 18-25, 26-30). |
| **target_interests**  | Key audience interests used for targeting (e.g., Technology, Fashion, Food). |

#### 3. `campaigns` Table
This table stores high-level metadata and budgetary information for each marketing campaign.

| Column Name | Description |
| :--- | :--- |
| **campaign_id** | Unique identifier for each campaign (Primary Key). |
| **name** | The descriptive name of the campaign. |
| **start_date** | The raw start date of the campaign activity. |
| **end_date** | The raw end date of the campaign activity. |
| **duration_days** | Total lifespan of the campaign in days. |
| **total_budget** | The total financial allocation for the campaign ($). |
| **Formatted_start_date** | Cleaned and standardized start date for reporting (DD-MM-YYYY). |
| **Formatted_end_date** | Cleaned and standardized end date for reporting (DD-MM-YYYY). |

#### 4. `users` Table
This table contains demographic and geographic details of the audience reached by the ads.

| Column Name | Description |
| :--- | :--- |
| **user_id** | Unique identifier for the individual user (Primary Key). |
| **user_gender** | The gender of the user. |
| **user_age** | The exact age of the user. |
| **age_group** | Categorization of users into specific age brackets (e.g., 18-25). |
| **country** | The country where the user is located. |
| **location** | Specific city or region within the country. |
| **interests** | User's personal preferences used for interest-based matching. |
