Hero Salon - AI Phone Agent
This repository contains the n8n workflow file (.json) for an automated AI phone agent designed for "Hero Salon".

Project Goal
The purpose of this project is to create an AI-powered virtual receptionist that can handle incoming phone calls. It is designed to understand customer requests, book appointments directly into a calendar, and answer basic questions, all without human intervention.

How It Works
The workflow automates the entire call process from start to finish:

Receives Call: A phone call to a dedicated number triggers the workflow.

Converts Speech to Text: The caller's spoken words are transcribed into text.

Understands Intent: The text is analyzed by an AI to determine what the caller wants (e.g., book an appointment).

Takes Action: Based on the intent, the system either creates a Google Calendar event or prepares an answer to a question.

Generates Audio Response: The text-based response is converted into a natural-sounding voice.

Responds to Caller: The audio response is played back to the caller over the phone.

Services Required
To run this workflow, you will need accounts for the following services:

n8n (for running the workflow)

Twilio (for the phone number)

OpenAI (for the AI analysis)

ElevenLabs (for speech-to-text and text-to-speech)

Google Cloud Platform (for Google Calendar integration)

Setup Instructions
Import Workflow: Import the .json file from this repository into your n8n instance.

Add Credentials: In n8n, add your API keys for Twilio, OpenAI, ElevenLabs, and set up Google OAuth2 credentials.

Configure Twilio:

Get a voice-enabled phone number from Twilio.

Set the number's voice webhook to the URL provided by the n8n "Call Trigger" node.

Activate: Save and activate the workflow in n8n.

Once set up, you can call the Twilio number to interact with the AI agent.
