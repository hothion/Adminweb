<template lang="">
    <div class="main-content" id="panel">
    <Header></Header>
        <div class="row align-items-center py-4">
                        <div class="col-lg-6 col-7">
                            <nav aria-label="breadcrumb" class="d-none d-md-inline-block ml-md-4">
                                <ol class="breadcrumb breadcrumb-links breadcrumb-dark">
                                    <li class="breadcrumb-item"><a href="#"><i class="fas fa-home"></i></a></li>
                                    <li class="breadcrumb-item"><a href="#">Thống kê</a></li>
                                </ol>
                            </nav>
                        </div>
                        <div class="col-lg-6 col-5 text-right">
                            <a href="#" class="btn btn-sm btn-neutral">New</a>
                            <a href="#" class="btn btn-sm btn-neutral">Filters</a>
                        </div>
                    </div>
    <div class="statistic">
    <div class="col1">
      <div class="LineChart">
        <h3>Người đăng ký và lượng sản phẩm qua các tháng</h3>
        <productChart />
      </div>
      <div class="BarChart">
        <h3>Đơn đặt hàng qua các tháng</h3>
        <orderBar />
      </div>
    </div>
 <router-view></router-view>
  </div>
    </div>
</template>

<script>
// import Chart from 'chart.js';
import Header from './Header.vue';
import productChart from "./ProductChart.vue";
import orderBar from "./OrderBar.vue";

export default {
  name: "order",
  data() {
    return {
      selected: "",
      counter: 0,
      numberWeek: {},
      getWeek: [],
      number: 0,
      listDay: [],
      yeus:[],
      currentYear: new Date().getFullYear(),
    };
  },
  components: {
    productChart,
    orderBar,
    Header
  },
};
</script>
<style lang="scss">
.statistic {
  width: 100%;
}
.col1 {
  width: 100%;
  display: flex;
  margin-left: 5%;
  margin-top: 4%;
  .LineChart {
    width: 80%;
  }
  .BarChart {
    width: 80%;
    margin-left: 3%;
  }
}
.col2 {
  width: 100%;
  display: flex;
  .PieChart {
    width: 80%;
  }
  .BarChart {
    width: 80%;
    margin-left: 3%;
    span {
      display: flex;
      padding: 20px;
      h3 {
        margin: 0px 10px 0px 10px;
      }
    }
  }
}
.statistic h1 {
  box-shadow: 0 0px 8px 0 rgba(0, 0, 0, 0.2), 0 0px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>
