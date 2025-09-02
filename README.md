# google-calendar-agent

Project integratres with Google Calendar and adds deadlines based on user's request to LLM-based agent.

## Application Flow
1. Authenticate user through Oauth
2. User makes request
3. Agent processes request and calls relevant tools to create-calendars -- if needed, or edit a pre-made calendar
4. Agent asks for permission to execute proposed changes
5. Agent confirms execution -- if allowed

