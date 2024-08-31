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
        colors: ["#0c2174", "#fff", "#c7001f"],
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
          "Lead engineer for team that created a software governance application that increases compliance and time to market for 1,000's of developers",
          "Created entire end-to-end functional test suite using Playwright, increasing speed of test cycle from 30 mins down to 1 min",
          "Led team that placed in the top 5 for our company's internal MS Teams Application hackathon",
          "In charge of a team of 10 developers where we moved application builds from local machines to jenkins, providing best practices for security, compliance, scanning, and deployment",
          "Facilitated cloud-to-cloud migration to Azure for suite of microservices, bringing our applications into compliance with company standards",
          "Engineered a tool to automate A11Y scans & aggregation of findings using Selenium for .NET before the company had a solution in place",
        ],
      },
      {
        colors: ["#225fb2", "#fff", "#225fb2"],
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
          "Managed the cloud migration for 4 client windows applications to AWS using terraform",
          "Developed scripts and jobs to provision windows host servers using Powershell DSC",
          "Automated internal API challenge framework, increasing company consultant knowledge of API experties",
        ],
      },
      {
        colors: ["#b5211d", "#d9dddf", "#b5211d"],
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
          "Designed, developed, documented, and deployed an application for market exposure reporting with rich UI table interactivity (saving precious user time)",
          "Built and maintained .NET applications for trading & portfolio management processes",
          "Increased test coverage from 0% to 100% on one of our primary trading applications, identifying and fixing many bugs",
          "Automated deployment and server provisioning for multiple applications, eliminating human error and saving hours per deployment",
        ],
      },
      {
        colors: ["#0c2174", "#fff", "#c7001f"],
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
          "Provided support for our online hosted payment solution which completed 1,000's of transactions monthly",
          "In charge of supplying transactional reporting on a daily & monthly basis for our customers, involving stored procedures, API endpoints, and batch jobs",
          "Developed & maintained web API for our peer-to-peer payment platform",
          "Contributed to our SDK for our consumer-to-business payment platform",
        ],
      },
      {
        colors: ["#86bc24", "#0f0b0b", "#1e3a51"],
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
          "Managed the daily calculations for client financials and provided statistical analysis",
          "Wrote VBA code behind Excel multiple spreadsheets to automate the monthly close process, saving 16+ hours every month",
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
</script>

<svelte:window bind:scrollY />
<!-- 

[x] I would make your "No, the honor is all mine" a little 
  smaller and maybe a different color so it all doesn't blend together.

[ ] When if first loads on my laptop the words kind of run off the
  right of the screen (more padding maybe)

[ ] Make sure the emojis are centered to the text.

[x] The words and imaged below the cards are 
  hard to read and the images are not loading?

[ ] Mobile would be great to have a similar effect on
 the cards where they are large but then move 
 into the background when you scroll.

[x] Might want to try not having the dark bar at the 
  top but the words changing is a keeper, 
  but having it on the blue background would be more modern/clean
-->
<header id="sticky-parallax-header">
  {#if scrollY < 615}
    <h1 class="fade-in">
      Hi, I'm {rez.basics.name}.
      <br />
      <span> No, the honor is all mine! </span>
    </h1>
  {:else if scrollY >= 615 && scrollY < 2000}
    <h1 class="fade-in">Stuff I've done... and still do!</h1>
  {:else if scrollY >= 2000 && scrollY < 3000}
    <h1 class="fade-in">A long time ago, in a cubicle far, far away...</h1>
  {:else}
    <h1 class="fade-in">Thanks for scrolling!</h1>
  {/if}
</header>
<main class="font-regular">
  <section class="work">
    <ul id="cards">
      {#each rez.work as job, index}
        <li class="card" id="card_{index}">
          <article class="card__content">
            <div class="highlights">
              <h3 class="font-header">
                {job.position},
                <a href={job.website} target="_blank">
                  {job.company}
                </a>
                ({job.startDate} - {job.endDate})
              </h3>
              <p>{job.summary}</p>
              <ul>
                {#each job.highlights as highlight}
                  <li>{highlight}</li>
                {/each}
              </ul>
            </div>
            <div class="brand">
              <div
                style="--company-color-1: {job.colors[0]};"
                class="company-color-1"
              ></div>
              <div
                style="--company-color-2: {job.colors[1]};"
                class="company-color-2"
              ></div>
              <div
                style="--company-color-3: {job.colors[2]};"
                class="company-color-3"
              ></div>
            </div>
            <!-- <img src="images/{job.pic}" alt={job.picAlt} /> -->
          </article>
        </li>
      {/each}
    </ul>
  </section>
  <section class="filler"></section>
</main>
<footer class="me">
  <!-- <EmailLink
    email={rez.basics.email}
    subject="Hi Trey"
    body="We would like you to help with our current project..."
  />
  <CallLink phoneNumber={rez.basics.phone} displayName={rez.basics.name} />
  <h2>{rez.basics.label}</h2>
  <div class="me__gallery">
    </div> -->
  <div class="solar-system">
    <div class="center">
      <img src="images/profile.jpg" alt="me" />
    </div>
    <div class="orbit">
      <div style="--delay: 0s;" class="planet planet1">
        <svg
          width="100"
          height="100"
          viewBox="0 0 100 100"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            x="10"
            y="20"
            width="80"
            height="60"
            rx="5"
            ry="5"
            fill="#ccc"
          />
          <rect x="15" y="25" width="70" height="45" fill="#333" />
          <text
            x="25"
            y="50"
            font-family="monospace"
            font-size="14"
            fill="#0f0"
          >
          </text>
          <rect x="40" y="80" width="20" height="5" fill="#ccc" />
        </svg>
      </div>
      <div style="--delay: 3s;" class="planet planet2">
        <svg
          width="100"
          height="100"
          viewBox="0 0 100 100"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            x="10"
            y="20"
            width="80"
            height="60"
            rx="5"
            ry="5"
            fill="#f0f0f0"
            stroke="#333"
            stroke-width="2"
          />
          <polyline
            points="10,20 50,50 90,20"
            fill="none"
            stroke="#333"
            stroke-width="2"
          />
        </svg>
      </div>
      <div style="--delay: 6s;" class="planet planet3">
        <svg
          width="100"
          height="100"
          viewBox="0 0 100 100"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M20,80 Q30,90 40,80 L60,40 Q70,30 80,40 L70,20 Q60,10 50,20 L30,60 Q20,70 20,80 Z"
            fill="#333"
          />
        </svg>
      </div>
    </div>
  </div>
</footer>

<style>
  :root {
    --delay: 0s;
    --gunmetal: #122c34ff;
    --indigo-dye: #224870ff;
    --marian-blue: #2a4494ff;
    --picton-blue: #4ea5d9ff;
    --robin-egg-blue: #44cfcbff;
    --scroll-animation-top-padding: 122vh;
    --clr-bg: var(--marian-blue);
    --list-style-type: "\\1F389";
  }
  @keyframes orbit {
    0% {
      transform: translate3d(0px, 0px, 500px) scale(1.5);
    }
    20% {
      transform: translate3d(495px, -195px, 200px) scale(1);
    }
    25% {
      transform: translate3d(500px, -200px, 200px) scale(1);
    }
    30% {
      transform: translate3d(495px, -205px, 200px) scale(1);
    }

    50% {
      transform: translate3d(0px, -500px, 0px) scale(0.5);
    }
    75% {
      transform: translate3d(-500px, -200px, 200px) scale(1);
    }
    100% {
      transform: translate3d(0px, 0px, 500px) scale(1.5);
    }
  }

  .solar-system {
    position: relative;
    width: 300px;
    height: 300px;
  }
  .solar-system img {
    border-radius: 100%;
    width: 25vw;
  }

  .center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .orbit {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    animation: orbit 10s ease-in infinite;
  }
  .orbit:hover {
    cursor: pointer;
    animation-play-state: paused;
  }

  .planet {
    position: absolute;
    width: 50px;
    height: 50px;
    top: 0;
  }

  .planet svg {
    width: 100%;
    height: 100%;
  }

  .company-color-1 {
    background-color: var(--company-color-1);
    clip-path: polygon(0% 0, 100% 0%, 100% 59%);
  }
  .company-color-2 {
    background-color: var(--company-color-2);
    clip-path: polygon(30% 0, 100% 0%, 115% 50%);
  }
  .company-color-3 {
    background-color: var(--company-color-3);
    clip-path: polygon(58% 0, 100% 0%, 100% 25%);
  }
  h1 span {
    font-size: 0.8em;
    color: #cbe6fa;
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
      background-color: var(--clr-bg);
      color: #fff;
      height: 5rem;
      font-size: 1rem;
    }
  }

  #sticky-parallax-header {
    position: fixed;
    top: 0;
    width: 98vw;

    animation: sticky-parallax-header-move-and-size linear forwards;
    animation-timeline: scroll();
    animation-range: 0vh 90vh;

    padding-left: 1.2rem;
    padding-right: 1.2rem;
    z-index: 9999;
  }

  .card {
    position: sticky;
    top: calc(160px + (16px * var(--index)));

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
  #card_0 .card__content .highlights ul {
    list-style-type: "\1F449";
  }
  #card_1 {
    --index: 1;
  }
  #card_1 .card__content .highlights ul {
    list-style-type: "\1F4E2";
  }
  #card_2 {
    --index: 2;
  }
  #card_2 .card__content .highlights ul {
    list-style-type: "\1F680";
  }
  #card_3 {
    --index: 3;
  }
  #card_3 .card__content .highlights ul {
    list-style-type: "\1F44C";
  }
  #card_4 {
    --index: 4;
  }
  #card_4 .card__content .highlights ul {
    list-style-type: "\1F389";
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
    height: 41rem;

    overflow: hidden;
    display: grid;
    grid-template-areas: "text img";
    grid-template-columns: 75% 1fr;
    grid-template-rows: auto;
    align-items: stretch;
    transform-origin: 50% 0%;
    will-change: transform;
  }
  .card__content .brand {
    grid-area: img;
    width: 100%;
    height: 100%;
    position: relative;
  }
  .card__content .brand div {
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  .card__content .highlights {
    grid-area: text;
    padding: 2rem;
  }
  .card__content .highlights h3 {
    font-size: 1.8rem;
    margin-bottom: 0.5rem;
  }
  .card__content .highlights p {
    font-size: 1.4rem;
  }
  .card__content .highlights li {
    font-size: 1.2rem;
    padding-left: 0.6rem;
    padding-bottom: 0.5rem;
    line-height: 1.7rem;
  }
  .card__content .highlights li::marker {
    font-size: 2rem;
  }
  main {
    padding-top: var(--scroll-animation-top-padding);
    background-color: var(--clr-bg);
  }
  .filler {
    height: 40vh;
    background-color: var(--clr-bg);
  }
  footer.me {
    padding-top: 30vh;
    padding-left: 30vw;
    background-color: var(--clr-bg);
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 36rem 36rem;
    place-items: center;
    place-content: center;
    background: linear-gradient(
      170deg,
      var(--marian-blue) 45%,
      var(--picton-blue) 75%,
      var(--robin-egg-blue) 100%
    );
  }
  .me .me__gallery {
    width: 100%;
    height: 100%;
    position: relative;
  }
  .me .me__gallery img {
    width: 24rem;
    border-top-left-radius: 12px;
    position: absolute;
    bottom: 0;
    right: 0;
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
