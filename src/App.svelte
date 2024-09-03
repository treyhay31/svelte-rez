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
      label: "Dev",
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
      Hi, I'm {rez.basics.name}
      <br />
      <span> No, the honor is all mine! </span>
    </h1>
  {:else if scrollY >= 615 && scrollY < 2000}
    <h1 class="fade-in">Stuff I've done... and still do!</h1>
  {:else if scrollY >= 2000 && scrollY < 3400}
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
  <div class="me__details">
    <img src="images/profile.png" alt="me" />
    <div class="me__details__panel-left">
      <h2>Software <br /> Engineer</h2>
    </div>
    <div class="me__details__panel-right">
      <EmailLink
        email={rez.basics.email}
        subject="Hi Trey"
        body="We would like you to help with our current project..."
      />
      <CallLink phoneNumber={rez.basics.phone} displayName={rez.basics.name} />
    </div>
  </div>
  <!-- <div class="solar-system">
    <div class="center">
      <img src="images/profile.png" alt="me" />
    </div>
    <div class="orbit">
      <div style="--delay: 0s;" class="planet planet1">
        <svg
          fill="#1C2033"
          width="52"
          height="52"
          version="1.1"
          id="lni_lni-phone-set"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          viewBox="0 0 64 64"
          style="enable-background:new 0 0 64 64;"
          xml:space="preserve"
        >
          <g>
            <path
              d="M60.2,55.2l-1.8-18.1c-0.3-3.3-3.1-5.8-6.4-5.8H12c-3.3,0-6,2.5-6.4,5.8L3.8,55.2c-0.2,1.8,0.4,3.6,1.6,4.9
		c1.2,1.3,2.9,2.1,4.7,2.1h43.6c1.8,0,3.5-0.8,4.7-2.1C59.8,58.8,60.3,57,60.2,55.2z M55.2,57.1c-0.4,0.4-0.9,0.6-1.4,0.6H10.2
		c-0.5,0-1-0.2-1.4-0.6c-0.4-0.4-0.5-0.9-0.5-1.5l1.8-18.1c0.1-1,0.9-1.7,1.9-1.7h40c1,0,1.8,0.7,1.9,1.7l1.8,18.1
		C55.7,56.2,55.6,56.7,55.2,57.1z"
            />
            <path
              d="M32,39.3c-4.1,0-7.5,3.4-7.5,7.5c0,4.2,3.4,7.5,7.5,7.5c4.2,0,7.5-3.4,7.5-7.5C39.5,42.7,36.2,39.3,32,39.3z M32,49.8
		c-1.7,0-3-1.4-3-3c0-1.7,1.4-3,3-3c1.7,0,3,1.4,3,3C35,48.5,33.7,49.8,32,49.8z"
            />
            <path
              d="M6.1,20.6c0.2,4.4,4,6.7,6.6,6.7c0,0,0,0,0,0l7,0c0,0,0.1,0,0.1,0c3.2-0.2,6.4-2.3,6.4-6.7l0-1.9c3.4,0,9.9,0,13.2,0l0,1.9
		c0,4.4,3.2,6.5,6.4,6.7c0,0,7.1,0,7.1,0c0,0,0,0,0,0c2.7,0,6.4-2.3,6.6-6.7c0-0.3,0-3.9,0-4.1c0-0.1,0-0.2,0-0.3
		c-0.3-2.9-1.3-5.3-3.1-7.2c0,0-0.1-0.1-0.1-0.1c-2.6-2.4-5.6-3.7-7.9-4.5c-6.8-2.6-15.3-2.6-15.7-2.6c0,0,0,0,0,0
		c-6,0.1-9.8,0.6-15.6,2.6c-2.4,0.9-5.4,2.2-8,4.5c0,0-0.1,0.1-0.1,0.1c-1.8,1.9-2.8,4.3-3.1,7.2c0,0.1,0,0.2,0,0.3
		C6,16.7,6.1,20.2,6.1,20.6z M12.3,12.2c2-1.8,4.4-2.8,6.4-3.6c5.2-1.9,8.5-2.2,14.1-2.4c0.5,0,8.1,0.1,14.1,2.4
		c2.1,0.8,4.5,1.8,6.4,3.6c1,1.1,1.6,2.6,1.8,4.3c0,0.3,0,3.6,0,3.9c-0.1,2.1-2.1,2.4-2.1,2.4l-6.9,0c-1-0.1-2.1-0.5-2.1-2.2l0-4.1
		c0-1-0.6-1.9-1.6-2.1C41.7,14,24,14,23.3,14.3c-0.9,0.3-1.6,1.2-1.6,2.1l0,4.2c0,1.7-1.1,2.1-2.1,2.2l-6.9,0c0,0-2-0.3-2.1-2.3
		c0-0.3,0-1.4,0-2.4c0-0.7,0-1.2,0-1.5C10.7,14.7,11.3,13.3,12.3,12.2z"
            />
          </g>
        </svg>
      </div>
      <div style="--delay: 3s;" class="planet planet2">
        <svg
          fill="#1C2033"
          width="52"
          height="52"
          version="1.1"
          id="lni_lni-code"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          viewBox="0 0 64 64"
          style="enable-background:new 0 0 64 64;"
          xml:space="preserve"
        >
          <g>
            <path
              d="M19.6,14.1c-0.9-0.8-2.4-0.7-3.2,0.2L2.6,29.9c-1.1,1.2-1.1,3.1,0,4.3l13.9,15.6c0.4,0.5,1.1,0.8,1.7,0.8
		c0.5,0,1.1-0.2,1.5-0.6c0.9-0.8,1-2.3,0.2-3.2L6.7,32l13.1-14.7C20.7,16.3,20.6,14.9,19.6,14.1z"
            />
            <path
              d="M61.4,29.9L47.5,14.3c-0.8-0.9-2.2-1-3.2-0.2s-1,2.2-0.2,3.2L57.3,32L44.2,46.7c-0.8,0.9-0.7,2.3,0.2,3.2
		c0.4,0.4,1,0.6,1.5,0.6c0.6,0,1.2-0.3,1.7-0.8l13.9-15.6C62.5,32.9,62.5,31.1,61.4,29.9z"
            />
            <path
              d="M37.9,14.4c-1.2-0.4-2.5,0.2-2.8,1.4L24.7,46.7c-0.4,1.2,0.2,2.5,1.4,2.8c0.2,0.1,0.5,0.1,0.7,0.1c0.9,0,1.8-0.6,2.1-1.5
		l10.3-30.9C39.7,16.1,39.1,14.8,37.9,14.4z"
            />
          </g>
        </svg>
      </div>
      <div style="--delay: 6s;" class="planet planet3">
        <svg
          fill="#1C2033"
          width="52"
          height="52"
          version="1.1"
          id="lni_lni-postcard"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          viewBox="0 0 64 64"
          style="enable-background:new 0 0 64 64;"
          xml:space="preserve"
        >
          <g>
            <path
              d="M56,11.9H8c-3.4,0-6.2,2.8-6.2,6.2v27.7c0,3.4,2.8,6.2,6.2,6.2h48c3.4,0,6.2-2.8,6.2-6.2V18.2C62.2,14.7,59.4,11.9,56,11.9
		z M57.8,45.8c0,1-0.8,1.8-1.8,1.8H8c-1,0-1.8-0.8-1.8-1.8V18.2c0-1,0.8-1.8,1.8-1.8h48c1,0,1.8,0.8,1.8,1.8V45.8z"
            />
            <path
              d="M32,20.9c-1.2,0-2.2,1-2.2,2.2v15.3c0,1.2,1,2.2,2.2,2.2c1.2,0,2.2-1,2.2-2.2V23.1C34.2,21.9,33.2,20.9,32,20.9z"
            />
            <path
              d="M11.6,33h8.9c1.2,0,2.2-1,2.2-2.2s-1-2.2-2.2-2.2h-8.9c-1.2,0-2.2,1-2.2,2.2S10.4,33,11.6,33z"
            />
            <path
              d="M52,20.9h-9.4c-1.5,0-2.6,1.2-2.6,2.6v9.4c0,1.4,1.2,2.6,2.6,2.6H52c1.4,0,2.6-1.2,2.6-2.6v-9.4C54.6,22,53.4,20.9,52,20.9
		z M50.1,31h-5.7v-5.7h5.7V31z"
            />
            <path
              d="M23,36.1H11.6c-1.2,0-2.2,1-2.2,2.2s1,2.2,2.2,2.2H23c1.2,0,2.2-1,2.2-2.2S24.3,36.1,23,36.1z"
            />
          </g>
        </svg>
      </div>
    </div>
  </div> -->
