<template>
  <div class="profile-container">
    <div class="profile-header">
      <q-avatar size="100px" color="purple" text-color="white">
        <img src="../assets/My picture.png" />
      </q-avatar>
      <h4 style="margin-left: 3%">Likhitha Reddy</h4>
    </div>
    <div class="profile-content">
      <q-tabs v-model="tab" class="text-primary">
        <q-tab name="About">About Myself</q-tab>
        <q-tab name="Education">Education</q-tab>
        <q-tab name="Interests">Interests</q-tab>
        <q-tab name="Next">Next</q-tab>
      </q-tabs>
      <q-tab-panels v-model="tab" animated transition="slide">
        <q-tab-panel name="About">
          <div class="section-title">About</div>
          <p>Hi, I'm Chitla Likhitha Reddy.</p>
          <p>I'm from Hyderabad, India.</p>
          <p>I have completed my education from Hyderabad.</p>
        </q-tab-panel>
        <q-tab-panel name="Education">
          <div class="section-title">Education</div>
          <p>I have a Bachelor's degree in Computer Science Engineering.</p>
          <p>Graduated from CMR Institute of Technology, Hyderabad.</p>
        </q-tab-panel>
        <q-tab-panel name="Interests">
          <div class="section-title">Interests</div>
          <p>
            Apart from studies i'm intersted in designing, i do interior
            designing and fashion designing and sketching.
          </p>
          <p>Badminton is my favorite sport.</p>
        </q-tab-panel>
        <q-tab-panel name="Next">
          <div class="section-title"></div>
          <p>
            <b><h5>THANK YOU!!!! :-)</h5></b>
          </p>
        </q-tab-panel>
      </q-tab-panels>
    </div>
  </div>
</template>
<script>
import { ref } from "vue";
export default {
  setup() {
    const tab = ref("About Myself");
    return {
      tab,
    };
  },
};
</script>
<style scoped>
.profile-container {
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  background-color: hwb(0 96% 4%);
  border-radius: 8px;
}
.profile-header {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}
.profile-header h3 {
  margin-left: 10px;
}
.profile-content .section-title {
  font-size: 1.2rem;
  font-weight: bold;
  margin-top: 20px;
}
.profile-content p {
  margin: 10px 0;
}
</style>
