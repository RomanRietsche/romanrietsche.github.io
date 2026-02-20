---
# Leave the homepage title empty to use the site title
title:
type: landing

sections:
# not working
  - block: about.biography
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
        
      
#  - block: logos
#    content:
#      title: Section Title
#      subtitle: Section Subtitle
#      # Path to the logo images within the `assets/media/` folder
#      logo_folder: logos
#    design:
#      columns: '1'  

  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Professor
          company: Bern University of Applied Sciences
          company_url: ''
          company_logo: bfh_2
          date_start: '2023-10-01'
          date_end: ''
          description: |2-
              Research Interests:
              1. Developing effective information systems that embed artificial intelligence and large language models.
              2. Designing and measuring behavior change through digital interventions.
              3. Evaluating the impact of digital technologies on organizations in the context of reskilling and upskilling 
            
              Head of Research Lab for AI-based re- and upskilling (LAIRU) 
                * Development of AI tools e.g.: for digital onboarding, personalized learning paths, automated situative judgement tests
                * Design of a holistic Human Centric Re- and Upskilling Framework for organizations
                * Consulting
                        
        - title: External Lecturer
          company: University of St. Gallen 
          company_url: ''
          company_logo: hsg
          date_start: '2020-09-01'
          date_end: ''
          description: Teaching courses in Master of Business Innovation, Master in Computer Science and Executive Education    

        - title: 'Research visit'
          company: Cambridge Assessment and Department of Computer Science and Technology - University of Cambridge
          company_logo: cam
          date_start: '2019-06-01'
          date_end: '2020-01-30'
          description:

        - title: 'Research visit'
          company: Fox School of Business - Temple University
          company_logo: temple
          date_start: '2019-01-01'
          date_end: '2019-05-30'
          description:
  
        - title: Research Group Leader, Postdoctoral Fellow and PhD
          company: Prof. Dr. Jan Marco Leimeister, Institute of Information Systems, University of St. Gallen 
          company_url: ''
          company_logo: hsg
          date_start: '2016-06-01'
          date_end: '2023-09-30'
          description:     

        - title: Senior Systems Engineer
          company: Leitwerk AG
          company_url:
          company_logo: leitwerk
          date_start: '2013-12-01'
          date_end: '2016-05-31'
          description: |2-
              * Security Consulting (Firewalls, security concepts)
              * Network Infrastructure Consulting (Routing, Switching, VPNs)
              * Founder of the Competence Center for IT Project Management
    design:
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
      buttons:
        - name: All
          tag: '*'
        - name: AI & LLM Systems
          tag: AI & LLM Systems
        - name: Digital Interventions
          tag: Digital Interventions
        - name: Re- & Upskilling
          tag: Re- & Upskilling
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
        
  - block: portfolio
    id: talks
    content:
      title: Talks & Events
      filters:
        folders:
          - talk
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: Compact
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false  

  - block: portfolio
    id: research
    content:
      title: Research Methods
      filters:
        folders:
          - research
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
      view: Compact
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false  
      
  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      
############
##   Courses
############


  - block: accomplishments
    id: teaching
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Current Teaching'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Digital Enterprise (B.Sc. Information Systems)
          date_start: '2024-02-01'
          description: ''
          organization: Bern University of Applied Sciences
          url: ''
        - title: AI for Business (M.Sc. Digital Business)
          date_start: '2023-09-01'
          description: ''
          organization: Bern University of Applied Sciences
          url: ''
        - title: Digital Business Management (M.Sc. Digital Business Administration)
          date_start: '2024-09-01'
          description: ''
          organization: Bern University of Applied Sciences
          url: ''
        - title: Engineering the Companies Digital Core (M.Sc. Computer Science)
          date_start: '2024-02-01'
          description: ''
          organization: University of St.Gallen
          url: ''
        - title: Business Innovation II (M.Sc. Business Innovation)
          date_start: '2023-09-01'
          description: ''
          organization: University of St.Gallen
          url: ''
        - title: 'Prompt Engineering: Innovation through generative AI (M.Sc. Business Innovation)'
          date_start: '2023-09-01'
          description: ''
          organization: University of St.Gallen
          url: ''
        - title: Prompt Engineering (Executive Education)
          date_start: '2023-09-01'
          description: ''
          organization: University of St.Gallen
          url: ''


      
      
#  - block: accomplishments
#    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
#      title: 'Accomplish&shy;ments'
#      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
#      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
#      items:
#        - title: Neural Networks and Deep Learning
#          date_start: '2021-01-25'
#          description: ''
#          organization: Coursera
#          url: ''
#    design:
#      columns: '2'

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        If you want to learn more about my work. Get in contact.
      # Contact (add or remove contact options as necessary)
      email: roman.rietsche@bfh.ch
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'


---
