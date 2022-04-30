<template>
  <va-navbar color="primary" shape>
    <template #left>
      <va-navbar-item style="width: 200px">
        <router-link to="/"><img class="absolute left-0" style="top: 10%; transform: scale(0.7)" src="@/assets/Logos/manageit-digital-logo-clear-no-koru.png" alt="manageit logo"></router-link>
      </va-navbar-item>


      <va-navbar-item @mouseover="upHere = true" @mouseleave="upHere = false">
        <div>
          <router-link to="/">Services <va-icon class="material-icons" :size="14">expand_more</va-icon></router-link>
        </div>
        <div class="w-100 absolute h2" v-show="upHere"></div>
        <va-card class="mw-900 mt-4" style="position: absolute" v-show="upHere" stripe stripe-color="success">
          <va-card-title>Proactive Monitoring, Managment And Support</va-card-title>
          <va-card-content class="row" style="text-align: left">
            <service title="ServiceIT" description="Proactive monitoring and management." />
            <service title="ConnectIT" description="Regular maintenance of your network devices." />
            <service title="SupportIT" description="Engeneer on call support." />
            <service title="SecureIT" description="Secure your vulnerable data against outside attacks." />
            <service title="BackIT" description="Prevention of data loss and downtime with backups." />
            <service title="RecoverIT" description="disaster recovery strategies and actions." />
          </va-card-content>
        </va-card>
      </va-navbar-item>
      <va-navbar-item>
        <router-link to="/about">About Us</router-link>
      </va-navbar-item>
      <va-navbar-item>
        <router-link to="/about">Contact</router-link>
      </va-navbar-item>
    </template>

    <template #center>
    </template>

    <template #right>
      <va-navbar-item>0800 648 7870 <va-icon class="material-icons" :size="14">phone</va-icon></va-navbar-item>
      <va-navbar-item>Unit 3, 92B Russley Roadf <va-icon class="material-icons" :size="14">home</va-icon></va-navbar-item>
      <va-navbar-item>Portal <va-icon class="material-icons" :size="14">account_circle</va-icon></va-navbar-item>
    </template>
  </va-navbar>
</template>


<script>
import Service from "@/components/navagation/Service";
export default {
  name: "MainBar.vue",
  components: {Service},
  data() {
    return {
      upHere: false
    }
  }
}
</script>

<style scoped>

</style>