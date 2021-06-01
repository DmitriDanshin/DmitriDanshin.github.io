<template>
  <section class="about">
    <div class="container">
      <div class="about__wrapper">

        <div class="about__descr">
          <h2 class="title title_fz36">ABOUT ME</h2>
          <div class="divider"></div>
          <p class="about__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
            incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
            laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
            esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
            qui officia deserunt mollit anim id est laborum</p>
        </div>
        <div class="about__skills">
          <div class="about__skills-item">
            <div class="about__skills-circle">
              <img src="../../assets/images/icons/about_me/web_development.svg" alt="web-dev">
            </div>
            <div>
              <div class="title title_fz14">Web-development</div>
              <div class="about__skills-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </div>
          </div>
          <div class="about__skills-item">
            <div class="about__skills-circle">
              <img src="../../assets/images/icons/about_me/design.svg" alt="design">
            </div>
            <div>
              <div class="title title_fz14">UI/UX Design</div>
              <div class="about__skills-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </div>
          </div>
          <div class="about__skills-item">
            <div class="about__skills-circle">
              <img src="../../assets/images/icons/about_me/mobile_dev.svg" alt="mobile">
            </div>
            <div>
              <div class="title title_fz14">Application Development</div>
              <div class="about__skills-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "About-block"
}
</script>

<style scoped>
@import "about.scss";
</style>