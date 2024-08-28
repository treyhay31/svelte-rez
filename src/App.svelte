<script>
  //TODO: create svg in procreate for favicon and maybe other images on the site
  //TODO: find profile picture of me being old
  import CallLink from "./components/CallLink.svelte";
  import EmailLink from "./components/EmailLink.svelte";
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
        "I'll solve your problems, I'll motivate your team members, and I'll do it all with a GREAT attitude! I love working hard and I love encouraging my teammates! When everyone can work together towards putting a smile on the customer's face, we all WIN!",
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
        pic: "usbank-dark.png",
        picAlt: "U.S. Bank logo",
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
        pic: "captech-dark.png",
        picAlt: "CapTech logo",
        position: "Senior Consultant",
        company: "CapTech",
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
        pic: "dfa.jpg",
        picAlt: "Dimensional Fund Advisors logo",
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
        pic: "usbank-dark.png",
        picAlt: "U.S. Bank logo (acquired ETS)",
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
        pic: "deloitte.png",
        picAlt: "Deloitte logo",
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
          "Bash",
          "Python",
          "Batch",
        ],
      },
      {
        name: "DevOps",
        level: "Proficient",
        keywords: [
          "Jenkins",
          "Terraform",
          "Docker",
          "Kubernetes",
          "VirtualBox",
        ],
      },
      {
        name: "Testing",
        level: "Proficient",
        keywords: [
          "Playwright",
          "Selenium",
          "Jest",
          "XUnit",
          "MSTest",
          "Postman",
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
  let scrollY;
  // $: console.log(scrollY);
  let randomNumber = Math.floor(Math.random() * 6);
  const profilePics = [
    "profile-1.png",
    "profile-2.png",
    "profile-3.png",
    "profile-4.png",
    "profile-5.png",
    "profile-6.jpg",
  ];
  console.log(randomNumber, profilePics[randomNumber]);
</script>

<svelte:window bind:scrollY />

<header id="sticky-parallax-header">
  {#if scrollY < 615}
    <h1 class="fade-in">
      Hi, I'm {rez.basics.name}.
      <br />
      No, the honor is all mine!
    </h1>
  {:else if scrollY >= 615 && scrollY < 1600}
    <h1 class="fade-in">Stuff I've done... and still do!</h1>
  {:else if scrollY >= 1600 && scrollY < 2400}
    <h1 class="fade-in">This is the stuff I have a hard time remembering</h1>
  {:else}
    <h1 class="fade-in">...That's about it!</h1>
  {/if}
</header>
<main>
  <section class="work">
    <ul id="cards">
      {#each rez.work as job, index}
        <li class="card" id="card_{index}">
          <article class="card__content">
            <div>
              <h3>
                {job.position}, {job.company}
                ({job.startDate} - {job.endDate})
              </h3>
              <p>{job.summary}</p>
              <ul>
                {#each job.highlights as highlight}
                  <li>{highlight}</li>
                {/each}
              </ul>
            </div>
            <img src="images/{job.pic}" alt={job.picAlt} />
          </article>
        </li>
      {/each}
    </ul>
  </section>
  <section class="filler"></section>
</main>
<footer class="me">
  <div class="me__gallery">
    <img src="images/{profilePics[randomNumber]}" alt="me" />
  </div>
  <h2>{rez.basics.label}</h2>
  <EmailLink
    email={rez.basics.email}
    subject="Hi Trey"
    body="We would like you to help with our current project"
  />
  <CallLink phoneNumber={rez.basics.phone} displayName={rez.basics.name} />
</footer>

<style>
  :root {
    --gunmetal: #122c34ff;
    --indigo-dye: #224870ff;
    --marian-blue: #2a4494ff;
    --picton-blue: #4ea5d9ff;
    --robin-egg-blue: #44cfcbff;
    --scroll-animation-top-padding: 122vh;
    --clr-bg: var(--marian-blue);
  }
  .fade-in {
    -webkit-animation: fade-in 1.2s cubic-bezier(0.39, 0.575, 0.565, 1) 0.5s
      both;
    animation: fade-in 1.2s cubic-bezier(0.39, 0.575, 0.565, 1) 0.5s both;
  }
  .fade-out {
    -webkit-animation: fade-in 1.2s cubic-bezier(0.39, 0.575, 0.565, 1) 0.5s
      reverse both;
    animation: fade-in 1.2s cubic-bezier(0.39, 0.575, 0.565, 1) 0.5s reverse
      both;
  }
  @-webkit-keyframes fade-in {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
  @keyframes fade-in {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

  @keyframes sticky-parallax-header-move-and-size {
    from {
      background-position: 50% 0;
      height: 100vh;
      font-size: calc(4vw + 1em);
      color: #fdfd66;
    }
    to {
      background-position: 50% 100%;
      background-color: var(--gunmetal);
      color: #fff;
      height: 12vh;
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

    padding-left: 1.2rem;
    z-index: 9999;
  }

  .card {
    position: sticky;
    top: 16vh;

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
    --numcards: 5;
    view-timeline-name: --cards-element-scrolls-in-body;
    list-style: none;
    /* padding-top: calc(var(--scroll-animation-top-padding)); */
  }

  #card_0 {
    --index: 0;
  }
  #card_1 {
    --index: 1;
  }
  #card_2 {
    --index: 2;
  }
  #card_3 {
    --index: 3;
  }
  #card_4 {
    --index: 4;
  }

  .card__content {
    --start-range: calc(var(--index0) / var(--numcards) * 100%);
    --end-range: calc((var(--index)) / var(--numcards) * 100%);

    animation: linear scale forwards;
    animation-timeline: --cards-element-scrolls-in-body;
    animation-range: exit-crossing calc(10vh + --scroll-animation-top-padding);

    box-shadow:
      0 0.2em 1em rgba(0, 0, 0, 0.1),
      0 1em 2em rgba(0, 0, 0, 0.1);
    background: rgb(255, 255, 255);
    color: rgb(10, 5, 7);
    border-radius: 1em;

    overflow: hidden;
    display: grid;
    grid-template-areas: "text img";
    grid-template-columns: 1fr 1fr;
    grid-template-rows: auto;
    align-items: stretch;
    transform-origin: 50% 0%;
    will-change: transform;
  }
  .card__content img {
    grid-area: img;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .card__content div {
    grid-area: text;
    padding: 2rem;
  }
  main {
    padding-top: var(--scroll-animation-top-padding);
    font-family: Arial, sans-serif;
    background-color: var(--clr-bg);
  }
  .filler {
    height: 60vh;
    background-color: var(--clr-bg);
  }
  footer.me {
    background-color: var(--clr-bg);
    padding-bottom: 55vh;
    padding-top: 33vh;
    display: grid;
    grid-template-columns: 1fr;
  }
  .me .me__gallery {
    position: relative;
    height: 100vh;
  }
  .me .me__gallery img {
    border-radius: 100%;
    position: absolute;
    width: 24rem;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
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
