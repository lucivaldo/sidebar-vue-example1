<template>
  <div class="navbar">
    <div class="app">
      <div class="app__logo">
        <img src="../../../assets/images/athenas.svg" alt="Logo">
      </div>

      <span class="app__name">Athenas</span>
    </div>

    <div class="notifications">
      <div class="notifications__email">
        <span class="icon"><i class="fas fa-envelope"></i></span>
      </div>

      <div class="notifications__alerts">
        <span class="icon"><i class="fas fa-bell"></i></span>
      </div>
    </div>

    <div class="user" ref="user">
      <div class="user__avatar">
        <img src="../../../assets/images/profile.jpg" alt="User Avatar">
      </div>

      <div class="user__description">
        <span class="user__name">Lucivaldo Castro</span>
        <span class="user__role">Desenvolvedor</span>
      </div>

      <div class="user__open-actions" @click="showUserActions = !showUserActions">
        <span class="icon"><i class="fas fa-ellipsis-v"></i></span>
      </div>

      <div class="user__actions" v-if="showUserActions">
        <a href="#" class="user__actions__item">
          <span class="icon"><i class="fas fa-user"></i></span>
          Perfil
        </a>

        <a href="#" class="user__actions__item">
          <span class="icon"><i class="fas fa-sign-out-alt"></i></span>
          Logout
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',

  mounted() {
    document.addEventListener('click', this.closeUser)
  },

  beforeDestroy() {
    document.removeEventListener('click', this.closeUser)
  },

  data() {
    return {
      showUserActions: false
    }
  },

  methods: {
    closeUser(event) {
      const user = this.$refs.user

      if (!user.contains(event.target)) {
        this.showUserActions = false
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.navbar {
  background-color: white;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.15), 
              0 2px 2px rgba(0, 0, 0, 0.15), 
              0 4px 4px rgba(0, 0, 0, 0.15), 
              0 8px 8px rgba(0, 0, 0, 0.15);
  transition: .3s;
  position: fixed;
  top: 0;
  left: calc(2 * 1rem + 2rem);
  right: 0;
  height: 4rem;
}

// Posicionamento em relação às medidas da sidebar
.nav--expand .navbar {
  left: 15rem;
}

.subnav--active .navbar {
  left: calc(2 * 1rem + 2rem + 20rem);
}

.nav--expand.subnav--active.subnav--shrink .navbar {
  left: calc(15rem);
}

.subnav--active.subnav--shrink .navbar {
  left: calc(2 * 1rem + 2rem);
}

.nav--expand.subnav--active .navbar {
  left: calc(15rem + 20rem);
}

.navbar {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: .5rem 2rem;
}

.app {
  display: flex;
  align-items: center;
  margin-right: auto;

  &__logo {
    margin-right: .75rem;
    width: 3rem;
    height: auto;
    overflow: hidden;
  }

  &__name {
    color: #444;
    font-weight: 700;
    font-size: 1.75rem;
    letter-spacing: 1px;
    text-transform: uppercase;
    transition: .3s;
    // font-family: 'Pathway Gothic One', sans-serif;
    // font-family: 'Carter One', cursive;
    font-family: 'Marcellus', serif;
    // font-family: 'Alata', sans-serif;

    &:hover {
      color: #111;
    }
  }
}

.notifications {
  display: flex;
  margin: 0 1.5rem;

  &__email, &__alerts {
    background-color: rgba(200, 200, 200, .15);
    border-radius: .5rem;
    color: #6a6a6a;
    width: 2rem;
    height: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: .4rem;
    cursor: pointer;

    &:hover {
      color: #333;
    }
  }
}

.user {
  display: flex;
  align-items: center;
  position: relative;

  &__avatar {
    border: 3px solid rgba(10, 10, 10, .75);
    border-radius: 50%;
    width: 3rem;
    height: 3rem;
    margin: 0 .5rem;
    overflow: hidden;

    &:hover {
      border-color: #222;
    }
  }

  &__avatar img {
    width: 3rem;
    height: auto;
  }

  &__description {
    display: flex;
    flex-direction: column;
    margin-right: 1rem;
  }

  &__name {
    color: #555;
    font-weight: bold;
    letter-spacing: 1px;

    &:hover {
      color: #333;
    }
  }

  &__role {
    color: #626262;
    font-weight: bold;
    font-size: .75rem;
    letter-spacing: 1px;

    &:hover {
      color: #444;
    }
  }

  &__open-actions .icon {
    color: #6a6a6a;
    padding: .5rem;

    &:hover {
      color: #333;
      cursor: pointer;
    }
  }
}

.user__actions {
  background-color: white;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.25), 
              0 2px 2px rgba(0, 0, 0, 0.20), 
              0 4px 4px rgba(0, 0, 0, 0.15), 
              0 8px 8px rgba(0, 0, 0, 0.10),
              0 16px 16px rgba(0, 0, 0, 0.05);
  position: absolute;
  top: 100%;
  right: 0;
  padding: .5rem;
  width: 17.5rem;
  border-radius: 5px;

  &__item {
    display: block;
    text-decoration: none;
    color: #333;
    padding: .75rem 1rem;
    border-radius: 5px;

    &:hover {
      background-color: rgba(0, 0, 0, 0.05);
      color: black;
    }
  }
}
</style>