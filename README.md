[![CC BY 4.0][cc-by-shield]][cc-by]
# "From Static to Intelligent: Evolving SaaS Pricing with LLMs - Supplementary Material"

The aim of this repository is to centralize the work performed by the authors to write the paper: "From Static to Intelligent: Evolving SaaS Pricing with LLMs" for SOC4AI Workshop for ICSOC 2024 about an AI-driven solution to model pricings with Pricing2Yaml syntax.

## Structure

The repository contains one folders:
- `output`

In addition, there is a `requirements.txt` file that contains the dependencies needed to run the scripts, a `LICENSE` file that contains the license of the repository, a `README.md` file that contains the information of the repository, and four `.py` files: `main.py`, `WebDriver.py`, `GeminiAPI.py` and `Yaml2Class.py`. Moreover, there is an excel, `results.xlsx`, that contains the results of the validation of the original paper. Lastly, there is a `.pdf` file, `ICSOC24_Workshop_SOC4AI__Technical_Report.pdf`, that contains the technical report of the original paper.

### Output
This folder contains the outputs generated by the script when executing it for the following 30 SaaS:
| SaaS          | 
| ------------- | 
| ClickUp       | 
| Microsoft 365 | 
| Salesforce    | 
| Slack         | 
| Buffer        | 
| Hypercontext  | 
| Notion        |
| OpenPhone     | 
| Pumble        | 
| Tableau       | 
| Quip          | 
| MailChimp     | 
| Deskera       | 
| UserGuiding   | 
| Crowdcast     | 
| Planable      | 
| Databox       | 
| Trustmary     |
| Evernote      |
| Canva         |
| Clockify      |
| GitHub        |
| Figma         |
| Jira          |
| Dropbox       |
| Overleaf      |
| Postman       |
| Zapier        |
| Box           |
| Wrike         |


## Usage

### Install Dependencies
Dependencies can be installed using the following command: 

```bash
pip install -r requirements.txt
```

### Environment Variables
The scripts use the following environment variables:
- `GOOGLE_AI_STUDIO`: The API key for the Gemini API.

You should create a `.env` file in the root of the repository with the following content:

```
GOOGLE_AI_STUDIO = YOUR_API_KEY
```

You can get your API key by following the instructions in [Gemini API](https://ai.google.dev/gemini-api).

### Run the Scripts
> [!WARNING]
> The scripts is designed to be run with Python 3.9 or higher. Python 3.12.4 was used to develop the scripts.
> For using the Gemini API, you must take into account [rates and limits](https://ai.google.dev/gemini-api/docs/models/gemini) as well as the [region](https://ai.google.dev/gemini-api/docs/available-regions) where you are going to use it.

The scripts can be run by running the file `main.py`. The file contains two constants that should be modified to run the scripts:
- `URL`: The URL of the SaaS pricing.
- `SAAS_NAME`: The name of the SaaS.

Reading the original paper and/or the technical report is recommended to understand the limitations of the scripts.

## License 

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg