<template>
  <div>
    <nav>
      <ul id="navigation" v-bind:class="isActive && `active`">
        <li><a href="#about-me">About Me</a></li>
        <li><a href="#work-experience">Work Experience</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact-me">Contact Me</a></li>
      </ul>
    </nav>
    <div @click="toggleMenu()" v-bind:class="isActive ? `menu-btn disabled` : `menu-btn`">
      <div class="menu-btn__burger" id="burger1"></div>
      <div class="menu-btn__burger" id="burger2"></div>
      <div class="menu-btn__burger" id="burger3"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navigation",
  data: () => {
    return ({
      isActive: false,
    })
  },
  methods: {
    toggleMenu() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

