# google-calendar-agent

Project integratres with Google Calendar and adds deadlines based on user's request to LLM-based agent.

## Application Flow
1. Authenticate user through Oauth
2. User makes request
3. Agent processes request and calls relevant tools to create-calendars -- if needed, or edit a pre-made calendar
4. Agent asks for permission to execute proposed changes
5. Agent confirms execution -- if allowed

## Note-to-self
- Assign each event an id (or use google's id, if you can get access)
- Agent MUST ask for approval before execution
  - Cache actions into a queue
  - Execute in parallel -- upon approval
- Agent MUST ask for clarification after initial user prompt to get the format they would like
    - Formats needed:
      - title
      - notifications  
