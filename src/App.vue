<template>
  <v-app :class="$style.vApp">
   
    <div :class="$style.card">
      <div class="card-body">
        <div class="container">
          <div class="row">
            <div class="col">
              <div :class="$style.colt">
                <v-title> 起點</v-title>
   
                <br />
                <v-text>租屋處</v-text>
              </div>
            </div>
            <div class="col">
              <div :class="$style.colt">
                <v-title> 目的地</v-title>

                <br />
                <v-text>實踐大學台北校區</v-text>
              </div>
            </div>
            <div class="col"></div>
          </div>
        </div>
        <div class="progress">
          <div
            role="progressbar"
            :class="$style.probar1"
            aria-valuenow="15"
            aria-valuemin="0"
            aria-valuemax="100"
          ></div>
          <div
            role="progressbar"
            :class="$style.probar2"
            aria-valuenow="30"
            aria-valuemin="0"
            aria-valuemax="100"
          ></div>
        </div>
        <div class="container">
          <div class="row">
            <div class="col">
              <div :class="$style.colt">
                <v-title> 出發時間</v-title>
                <br />
                <v-text>10:25</v-text>
              </div>
            </div>
            <div class="col">
              <div :class="$style.colt">
                <v-title>預約時間</v-title>
                <br />
                <v-text>10:50</v-text>
              </div>
            </div>
            <div class="col">
              <div :class="$style.colt">
                <v-text
                  style="color: #17e68e; font-weight: bold; font-size: 30px"
                  >25</v-text
                >

                <v-text>分鐘</v-text>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <br />
    <div :class="$style.btn">
      <button type="button" class="btn btn-success">詳細資訊</button>
    </div>
  </v-app>
</template>

<script>
import { reactive } from "vue";

export default {
  props: {
    msg: String,
  },
  setup() {
    const data = reactive({
      username: "joesong",
    });
    return { data };
  },
};
</script>


<style module>
.card {
  width: 100%;
  opacity: 0.95;
  border-radius: 20px;
  background-color: #40434b;
  margin-top: 539px;
}
.colt {
  width: 150%;
}
.colt v-title {
  font-size: 13px;
  color: #aaaaaa;
}
.colt v-text {
  color: #ffffff;
}
.probar1 {
  width: 50%;

  background-color: #f66b6f;
}
.probar2 {
  width: 50%;

  background-color: #e9a668;
}
.btn {
  text-align: center;
}
.btn button {
  background-color: #40434b;
  font-weight: bold;
  color: #2e2d2d;
  background: #17e68e;
  border-radius: 20px;
  width: 95%;
  height: 49px;
  text-align: center;
}
</style>
