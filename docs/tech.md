
# Technologies

## Application Tech
<hr/>
A typical DD application employs the following technologies:

``` yaml

Amazon Web Services (AWS):
  - Hosting, domains, load balancing, and content delivery networks
Docker:
  - Containerization of application environments
Python + Django:
  - Backend programming language and framework
Nginx + Gunicorn:
  - HTTP(S) Server and Web Server Gateway Interface (WSGI)
PostgreSQL:
  - Relational Database
React.js:
  - Frontend Framework to create an SPA (Single Page Application) User Interface
```

A **simplified** structure of a small application may look like the following:

``` mermaid
flowchart LR
  subgraph S1 ["Typical Small Application (Simplified)"]
    direction LR
    A[(PostgreSQL<br/>Database)] <--> B{Python+Django<br/>Backend};
    B <--> C((React.js SPA<br/>Frontend));
    E[(3rd Party<br/>Data Source)] --> B;
    C <--> D[End-user];
  end
```
!!! question "Information Overload?  <br/>We embrace an educational philosophy ensuring our client's preferred tech understanding is accurate."
    [ :material-thought-bubble: Philosophy ](/philosophy){ .md-button .md-button--primary }
## Development Tech
<hr/>
We employ the following technologies to streamline our development phase:

``` yaml
GIT Version control repositories (AWS CodeCommit):
  - Provides an iterative framework for tracking code
Slack:
  - Provides clear client and inhouse communication channels
Sentry.io:
  - Error management and tracking
Docker:
  - For containerization and provisioning of development environments
mkdocs:
  - For building thorough software documentation
Figma:
  - For wireframing, prototyping, and UI design in initial phase of development
    cycle.
Google Cloud:
  - Provides video meetings, and file management of documents, spreadsheets,
    and important files
2-Factor Auth:
  - Enabled on all development accounts to be sure sensitive information is
    never in the wrong hands
AWS Backup:
  - All project resources are backed up into the secure cloud on a daily basis
```

!!! ninfo "Click below to learn how these technologies apply in the Development Process."
    [ :material-cog: Development Process  ](/process){ .md-button .md-button--primary }
