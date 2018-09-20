<template>
  <div class="animated fadeIn">
    <b-row>
      <b-col xs="12" lg="6">
        <b-card>
          <div slot="header">
            Tabs with icons
          </div>
          <b-tabs v-model="tabIndex[0]">
            <b-tab active>
              <template slot="title">
                 <i class="icon-pie-chart"></i> {{tabs[0]}}
              </template>
              <br>
              
              </b-tab>
            <b-tab>
              <template slot="title">
                <i class="icon-pie-chart"></i> {{tabs[1]}}
              </template>
              <br>2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore
              et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
              aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
              dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt mollit anim id est laborum.
            </b-tab>
            <b-tab>
              <template slot="title">
                <i class="icon-pie-chart"></i> {{tabs[2]}}
              </template>
              <br>3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore
              et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
              aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
              dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt mollit anim id est laborum.
            </b-tab>
          </b-tabs>
        </b-card>
      </b-col>
      
    </b-row>
  </div>
</template>

<script>
import * as d3 from 'd3';

export default {
  name: 'tabs',
  data () {
    return {
      tabIndex: [0, 0],
      tabs: [
        'Trainings By Month',
        'Trainings Completed Monthly',
        'Trainings Completed by Accounts'
      ]
    }
  }
}
</script>

<style scoped>
.col-lg-6 {
    flex: none;
    max-width: none;
}
</style>

<style lang="sass" scoped>
svg
  margin: 25px;
path
  fill: none
  stroke: #76BF8A
  stroke-width: 3px
</style>
