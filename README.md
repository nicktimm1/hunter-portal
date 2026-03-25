# Hunter Group Portal Hosting Package

## Main entry point
- index.html
- Gateway target: Hunter_Group_Portal_Gateway_Matched_Protected.html

## Included files
- Hunter_Group_Portal_Gateway_Matched_Protected.html
- Hunter_Group_Portal_Gateway_With_All_Modules.html
- Hunter_Group_Portal_Gateway_Start.html
- Hunter_ALL_DISCIPLINES_LEVELLED_UP.html
- Hunter_Actuals_2025_2026_Monthly_Portal.html
- Hunter_Portal_Opportunities_AutoSum_FIXED.html
- Hunters_North_2026_Monthly_Board_Portal.html
- Hunters_South_2026_Monthly_Board_Portal.html
- Hunters_National_2026_Monthly_Board_Portal.html
- HCS_Supplies_2026_Monthly_Board_Portal.html

## Directors Area password
The current directors password is set inside:
- Hunter_Group_Portal_Gateway_Matched_Protected.html

Search for:
- DIRECTORS_PASSWORD

## Recommended hosting
Azure Static Web Apps

## Quick hosting steps
1. Create a GitHub repo.
2. Upload all files from this package to the repo root.
3. Create an Azure Static Web App linked to that repo.
4. Set your custom domain, for example:
   - portal.huntergroup.co.uk
5. Publish.

## Optional shared save
Files included:
- config.js
- config.sample.js

To add shared cloud saving later, wire your modules to Supabase and use:
create table if not exists service_sheets (
  job_id text primary key,
  content jsonb not null,
  updated_at timestamptz default now()
);