<script>
  //TODO: create svg in procreate for favicon and maybe other images on the site
  //TODO: find profile picture of me being old
  //TODO: at least try a background slowmotion video
  const rez = {
    meta: {
      theme: "elegant",
    },
    basics: {
      name: "Trey Hayden",
      label: "Software Engineer",
      picture:
        "https://lh3.googleusercontent.com/MS0VpWuzC_0WevZjP5khDTcHSn9VhgqaDXo7Vatwfmae1LarwULPDTtIXRFJ9LXZOAV3YAyTSgF3IMqfLK36Ymhp8jlQMVPiYvArVUPW1JFMCvw0BFcL4Ovg9jcesXUU-JKI--M0dcU=s200-p-k",
      email: "treyhay@gmail.com",
      phone: "(703) 994-8268",
      website: "https://go.treyhay.com/resume-download",
      summary:
        "Can I interest you in some automation?! I am a full-stack polyglot software engineer who gets excited to save button clicks! I favor .NET and the backend side of software but mostly enjoy collaborating with smart people on difficult problems!",
      location: {
        address: "9461 Assembly Way",
        postalCode: "23116",
        city: "Mechanicsville",
        countryCode: "US",
        region: "Virginia",
      },
      profiles: [
        {
          network: "linkedin",
          username: "trey-hayden",
          url: "https://www.linkedin.com/in/trey-hayden",
        },
        {
          network: "github",
          username: "treyhay31",
          url: "https://github.com/treyhay31",
        },
      ],
    },
    work: [
      {
        position: "Lead Software Engineer",
        company: "U.S. Bank",
        startDate: "2019",
        endDate: "now",
        summary:
          "At the bank I've been involved with several different teams dealing with a broad range of tech. We support ecommerce, mobile apps, payment terminals, and most recently technology governance.",
        website: "https://www.elavon.com/index.html",
        highlights: [
          "Created entire end-to-end functional test suite using Playwright, shrinking our testing from around 30 mins per cycle down to 1 min per cycle",
          "Handled requirements gathering to production deployment for features in our governance app which increases compliance measures and decreases time to production for 1,000s of developers",
          "Led team that placed in the top 5 for our company's internal MS Teams Application hackathon",
          "Led team of 10 developers on new secret management using Hashicorp Vault for wide range of applications",
          "Enhanced & maintained applications that support payment processing across windows, web, iOS, and Android platorms",
          "Improved developer workflow with scripts that enforce standardizations and automate common tasks in js, python, bash, batch, and powershell",
          "Implemented robust DevOps pipelines for hundreds of code repositories",
          "Increased test coverage and implemented secure code practices across legacy code bases",
          "Facilitated cloud-to-cloud migration to Azure for suite of microservices",
          "Led team of five QA engineers on A11Y automated scan & aggregation of accessibility findings using Selenium for .NET",
        ],
      },
      {
        position: "Senior Consultant",
        company: "CapTech Ventures, Inc",
        startDate: "2019",
        endDate: "2019",
        summary:
          "Our team helped bring a cloud solution and proper development best practices to clients of all levels of expertise.",
        website: "https://www.captechconsulting.com/",
        highlights: [
          "Supported a lift-and-shift cloud migration to AWS using terraform",
          "Provisioned windows host servers using Powershell DSC for declarative automation",
          "Automated internal API challenge framework",
        ],
      },
      {
        position: "Software Developer",
        company: "Dimensional Fund Advisors",
        startDate: "2017",
        endDate: "2019",
        summary:
          "Our team handled many internal applications for the portfolio managers and traders. On top of addressing bugs and feature requests, we automated integration pipelines and greatly shrank the level of effort required for deployments.",
        website: "https://www.dimensional.com/",
        highlights: [
          "Built and maintained .NET applications for trading & portfolio management processes",
          "Increased test coverage from 0% to 100% on one of our primary trading applications",
          "Automated deployment and server provisioning for multiple applications, eliminating human error",
        ],
      },
      {
        position: "Software Developer",
        company: "ETS: Electronic Transaction Systems",
        startDate: "2013",
        endDate: "2017",
        summary:
          "Our development team developed online checkout solutions and peer to peer payments for customers.",
        website: "https://elavonpayments.com/",
        highlights: [
          "Developed & maintained Web API for company peer-to-peer payment platform",
          "Developed SDK for company consumer-to-business payment platform",
        ],
      },
      {
        position: "Consultant",
        company: "Deloitte",
        startDate: "2011",
        endDate: "2013",
        summary:
          "As part of the Audit, Valuation, & Analytics (AVA) group our team helped clients organize and analyze their data.",
        website: "https://www2.deloitte.com/us/en.html",
        highlights: [
          "Used tools: MS Excel, VBA, SAS, and ACL to bring reconcile data and bring insights to clients",
        ],
      },
    ],
    volunteer: [],
    education: [
      {
        institution: "Virginia Tech",
        area: "Business Information Technology",
        studyType: "Bachelor",
        startDate: "2009-08-01",
        endDate: "2011-05-01",
        courses: [],
      },
    ],
    awards: [],
    publications: [],
    skills: [
      {
        name: "Web Development",
        level: "Proficient",
        keywords: [
          "HTML",
          "CSS",
          "Javascript",
          "C#",
          "Java",
          "Powershell",
          "SQL",
        ],
      },
    ],
    languages: [
      {
        language: "English",
        fluency: "Native speaker",
      },
    ],
    interests: [
      {
        name: "Friends & Family",
        keywords: ["Fire pits", "Richmond"],
      },
      {
        name: "Art",
        keywords: ["Sketching", "Piano"],
      },
    ],
    references: [],
  };
