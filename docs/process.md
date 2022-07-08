# Development Process
=== "Introduction"
    Coming Soon.  See the **Visual Flowchart** for an overview.
=== "Visual Flowchart"
    ``` mermaid
    flowchart TB
      subgraph S1 [Step 1: Discovery Phase]
        direction RL
        A("<b>Discovery</b>\n[Video Call, In-Person]") --> B("<b>Requirements\nDocumentation</b>\n[Google Docs]")
        B --> A
      end

      S1 --> M1[<b>Estimate & Contract Agreement</b>]

      subgraph S2 [Step 2: Prototyping & Design]
        direction LR
        E{"<b>Wireframing\nProtoyping\nDesign</b>\n[Figma]"};
        E --> X("<b>Client\nFeedback</b>\n[Video Call, Slack]");
        X --> F("<b>Update\nRequirements</b>\n[Google Docs]");
        F --> E;
      end

      S2 --> M2[<b>Finalize Requirements</b>]

      subgraph S3 [Step 3: Minimum Viable Product]
        direction LR
        G{"<b>Active Development</b>\n[GIT, Docker, Slack,\nmkdocs, etc]"};
        G --> H["<b>Testing</b>\n[Unit Tests, User Tests]"];
        H --> J("<b>Client\nFeedback</b>\n[Video Call, Slack]");
        J --> G;
      end

      S3 --> M3[<b>Client Approval</b>]

      subgraph S4 [Step 4: Going Live]
        direction LR
        TEST("<B>Final Testing</B>") --> PROD("<B>Secure Production Environment</B>")
        PROD --> LIVE{"<B>Push Live</B>"}
      end

      S4 --> M4["<b>Transition from Active Development\n to Long-Term Support</b>"]

      subgraph S5 [Step 5: Long Term Support]
        direction LR
        BUG{"<b>Error Tracking\nBug Fixing</b>\n[Sentry]"} --> MAINT{"<B>Maintenance</B>"}
        MAINT --> ENHANCE{"<b>New Features\nEnhancements</b>"}
        ENHANCE --> BUG
      end

      M1 --> S2
      M2 --> S3
      M3 --> S4
      M4 --> S5

    ```
