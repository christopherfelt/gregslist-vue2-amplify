<template>
  <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/">About</router-link>
    </nav> -->
  <div>
    <div class="w-100">
      <b-navbar toggleable="lg" type="dark" variant="info" class="p-1 px-4">
        <b-navbar-brand href="#">Gregslist</b-navbar-brand>

        <!-- <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item><rouer-link>Cars</rouer-link></b-nav-item>
            <b-nav-item><rouer-link>Cars</rouer-link></b-nav-item>
            <b-nav-item><rouer-link>Cars</rouer-link></b-nav-item>
          </b-navbar-nav>
        </b-collapse> -->

        <!-- <div class="w-25 d-flex justify-content-between">
          <rouer-link>Cars</rouer-link>
          <rouer-link>Houses</rouer-link>
          <rouer-link>Jobs</rouer-link>
        </div> -->
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <!-- <em>User</em> -->
              <b-icon icon="person-fill"></b-icon>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
        <!-- </b-collapse> -->
      </b-navbar>
    </div>
    <router-view />
  </div>
</template>

<style>
</style>