</script>

<main>
  <section id="sticky-parallax-header">
    <h1>
      Hi, I'm {rez.basics.name}.
      <br />
      No, the honor is all mine!
    </h1>
  </section>
  <section class="work">
    <h2>
      Here is the stuff I did... (and still do but just soOoOo much better now!)
    </h2>
    <ul id="cards">
      {#each rez.work as job, index}
        <li class="card" id="card_{index}">
          <article>
            <h3>{job.position}</h3>
            <h4>{job.company}</h4>
            <p>{job.startDate} - {job.endDate}</p>
            <p>{job.summary}</p>
            <ul>
              {#each job.highlights as highlight}
                <li>{highlight}</li>
              {/each}
            </ul>
          </article>
        </li>
      {/each}
    </ul>
  </section>
  <section class="me">
    <h2>{rez.basics.label}</h2>
    <h2>{rez.basics.email}</h2>
    <h2>{rez.basics.phone}</h2>
  </section>
</main>

<style>
  @keyframes sticky-parallax-header-move-and-size {
    from {
      background-position: 50% 0;
      height: 100vh;
      font-size: calc(4vw + 1em);
    }
    to {
      background-position: 50% 100%;
      background-color: #0b1584;
      color: #fff;
      height: 13vh;
      font-size: 1rem;
    }
  }

  #sticky-parallax-header {
    position: fixed;
    top: 0;
    width: 100vw;

    animation: sticky-parallax-header-move-and-size linear forwards;
    animation-timeline: scroll();
    animation-range: 0vh 90vh;
  }

  .card {
    --index0: calc(var(--index) - 1); /* 0-based index */
    --reverse-index: calc(var(--numcards) - var(--index0)); /* reverse index */
    --reverse-index0: calc(
      var(--reverse-index) - 1
    ); /* 0-based reverse index */
  }

  @keyframes scale {
    to {
      transform: scale(calc(1.1 - calc(0.1 * var(--reverse-index))));
    }
  }

  #cards {
    --numcards: 4;
    view-timeline-name: --cards-element-scrolls-in-body;
  }

  .card__content {
    --start-range: calc(var(--index0) / var(--numcards) * 100%);
    --end-range: calc((var(--index)) / var(--numcards) * 100%);

    animation: linear scale forwards;
    animation-timeline: --cards-element-scrolls-in-body;
    animation-range: exit-crossing var(--start-range) exit-crossing
      var(--end-range);
  }
  main {
    padding-top: 133vh;
    font-family: Arial, sans-serif;
  }

  /* Print styles */
  @media print {
    main {
      font-size: 12pt;
      line-height: 1.5;
      color: #000;
      max-width: 100%;
      padding: 0;
    }

    h1 {
      font-size: 18pt;
      margin-bottom: 10pt;
    }

    h2 {
      font-size: 14pt;
      margin-top: 15pt;
      margin-bottom: 5pt;
    }

    p,
    li {
      orphans: 3;
      widows: 3;
    }

    /* Hide unnecessary elements for print */
    nav,
    footer,
    button {
      display: none !important;
    }

    /* Ensure background colors and images are printed */
    * {
      -webkit-print-color-adjust: exact;
      print-color-adjust: exact;
    }
  }
</style>
