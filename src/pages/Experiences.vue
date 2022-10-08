<template>
  <div>
    <Navbar />
    <footer class="content margin-auto">
      <article style="color: aliceblue" class="text-center">
        <section>
          <span>"{{ motto2 }}"</span>
        </section>
        <section>
          <span>--- {{ author }} ---</span>
        </section>
        <hr />
        <div v-for="e in experiences" :key="e.title">
          <section class="title">
            <span>{{ e.title }}</span>
          </section>

          <article class="skill-menu margin-auto">
            <ul class="ul-navbar">
              <li class="menu-list">
                <a> {{ e.subtitle }} </a>
              </li>
              <li class="menu-list">
                <a> {{ e.subtitle2 }} </a>
              </li>
            </ul>
          </article>
        </div>
      </article>
    </footer>
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import axios from "axios";
//https://6341578520f1f9d79970eb42.mockapi.io/profile/v1/profilejava
export default {
  components: { Navbar },
  methods: {
    async fetchExperience() {
      try {
        let res = await axios.get(
          "https://6341578520f1f9d79970eb42.mockapi.io/profile/v1/profilejava"
        );
        this.experiences = res.data;
      } catch (error) {}
    },
  },
  data() {
    return {
      motto2: "Every accomplishment starts with the decision to try",
      author: "John F. Kennedy",
      experiences: [],
    };
  },
  beforeMount() {
    this.fetchExperience();
  },
};
</script>

<style>
</style>