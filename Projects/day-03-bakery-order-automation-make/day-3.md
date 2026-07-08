# Day 3 - Bakery Order Automation (Make)

## Project

Built a bakery order automation workflow in Make using Google Forms, Google Sheets, Gmail, and conditional routing.

## Workflow

Google Form Submission
Store Order in Google Sheets
Router (Delivery Option)
        Pickup -> Send Pickup Confirmation Email
        Delivery -> Send Delivery Confirmation Email -> Notify Delivery Team

## What I Learned

- Built the same workflow in Make after implementing it in Zapier.
- Learned how Make structures Google Forms responses as nested collections.
- Understood data mapping using:
  - textAnswers
  - answers[]
  - value
- Configured routers and conditional paths.
- Used conditions based on the "Delivery Option" field.
- Mapped form responses into Google Sheets.
- Built multiple actions inside a single route.

## Challenges Faced

- Incorrect email mapping caused Gmail validation errors.
- Initially mapped collections instead of the actual value.
- Learned to navigate nested objects to retrieve the required data.
- Understood why conditions fail when the mapped value doesn't exactly match the expected text.

## Zapier vs Make

### Zapier

- Beginner-friendly interface
- Easier field mapping
- Faster to build simple automations
- More guided experience

### Make

- More visual workflow builder
- Provides greater flexibility
- Requires understanding nested data structures
- More control over routing and complex logic
- Better suited for advanced automation scenarios

<img width="1652" height="811" alt="image" src="https://github.com/user-attachments/assets/e9d2b667-60e1-4ce4-b897-5e0c428a283f" />

