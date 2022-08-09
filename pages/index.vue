<template>
  <div>
    <Head>
      <Title>Dripada</Title>
      <Meta name="description" content="Dripada site" />
    </Head>
    <NavigationBar />
    <header>
      <div class="container-lg">
        <div class="row align-items-start justify-content-between">
          <div class="col-lg-5 col-12">
            <img
              src="@/assets/icons/person.svg"
              class="img-fluid"
              alt="Person"
            />
          </div>

          <div class="col-lg-6 col-12">
            <h1 class="text-center">Welcome To Dripada</h1>
            <h2 class="text-center">Complete Tasks and Earn ADA</h2>
            <div class="row-item">
              <NuxtLink
                class="learn-more"
                to="https://t.me/dripadacommunity"
                target="_blank"
                >Learn more</NuxtLink
              >
              <NuxtLink
                class="start-earning"
                to="https://resources.dripada.com/what-is-dripada/how-does-it-work"
                target="_blank"
                >Start Earning</NuxtLink
              >
            </div>
          </div>
        </div>
      </div>
    </header>

    <div id="about-us" class="our-mission">
      <div class="container-fluid">
        <div class="row align-items-center justify-content-between">
          <div class="col-lg-6 col-sm-7 col-12">
            <h2>
              Our mission is to build your business with our community through a
              Creative method of engagement.
            </h2>
            <div class="learn-engage-earn">
              <h2>Learn, Engage And Earn</h2>
              <p>
                Learn about new and innovative projects on the Cardano
                blockchain and get rewarded for that.
              </p>
            </div>
          </div>
          <div class="col-lg-6 col-sm-5 col-12">
            <img src="@/assets/icons/phone.svg" class="img-fluid" alt="Phone" />
          </div>
        </div>
      </div>
    </div>
    <div class="promote-engage">
      <div class="text-center heading">
        <h2>
          Promote & Engage In The Most Innovative projects, NFTs & metaverse
          ideas on the Cardano blockchain.
        </h2>
      </div>

      <div class="card-container">
        <div class="engage-card">
          <img src="@/assets/icons/engage-card-one.svg" alt="Avaliable Offer" />
        </div>
        <div class="engage-card">
          <img src="@/assets/icons/engage-card-two.svg" alt="Commission" />
        </div>
        <div class="engage-card">
          <img src="@/assets/icons/engage-card-three.svg" alt="Earning" />
        </div>
      </div>
    </div>

    <div class="security">
      <div class="container-lg">
        <div class="row align-items-center justify-content-center">
          <div class="col-lg-7 col-sm-6 col-12">
            <h2 class="text-lg-start text-center">
              We List Only Reputable Projects
            </h2>
            <p>
              All Dripada offers will be community verified and vetted so you
              can rest assured that you’re always interacting with quality
              projects.
            </p>
          </div>
          <div class="col-lg-5 col-sm-5 col-12 text-lg-start text-center">
            <img
              src="@/assets/icons/security.svg"
              class="img-fluid"
              alt="Security"
            />
          </div>
        </div>

        <div class="text-center join">
          <h2>Join Dripada in a few simple steps.</h2>
        </div>

        <div class="row align-items-center justify-content-center">
          <div class="col-lg-5 col-sm-6 col-12">
            <div class="border">
              <div class="row-item">
                <img src="@/assets/icons/visit.svg" alt="Visit" />
                <h5>Visit Dripada website</h5>
              </div>
            </div>
          </div>
          <div class="col-lg-5 col-sm-6 col-12">
            <div class="border">
              <div class="row-item">
                <img
                  src="@/assets/icons/choose_an_offer.svg"
                  alt="Choose Offer"
                />
                <h5>Choose an offer</h5>
              </div>
            </div>
          </div>
          <div class="col-lg-5 col-sm-6 col-12">
            <div class="border">
              <div class="row-item">
                <img
                  src="@/assets/icons/complete_task.svg"
                  alt="Complete Task"
                />
                <h5>Complete Tasks</h5>
              </div>
            </div>
          </div>
          <div class="col-lg-5 col-sm-6 col-12">
            <div class="border">
              <div class="row-item">
                <img src="@/assets/icons/get_rewarded.svg" alt="Rewarded" />
                <h5>Get Rewarded In ADA</h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="multiple-ways-to-earn">
      <div class="row-item">
        <div class="line"></div>
        <h2>Multiple ways to earn</h2>
        <div class="line"></div>
      </div>
      <div class="container-row">
        <div class="card-one">
          <div class="row-item">
            <h1>1</h1>
            <span class="box"></span>
          </div>
          <h4>Engage To Earn</h4>
          <p>
            This works using cost per engagement, as you take action which could
            be filling out a form with verified details, making a tweet or
            purchasing an NFT. The more advanced the action, the higher your
            payout.
          </p>
        </div>
        <div class="card-two">
          <div class="row-item">
            <h1>2</h1>
            <span class="box"></span>
          </div>
          <h4>Refer To Earn</h4>
          <p>
            Refer and Earn – the easiest way to rack up earning points is to
            send your referrals to our project offers on a Cost Per Lead basis.
          </p>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
<script setup>
const menuHandler = () => {
  const navItem = document.querySelector(".nav-item-list");

  navItem.classList.toggle("active");
};
</script>

<style>
</style>