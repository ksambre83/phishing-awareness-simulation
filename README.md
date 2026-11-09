# Phishing Awareness Simulation

A controlled, local phishing-awareness exercise built around GoPhish and Mailpit. The project demonstrates how a test campaign can deliver a simulated message, track safe link interaction, and direct the participant to an educational landing page without collecting credentials.

## Objectives
- Configure a local email-testing workflow.
- Build a simple awareness email and landing page.
- Execute a campaign against a test recipient under the project owner's control.
- Review campaign delivery, open, and click metrics.
- Demonstrate safe handling by disabling submitted-data capture.

## Tools
- GoPhish — campaign management and event tracking.
- Mailpit — local SMTP capture and inbox inspection.

The tools are not included in this repository; download them from their official sources.

## Repository contents
```text
phishing-awareness-simulation/
├── README.md
├── campaign-artifacts/
│   ├── email-template.html
│   └── awareness-landing-page-copy.md
└── docs/
    └── local-setup.md
```

## Demonstrated outcome
In the final controlled test, the campaign dashboard recorded 1 email sent, 1 email opened, 1 link click, and 0 submitted data. The recipient was a test account controlled by the project owner; email was captured locally by Mailpit. These figures describe this single test run only.

## Run the lab
See [Local setup](docs/local-setup.md) for the workflow and local endpoint configuration.

## Safety notice
For education and authorized awareness testing only. Use a test recipient you control, keep services local, disable credential capture, and do not run campaigns against people or organizations without explicit written authorization.
