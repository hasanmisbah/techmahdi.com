<template>
  <section id="about">
    <div class="container is-fluid">
      <div class="page-title">
        <h1>About</h1>
      </div>
      <div class="container is-flex">
        <div class="columns">
          <div class="column is-6">
            <div class="profile-photo-images">
              <div class="images"></div>
            </div>
          </div>
          <div class="column is-6">
            <b-tabs>
              <b-tab-item label="About Me" icon="google-photos">
                <p>
                  <strong>Who am I?</strong>
                </p>
                <p>
                  I am a software engineer, currently working at Collectors Abode & Centava.
                  Native Android and Flutter are my TOP skills in mobile development. I have more than 2 years of experience in creating Native Apps on the Android platform. For Web development, I am familiar with frontend technologies - HTML/CSS/Javascript, as well as React JS to operate with WordPress. Furthermore, I have basic experience with a wide range of programming languages and technologies, such as Java, C++, C and Dart. I have worked with NoSQL database systems, such as Firebase and I can operate with PHP/MySQL Database systems.
                  Most applications I have developed from scratch, so I know how to design application architecture and write clean and simple code. In addition, I have maintained legacy code and am very familiar with debugging and refactoring.
                </p>
                <p>I understand the main principles for creating successful application design (SOLID, OOP, OOD), I have experience with all required development tools and of course with all common WEB technologies. I try to be aware of trending technologies, not limiting to Android but also ios and WEB. I'm self-motivated, a quick learner and a good team player</p>
                <p>
                  <strong>What am I like?</strong>
                </p>
                <p>
                  The people I’ve worked with would describe me as a positive, optimistic, friendly, flexible and hard-working person. I am a team player who can handle work under pressure and calmly resolve any urgent or unpredictable problems.
                  I always try to keep the code quality with bug free, best app performance and long term maintenance.
                </p>
                <p>
                  <strong>Next steps?</strong>
                </p>
                <p>Contact me and let's discuss about your project</p>
              </b-tab-item>
              <b-tab-item label="Profile" icon="library-music">
                <div class="profile">
                  <p>
                    <strong>Name</strong> : Amimul Ihsan
                  </p>
                  <p>
                    <strong>Nationality</strong> : Bangladeshi
                  </p>
                  <p>
                    <strong>Email</strong> : amimulihsan@techmahdi.com
                  </p>
                  <p>
                    <strong>Date of birth</strong> : 12-07-1996
                  </p>
                  <p>
                    <strong>Phone</strong> : +880-1789 93 75 76
                  </p>
                </div>
              </b-tab-item>
              <b-tab-item label="Skill" icon="video">
                <div class="skillbar">
                  <p>Java</p>
                  <b-progress type="is-success" :value="80"></b-progress>
                </div>
                <div class="skillbar">
                  <p>xml</p>
                  <b-progress type="is-success" :value="90"></b-progress>
                </div>
                <div class="skillbar">
                  <p>Firebase</p>
                  <b-progress type="is-success" :value="70"></b-progress>
                </div>
                <div class="skillbar">
                  <p>Flutter</p>
                  <b-progress type="is-success" :value="60"></b-progress>
                </div>
                <div class="skillbar">
                  <p>php/mySql</p>
                  <b-progress type="is-success" :value="60"></b-progress>
                </div>
                <div class="skillbar">
                  <p>HTML, CSS, JS</p>
                  <b-progress type="is-success" :value="60"></b-progress>
                </div>
                <div class="skillbar">
                  <p>Wordpress</p>
                  <b-progress size="is-medium" show-value type="is-success" :value="60">50%</b-progress>
                </div>
              </b-tab-item>
            </b-tabs>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  head() {
    return {
      title: "About Me || Amimul Ihsan Mahdi"
    };
  }
};
</script>

<style lang="scss">
#about {
  overflow: hidden;
  .skillbar {
    p {
      color: #333;
      margin: 8px 0;
      line-height: 18px;
      font-size: 14px;
      letter-spacing: 0.4px;
    }
  }
  .page-title {
    h1 {
      &::before {
        content: "about";
      }
    }
  }
  .columns {
    width: 100%;
  }
  .profile {
    p {
      line-height: 1.6;
      margin-bottom: 10px;
    }
  }
  .profile-photo-images {
    .images {
      background-image: url("../assets/images/amimulislammahdi.jpg");
      height: 350px;
      width: 85%;
      margin: auto;
      border-radius: 5px;
      margin-bottom: 50px;
      transition: all 500ms ease-in-out;
      background-position: center center;
      background-size: cover;
      background-repeat: no-repeat;
      margin-left: 0;
    }
  }
}
</style>