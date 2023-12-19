---
# Leave the homepage title empty to use the site title
title: ''
date: 2023-12-07
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Data Scientist II - People Analytics
          company: Unum
          company_url: 'https://www.unum.com'
          company_logo: org-unum
          location: Remote
          date_start: '2021-06-21'
          date_end: ''
          description: |2-
              
              * Built a machine learning model to analyze gender-pay equity.
              * Used natural language processing for topic modelling to summarize open-ended survey questions.
              * Wrote an R script to extract relevant skillsets from online job requisition postings.
              * Deployed the first corporate social responsibility tableau dashboard enterprise-wide.
              * Wrote a Python script to analyze  discrepancies between leave absence requests across two disparate systems.
              * Performed a continual chi-square analysis to analyze turnover rates for employees who received a salary adjustment.

        - title: I/O Psychologist
          company: Checkster / OutMatch
          company_url: 'https://outmatch.com/'
          company_logo: org-checkster
          location: Remote
          date_start: '2020-10-01'
          date_end: '2021-03-01'
          description:  |2-
          
              * Led a project to develop a machine learning algorithm to predict job performance from 360 degree reference-check scores.
              * Served as a consultant to advise clients on topics such as survey items, rating scales, benchmark analytics and scoring.
              * Created an internal wiki repository of centralized knowledge concerning best practices with regards to I/O psychology topics and principles.
              * Cluster-analyzed job classifications to streamline competencies.

        - title: Consultant / Senior Researcher
          company: Industrial/Organizational Solutions, Inc.
          company_url: 'https://iosolutions.com/'
          company_logo: org-ios
          location: Oak Brook Terrace, Illinois
          date_start: '2012-09-01'
          date_end: '2020-09-20'
          description:  |2-
          
              * Consulted police & fire chiefs, HR managers and other key government officials on policies and practices in employee selection and minimizing adverse impact and bias in testing.
              * Compiled and produce rigorous statistical technical documentation for project work.
              * Built a dynamic feedback reporting system with R and Markdown to create automated customizable feedback reports for clients.
              * Built an interactive Shiny R user dashboard to import, pre-process, score, and summarize datasets containing written examination data.
              * Ran statistical analyses to drive organizational change including: ANOVA, t-test, chi-square, linear, multiple and logistic regression, correlations, factor and cluster analysis, etc.
              * Developed machine learning algorithms (regression) to set cut-scores on high-stakes employment tests administered nationally to over 100,000 candidates.

    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2015-09-01'
          description: ''
          icon: faa
          organization: Federal Aviation Administration
          organization_url: https://www.faa.gov
          title: Private Pilot License, Aircraft Single Engine Land
          url: ''
        - certificate_url: ''
          date_end: '2023-05-01'
          date_start: '2020-10-01'
          description: Built an R package called *Medusa* to streamline the data cleaning process of membership data. Also participated in establishing a fundamental data infrastructure plan for all volunteer committees within SIOP to better streamline the availability of data democratization across the organization.
          icon: siop
          organization: SIOP
          organization_url: https://www.siop.org
          title: Society for Industrial/Organizational Psychologists - Volunteer
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-11-01'
          description: Helping build data visualization infrastructure from survey responses to document the story of engagement and growth for YTP. I primarily use R Markdown / Quarto to build visualization notebooks that are connected to google sheets survey data. Other duties as a volunteer include consultation on survey development processes concerning content, sample sizes, and statistical testing to demonstrate event impact on the wellbeing of the community.
          icon: org-ytp
          organization: Yellow Tulip Project
          organization_url: https://theyellowtulipproject.org/
          title: The Yellow Tulip Project - Volunteer
          url: ''
        - certificate_url: ''
          date_end: '2019-01-01'
          date_start: '2017-11-01'
          description: I served on the board of a not-for-profit flying club.
          icon: 
          organization: Fox Flying Club
          organization_url: https://www.foxflying.com/
          title: Fox Flying Club - Board Member
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: 'A curated set of photos from my flying trips.'
      text: |-
        {{< gallery album="aviation" >}}    
    design:
      columns: '1'
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Topics
    design:
      columns: '2'
---