</footer>

<style>
  .me__details {
    position: relative;
    display: grid;
    grid-template-columns: 18rem 25rem;
    grid-template-rows: 25rem;
  }
  .me__details img {
    position: absolute;
    width: 21rem;
    left: 7rem;
    z-index: 10;
    border-radius: 1rem;
  }
  .me__details .me__details__panel-left {
    background: #fff;
    align-self: start;
    width: 18rem;
    border-radius: 1rem;
    margin-top: 7rem;
    padding-left: 1.5rem;
    margin-left: 2rem;
  }
  .me__details .me__details__panel-right {
    background: #fff;
    height: 19rem;
    width: 13rem;
    justify-self: start;
    align-self: end;
    border-top-right-radius: 100rem;
    border-bottom-right-radius: 100rem;
    display: grid;
    grid-template-rows: 1fr 1fr;
    place-content: center;
    place-items: center;
    margin-left: 2rem;
  }
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
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }

  .solar-system {
    position: relative;
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
    transform: rotate(45deg);
    width: 24rem;
    height: 24rem;
    animation: orbit 7s linear infinite;
  }
  .orbit:hover {
    cursor: pointer;
    animation-play-state: paused;
  }

  .planet {
    position: absolute;
    width: 6rem;
    height: 6rem;
  }

  @keyframes axis-spin {
    0% {
      transform: rotateZ(0deg);
    }
    100% {
      transform: rotateZ(360deg);
    }
  }

  @keyframes scale-in-out-left-right {
    0% {
      transform: scale(2);
      opacity: 1;
    }
    40%,
    50%,
    60% {
      transform: scale(0.5);
      opacity: 0;
    }
    100% {
      transform: scale(2);
      opacity: 1;
    }
  }
  .planet1 {
    left: 0;
    bottom: 0;
    animation: 7s linear axis-spin infinite;
  }
  .planet2 {
    right: 0;
    top: 0;
    animation: 7s linear axis-spin infinite;
  }
  .planet3 {
    right: 0;
    bottom: 0;
    animation: 7s linear axis-spin infinite;
  }
  .planet svg {
    width: 100%;
    height: 100%;
  }
  .planet1 svg {
    animation: 7s linear 1s scale-in-out-left-right infinite;
  }
  .planet2 svg {
    animation: 7s linear 3s scale-in-out-left-right infinite;
  }
  .planet3 svg {
    animation: 7s linear 6s scale-in-out-left-right infinite;
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
    font-size: 0.6em;
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
  .card__content .highlights ul {
    list-style: none;
  }
  .card__content .highlights ul li {
    position: relative;
    font-size: 1.4rem;
    padding-left: 2.6rem;
    padding-bottom: 2.5rem;
  }
  .card__content .highlights ul li::before {
    font-size: 3rem;
    position: absolute;
    top: 0.29rem;
    left: -2.2rem;
  }

  #card_0 {
    --index: 0;
  }
  #card_0 .card__content .highlights ul li::before {
    content: "\1F449";
  }
  #card_1 {
    --index: 1;
  }
  #card_1 .card__content .highlights ul li::before {
    content: "\1F4E2";
  }
  #card_2 {
    --index: 2;
  }
  #card_2 .card__content .highlights ul li::before {
    content: "\1F680";
  }
  #card_3 {
    --index: 3;
  }
  #card_3 .card__content .highlights ul li::before {
    content: "\1F44C";
  }
  #card_4 {
    --index: 4;
  }
  #card_4 .card__content .highlights ul li::before {
    content: "\1F389";
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
    height: 10rem;
    background-color: var(--clr-bg);
  }
  footer.me {
    height: 50rem;
    background-color: var(--clr-bg);
    display: grid;
    grid-template-columns: 80vw;
    place-items: center;
    place-content: center;
    background: linear-gradient(
      170deg,
      var(--marian-blue) 45%,
      var(--picton-blue) 75%,
      var(--robin-egg-blue) 100%
    );
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
