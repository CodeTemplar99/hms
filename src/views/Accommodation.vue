<template>
  <div>
    <!-- BootstrapVue Done -->
    <base-header class="pb-6 pb-8 pt-5 pt-md-8 bg-gradient-success">
      <!-- Card stats -->
      <b-row>
        <b-col xl="3" md="6">
          <stats-card
            title="Total space"
            type="gradient-red"
            sub-title="350,897"
            icon="ni ni-active-40"
            class="mb-4"
          >
            <!-- <template slot="footer">
              <span class="text-success mr-2">3.48%</span>
              <span class="text-nowrap">Since last month</span>
            </template> -->
          </stats-card>
        </b-col>
        <b-col xl="3" md="6">
          <stats-card
            title="Available"
            type="gradient-orange"
            sub-title="2,356"
            icon="ni ni-chart-pie-35"
            class="mb-4"
          >
            <!-- <template slot="footer">
              <span class="text-success mr-2">12.18%</span>
              <span class="text-nowrap">Since last month</span>
            </template> -->
          </stats-card>
        </b-col>
        <b-col xl="3" md="6">
          <stats-card
            title="Allocated"
            type="gradient-green"
            sub-title="924"
            icon="ni ni-money-coins"
            class="mb-4"
          >
            <!-- <template slot="footer">
              <span class="text-danger mr-2">5.72%</span>
              <span class="text-nowrap">Since last month</span>
            </template> -->
          </stats-card>
        </b-col>
        <b-col xl="3" md="6">
          <stats-card
            title="Performance"
            type="gradient-info"
            sub-title="49,65%"
            icon="ni ni-chart-bar-32"
            class="mb-4"
          >
            <template slot="footer">
              <span class="text-success mr-2">54.8%</span>
              <span class="text-nowrap">Since last month</span>
            </template>
          </stats-card>
        </b-col>
      </b-row>
    </base-header>

    <b-container fluid class="mt--7">
      <b-row class="justify-content-center">
        <b-col lg="12">
          <card header-classes="bg-transparent">
            <h3 slot="header" class="mb-0">
              Rooms<br />

              <span class="text-muted font-weight-lighter"
                >click on a room to reserve a bedspace</span
              >
            </h3>
            <form>
              <div class="form-group col-sm-12 d-flex flex-column justify-content-center align-items-end">
                <label for="exampleFormControlSelect1">Select a hostel to reserve available space</label>
                <select class="form-control col-sm-4" id="exampleFormControlSelect1">
                  <option>Mary Slessor</option>
                  <option>1</option>
                  <option>2</option>
                  <option>3</option>
                  <option>4</option>
                </select>
              </div>
             
            </form>
            <b-row class="icon-examples">
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-active-40'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-air-baloon'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 102</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-album-2'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 103</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-align-center'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 104</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-align-left-2'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-ambulance'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-app'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-archive-2'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-atom'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-badge'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bag-17'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-basket'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bell-55'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bold-down'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bold-left'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bold-right'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bold-up'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bold'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-book-bookmark'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-books'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-box-2'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-briefcase-24'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-building'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bulb-61'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bullet-list-67'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-bus-front-12'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-button-pause'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-button-play'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-button-power'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-calendar-grid-58'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-camera-compact'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-caps-small'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-cart'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-chart-bar-32'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-chart-pie-35'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-chat-round'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-check-bold'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-circle-08'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-cloud-download-95'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-cloud-upload-96'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-compass-04'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-controller'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-credit-card'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-curved-next'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-delivery-fast'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-diamond'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-email-83'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-fat-add'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-fat-delete'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-fat-remove'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-favourite-28'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-folder-17'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-glasses-2'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-hat-3'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-headphones'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-html5'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-istanbul'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-circle-08'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="2" md="6">
                <button
                  type="button"
                  class="btn-icon-clipboard"
                  v-clipboard:copy="'ni ni-key-25'"
                  v-clipboard:success="onCopy"
                  title=""
                  data-original-title=" You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment"
                >
                  <div>
                    <span>Room 101</span>
                  </div>
                </button>
              </b-col>
            </b-row>
          </card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
import Vue from "vue";
import VueClipboard from "vue-clipboard2";
import BaseHeader from "@/components/BaseHeader";

Vue.use(VueClipboard);
export default {
  name: "icons",
  components: {
    BaseHeader,
  },
  methods: {
    onCopy() {
      this.$notify({
        type: "info",
        message:
          " You have successfully reserved a bedspace in this room, check your activity for more details. Note: This is not your bedspace yet, it has been reserved pending payment and will be forfeited after a 24 hours of non payment",
      });
    },
  },
};
</script>
<style></style>
