![Build Status Badge](https://github.com/josh-mchugh/reactjs-resume/actions/workflows/main.yml/badge.svg)
[![Code Coverage Badge](https://codecov.io/gh/josh-mchugh/html-resume/branch/main/graph/badge.svg?token=3rP70grID8)](https://codecov.io/gh/josh-mchugh/html-resume)

# ReactJS Resume

> Data Driven ReactJS and Tailwindcss Resume

Create a clean looking resume with ReactJS and Tailwindcss with a web view of a A4 paper. 

## Example Image
![Screenshot of ReactJS Resume](./documentation/example.png)

## Installation
Run npm install to install dependencies.
```bash
$ npm install
```

## Run App
Hot reload and live reload with Vite
```bash
$ npm run dev
```

### Save as PDF
To save as a PDF, use the browsers print functionality but make sure he destination field has `Save to PDF` selected. Also make sure to have `Print backgrounds` enabled so it saves correctly with the background colors.

Save to PDF configuration
![Example of Save to PDF configuration](./documentation/save-as-pdf-demonstration.png)

Print backgrounds configuration
![Example of Print backgrounds configuration](./documentation/print-backgrounds-configuration.png)

## Example Data Structure
```json
[
  {
    "page": 1,
    "sideContent": [
      {
        "templateId": "nameTemplate",
        "data": {
          "name": "John Doe",
          "title": "Web and Graphic Designer"
        }
      },
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "Summary",
          "color": "white",
          "margins": "mt-10"
        }
      },
      {
        "templateId": "objectiveTemplate",
        "data": {
          "objective": "Rock Star/Ninja can you ballpark the cost per unit for me, for touch base disband the squad but rehydrate as needed sacred cow."
        }
      },
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "CONTACT",
          "color": "white",
          "margins": "mt-10"
        }
      },
      {
        "templateId": "contactTemplate",
        "data": {
          "phone": "(123) 456-8899",
          "email": "info@youremail.com",
          "location": "New York, New York"
        }
      },
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "SOCIAL",
          "color": "white",
          "margins": "mt-12"
        }
      },
      {
        "templateId": "socialTemplate",
        "data": [
          {
            "name": "Facebook",
            "icon": "fa-brands fa-facebook",
            "url": "https://facebook.com/profile"
          },
          {
            "name": "Twitter",
            "icon": "fa-brands fa-twitter",
            "url": "https://twitter.com/profile"
          },
          {
            "name": "LinkedIn",
            "icon": "fa-brands fa-linkedin",
            "url": "https://linkedin.com/profile"
          }
        ]
      }
    ],
    "content": [
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "WORK EXPERIENCE",
          "color": "gray-700",
          "margins": ""
        }
      },
      {
        "templateId": "experienceTemplate",
        "data": {
          "experiences": [
            {
              "name": "Company Name Here",
              "title": "Senior Web Developer",
              "duration": "Jan 2023 - Present",
              "location": "Remote",
              "descriptions": [
                "Efficiently unleash cross-media information without cross-media value.",
                "Quickly maximize timely deliverables for real-time schemas. Dramatically maintain clicks-and-mortar solutions without functional solutions.",
                "Completely synergize resource taxing relationships via premier niche markets. Professionally cultivate one-to-one customer service with robust ideas"
              ],
              "technologies": [
                "Photoshop",
                "HTML",
                "CSS",
                "Illustrator",
                "PHP",
                "JavaScript"
              ]
            },
            {
              "name": "Company Name Here",
              "title": "Senior Web Developer",
              "duration": "Jan 2022 – Dec 2022",
              "location": "Remote",
              "descriptions": [
                "Collaboratively administrate empowered markets via plug-and-play networks.",
                "Dynamically procrastinate B2C users after installed base benefits. Dramatically visualize customer directed convergence without revolutionary ROI.",
                "Completely pursue scalable customer service through sustainable potentialities."
              ],
              "technologies": [
                "Photoshop",
                "HTML",
                "CSS",
                "Illustrator",
                "PHP",
                "JavaScript"
              ]
            },
            {
              "name": "Company Name Here",
              "title": "Senior Web Developer",
              "duration": "Jan 2021 – Dec 2021",
              "location": "Remote",
              "descriptions": [
                "Phosfluorescently engage worldwide methodologies with web-enabled technology. Interactively coordinate proactive e-commerce.",
                "Proactively envisioned multimedia based expertise and cross-media growth strategies.",
                "Completely synergize resource taxing relationships via premier niche markets. Professionally cultivate one-to-one customer service with robust ideas. "
              ],
              "technologies": [
                "Photoshop",
                "HTML",
                "CSS",
                "Illustrator",
                "PHP",
                "JavaScript"
              ]
            }
          ]
        }
      },
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "PROFESSIONAL SKILLS",
          "color": "gray-700",
          "margins": "mt-6"
        }
      },
      {
        "templateId": "skillsTemplate",
        "data": {
          "skills": [
            {
              "name": "",
              "showGauge": true,
              "items": [
                {
                  "name": "Photoshop",
                  "value": 4
                },
                {
                  "name": "JavaScript",
                  "value": 4
                },
                {
                  "name": "Illustrator",
                  "value": 2
                },
                {
                  "name": "PHP",
                  "value": 2
                },
                {
                  "name": "HTML",
                  "value": 3
                },
                {
                  "name": "WORDPRESS",
                  "value": 3
                },
                {
                  "name": "CSS",
                  "value": 3
                },
                {
                  "name": "JOOMLA",
                  "value": 3
                }
              ]
            }
          ]
        }
      },
      {
        "templateId": "headerTemplate",
        "data": {
          "title": "EDUCATION",
          "color": "gray-700",
          "margins": "mt-6"
        }
      },
      {
        "templateId": "educationTemplate",
        "data": {
          "certifications": [
            {
              "title": "Master Degree in Studies",
              "name": "Name of University",
              "location": "New York, NY",
              "year": "2012"
            }
          ]
        }
      }
    ]
  }
]
```
