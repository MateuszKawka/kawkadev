<template>
  <nav class="nav">
    <button class="nav__button">a</button>
    <ul class="menu">
      <li class="menu-item" v-for="(navItem, index) in navData" :key="`nav-item-${index}`">
        <a :href="navItem.href" class="menu-item__link">{{navItem.name}}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Navigation",
  data() {
    return {
      navData: [
        {
          name: "Start",
          href: ""
        },
        {
          name: "Exp",
          href: "#exp"
        },
        {
          name: "Works",
          href: "#works"
        },
        {
          name: "Skills",
          href: "#skills"
        },
        {
          name: "Contact",
          href: "#contact"
        }
      ]
    };
  },
  methods: {
    detectViewboxDistance() {
      
    },
    navHide() {
      const pos = window.pageYOffset;
      const menu = document.querySelector('.menu');
      const navigationButton = document.querySelector('.nav__button')
      menu.classList.toggle("menu--hide", pos > 100);
      navigationButton.classList.toggle("nav__button--show", pos > 100)
    }
  },
  mounted() {
     window.addEventListener("scroll",this.navHide)
  }
};
</script>

<style lang="scss" scoped>
.nav {
  width: 100%;
  display: flex;
  justify-content: center;
  position: fixed;
  top: 1rem;
  transition: .3s all ease-in-out;
}

.menu--hide {
  transform: translateX(70%) scale(0) 
}

.nav__button {
  position: fixed;
  right: 0;
  transform: translateX(100px);
  transition: .3s all ease-in-out;
}

.nav__button--show {
  
 transform: translateX(100px);
}
.menu {
  width: auto;
  display: flex;
  justify-content: space-around;
  list-style: none;
  transition: .3s all ease-in-out;
}

.menu-item__link {
  text-decoration: none;
  color: #fff;
  margin: 0 2rem;
  font-size: $font-medium;
  padding: 0rem 1rem;
  transition: 0.25s all ease-in-out;
}

.menu-item__link:hover {
  background: #fff;
  color: $details;
  padding: 0.5rem 1rem;
}
</style>