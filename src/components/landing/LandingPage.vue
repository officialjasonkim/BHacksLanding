<template>
  <v-layout class="d-inline">
    <header style="background: #80d2ff">
      <div class="container-fluid">
        <div class="row">
          <div class="col"></div>
          <div class="col-3 col-sm-2 col-lg-1">
            <a
              id="mlh-trust-badge"
              rel="noreferrer"
              href="https://mlh.io/seasons/na-2020/events?utm_source=na-hackathon&amp;utm_medium=TrustBadge&amp;utm_campaign=2020-season&amp;utm_content=gray"
              target="_blank"
            >
              <img
                src="https://s3.amazonaws.com/logged-assets/trust-badge/2020/mlh-trust-badge-2020-gray.svg"
                alt="Major League Hacking 2020 Hackathon Season"
                style="width: 70%"
              />
            </a>
          </div>
        </div>
      </div>
    </header>

    <div id="home" style="padding-bottom: 0px, margin-bottom: 0px">
      <v-container>
        <div class="flexc" style="justify-content: center">
          <h2
            style="font-size: 1.25rem; text-align: center; color: white; font-weight: bold"
          >
            We're turning 6.
            <br />
            And you're invited <br />
            to our virtual hackathon!
          </h2>
        </div>
        <div class="flexc" style="justify-content: center">
          <v-btn rounded depressed @click="login()"
            >Login</v-btn
          >
        </div>
      </v-container>
      <v-container>
        <div class="flexc" style="justify-content: space-around; height: 9rem">
          <img
            src="@/assets/landing/Feliz and Balloons.png"
            alt="pinata"
            height="300"
            style="margin: -9rem"
          />
          <div class="sponsor-flexc" style="width: 18rem">
            <div class="sponsor-info">
              <h2
                style="font-size: 1.25rem; text-align: center; color: white; font-weight: bold"
              >
                Interested in Sponsoring?
              </h2>
              <h2 style="font-size: 1rem; text-align: center; color: white; font-weight: normal">
                We’d love to have you on board. Contact us at
                sponsor@bostonhacks.io or check out our sponsor document!
              </h2>
              <div class="flexc" style="justify-content: center">
                <v-btn
                  depressed
                  rounded
                  @click="sponsor()"
                  >Learn more</v-btn
                >
              </div>
            </div>
          </div>
        </div>
      </v-container>
      <div class="curve1">

      </div>
    </div>


    <div id="tracks" style="margin-top: 0; padding-top: 0;">
      <v-container>
        <h2 class="display-1" style="color: white; text-align: center; font-weight: bold">
          Tracks and Work­shops
        </h2>
        <div class="flexc" style="justify-content: flex-end">
          <div class="tracks-info">
            <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Conservation for Society
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              Scientists continue to release research about the effects humans
              have on varying types of pollution. What can be done to facilitate
              research, increase awareness, lessen our carbon footprint, and in
              general just leave earth in a better state than we found it?
            </p>
          </div>
        </div>
        <div class="flexc" style="justify-content: center">
          <div class="tracks-info">
            <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Smart Home
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              Quarantine has us realizing that the home is not as efficient and
              optimized as it could be. How can we incorporate software and
              hardware to create a more comprehensive experience at home?
            </p>
          </div>
        </div>
        <div class="flexc" style="justify-content: flex-start">
          <div class="tracks-info">
            <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Fit-Tech
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              Current fitness tech encourages people to stay indoors (Peloton,
              online classes), or simply tracks data and provides analytics. How
              can we revamp fitness with technology that makes exercise more
              interactive and engaging, giving people more excuses to enjoy the
              outdoors?
            </p>
          </div>
        </div>
      </v-container>
    </div>

    <div id="schedule">
      <v-container> 
        <h2 class="display-1" style="color: white; text-align: center; font-weight: bold">
          Schedule
        </h2>
        <div class="schedulec">
          <div class="sevent" style="color: white">
            7:00AM Event Starts
          </div>
          <div class="sevent" style="color: white">
            8:00AM Event Continues
          </div>
          <div class="sevent" style="color: white">
            9:00AM Still Continues!
          </div>
        </div> 
      </v-container>
    </div>

    <div id="FAQ">
      <h2 class="display-1" style="color: white; text-align: center; font-weight: bold">Frequently Asked Questions</h2>
      <v-container class="faq-grid"> 
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              What is BostonHacks?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              BostonHacks is a 36-hour event where students from different backgrounds gather 
              together to use technology to create cool projects. Come to BostonHacks to expand
              your knowledge and skills, make new friends, win prizes and network with recruiters
              from our corporate sponsors! 
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              When and where is BostonHacks?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              BostonHacks is a virtual 36-hour hackathon on November 14-15th, 2020.
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Who can attend?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              All students including undergraduate, graduate and high school students 
              with any background, all across the world are welcome! 
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Do I need experience?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              No experience is necessary. We will have plenty of mentors and resources available, 
              along with several workshops targeted for beginners. Come learn and experience your 
              first hackathon at BostonHacks!
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Does it cost anything?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              BostonHacks is 100% free. You don’t have to spend a dime! Unfortunately, we won’t 
              be providing any travel reimbursements this year. 
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Can we form teams?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              Of course you can! We encourage people to work in teams of up to 5 people. You may 
              opt-in to team formation through our Slack Channel which will match you with an ideal 
              team. You can work alone, but it won’t be the same. 
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              Are there any rules?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              We want to ensure a positive experience for all participants. We encourage you to 
              read the Code of Conduct.
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              What do I need to bring?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              Remember it’s an overnight event! You should bring your laptop, phone, chargers. 
            </p>
        </div>
        <div class="qna">
          <h2 style="font-size: 1.25rem; color: white; font-weight: bold">
              What if I have a different question?
            </h2>
            <p
              style="font-size: 1rem; color: white; font-weight: normal"
            >
              We’re here for you! Shoot us an email at contact@bostonhacks.io, or a message on 
              any of our social media platforms. 
            </p>
        </div>
      </v-container>
    </div>
  </v-layout>
</template>

<script>
export default {
  computed: {
    user() {
      return this.$store.state.user;
    }
  },
  methods: {
    login() {
      this.$router.push("/login");
    },
    sponsor() {
      this.$router.push("/sponsor");
    }
  }
};
</script>

<style>
html {
  scroll-behavior: smooth;
}

#home {
  background: #80d2ff;
}

#tracks {
  background: #aee2ff;
}

#schedule {
  background: #53d186;
}

#FAQ {
  background: #e6c8bc;
}


.flexc {
  display: flex;
  margin: 1rem 1rem;
}

.tracks-info {
  width: 32rem;
}

.schedulec {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.sevent {
  text-align: center;
  padding: .5rem;
}

.faq-grid{
  display: grid;
  grid-template-columns: auto auto auto;
}

.qna {
  padding: 1.5rem;
}

.curve1 {

  height: 16rem !important;
  width: 100% !important;
  background: url('../../assets/landing/wave.svg') no-repeat center bottom/cover !important;
  background-size: 100% 16rem !important;

}

@media screen and (max-width: 768px) {
  .faq-grid{
    grid-template-columns: auto;
  }
}
</style>
