/* eslint-disable vue/valid-v-for */
<template>
    <div class="main-content" id="panel">
         <nav class="navbar navbar-top navbar-expand navbar-dark bg-primary border-bottom">
            <div class="container-fluid">
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <!-- Search form -->
                    <form class="navbar-search navbar-search-light form-inline mr-sm-3" id="navbar-search-main">
                        <div class="form-group mb-0">
                            <div class="input-group input-group-alternative input-group-merge">
                                <div class="input-group-prepend">
                                    <span class="input-group-text"><i class="fas fa-search"></i></span>
                                </div>
                                <input class="form-control" placeholder="Search" v-model="search" type="text">
                            </div>
                        </div>
                        <button type="button" class="close" data-action="search-close" data-target="#navbar-search-main" aria-label="Close">
              <span aria-hidden="true">×</span>
            </button>
                    </form>
                    <!-- Navbar links -->
                    <ul class="navbar-nav align-items-center  ml-md-auto ">
                        <li class="nav-item d-xl-none">
                            <!-- Sidenav toggler -->
                            <div class="pr-3 sidenav-toggler sidenav-toggler-dark" data-action="sidenav-pin" data-target="#sidenav-main">
                                <div class="sidenav-toggler-inner">
                                    <i class="sidenav-toggler-line"></i>
                                    <i class="sidenav-toggler-line"></i>
                                    <i class="sidenav-toggler-line"></i>
                                </div>
                            </div>
                        </li>
                        <li class="nav-item d-sm-none">
                            <a class="nav-link" href="#" data-action="search-show" data-target="#navbar-search-main">
                                <i class="ni ni-zoom-split-in"></i>
                            </a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link" href="#" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                <i class="fas fa-bell"></i>
                            </a>
                            <div class="dropdown-menu dropdown-menu-xl  dropdown-menu-right  py-0 overflow-hidden">
                                <!-- Dropdown header -->
                                <div class="px-3 py-3">
                                    <h6 class="text-sm text-muted m-0">You have <strong class="text-primary">13</strong> notifications.</h6>
                                </div>
                                <!-- List group -->
                                <div class="list-group list-group-flush">
                                    <a href="#!" class="list-group-item list-group-item-action">
                                        <div class="row align-items-center">
                                            <div class="col-auto">
                                                <!-- Avatar -->
                                                <img alt="Image placeholder" src="../assets/img/theme/team-1.jpg" class="avatar rounded-circle">
                                            </div>
                                            <div class="col ml--2">
                                                <div class="d-flex justify-content-between align-items-center">
                                                    <div>
                                                        <h4 class="mb-0 text-sm">John Snow</h4>
                                                    </div>
                                                    <div class="text-right text-muted">
                                                        <small>2 hrs ago</small>
                                                    </div>
                                                </div>
                                                <p class="text-sm mb-0">Let's meet at Starbucks at 11:30. Wdyt?</p>
                                            </div>
                                        </div>
                                    </a>
                                    <a href="#!" class="list-group-item list-group-item-action">
                                        <div class="row align-items-center">
                                            <div class="col-auto">
                                                <!-- Avatar -->
                                                <img alt="Image placeholder" src="../assets/img/theme/team-2.jpg" class="avatar rounded-circle">
                                            </div>
                                            <div class="col ml--2">
                                                <div class="d-flex justify-content-between align-items-center">
                                                    <div>
                                                        <h4 class="mb-0 text-sm">John Snow</h4>
                                                    </div>
                                                    <div class="text-right text-muted">
                                                        <small>3 hrs ago</small>
                                                    </div>
                                                </div>
                                                <p class="text-sm mb-0">A new issue has been reported for Argon.</p>
                                            </div>
                                        </div>
                                    </a>
                                    <a href="#!" class="list-group-item list-group-item-action">
                                        <div class="row align-items-center">
                                            <div class="col-auto">
                                                <!-- Avatar -->
                                                <img alt="Image placeholder" src="../assets/img/theme/team-3.jpg" class="avatar rounded-circle">
                                            </div>
                                            <div class="col ml--2">
                                                <div class="d-flex justify-content-between align-items-center">
                                                    <div>
                                                        <h4 class="mb-0 text-sm">John Snow</h4>
                                                    </div>
                                                    <div class="text-right text-muted">
                                                        <small>5 hrs ago</small>
                                                    </div>
                                                </div>
                                                <p class="text-sm mb-0">Your posts have been liked a lot.</p>
                                            </div>
                                        </div>
                                    </a>
                                    <a href="#!" class="list-group-item list-group-item-action">
                                        <div class="row align-items-center">
                                            <div class="col-auto">
                                                <!-- Avatar -->
                                                <img alt="Image placeholder" src="../assets/img/theme/team-4.jpg" class="avatar rounded-circle">
                                            </div>
                                            <div class="col ml--2">
                                                <div class="d-flex justify-content-between align-items-center">
                                                    <div>
                                                        <h4 class="mb-0 text-sm">John Snow</h4>
                                                    </div>
                                                    <div class="text-right text-muted">
                                                        <small>2 hrs ago</small>
                                                    </div>
                                                </div>
                                                <p class="text-sm mb-0">Let's meet at Starbucks at 11:30. Wdyt?</p>
                                            </div>
                                        </div>
                                    </a>
                                    <a href="#!" class="list-group-item list-group-item-action">
                                        <div class="row align-items-center">
                                            <div class="col-auto">
                                                <!-- Avatar -->
                                                <img alt="Image placeholder" src="../assets/img/theme/team-5.jpg" class="avatar rounded-circle">
                                            </div>
                                            <div class="col ml--2">
                                                <div class="d-flex justify-content-between align-items-center">
                                                    <div>
                                                        <h4 class="mb-0 text-sm">John Snow</h4>
                                                    </div>
                                                    <div class="text-right text-muted">
                                                        <small>3 hrs ago</small>
                                                    </div>
                                                </div>
                                                <p class="text-sm mb-0">A new issue has been reported for Argon.</p>
                                            </div>
                                        </div>
                                    </a>
                                </div>
                                <!-- View all -->
                                <a href="#!" class="dropdown-item text-center text-primary font-weight-bold py-3">View all</a>
                            </div>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link" href="#" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                          <i class="fas fa-comment"></i>
                            </a>
                            <div class="dropdown-menu dropdown-menu-lg dropdown-menu-dark bg-default  dropdown-menu-right ">
                                <div class="row shortcuts px-4">
                                    <a href="#!" class="col-4 shortcut-item">
                                        <span class="shortcut-media avatar rounded-circle bg-gradient-red">
                      <i class="ni ni-calendar-grid-58"></i>
                    </span>
                                        <small>Calendar</small>
                                    </a>
                                    <a href="#!" class="col-4 shortcut-item">
                                        <span class="shortcut-media avatar rounded-circle bg-gradient-orange">
                      <i class="ni ni-email-83"></i>
                    </span>
                                        <small>Email</small>
                                    </a>
                                    <a href="#!" class="col-4 shortcut-item">
                                        <span class="shortcut-media avatar rounded-circle bg-gradient-info">
                      <i class="ni ni-credit-card"></i>
                    </span>
                                        <small>Payments</small>
                                    </a>
                                </div>
                            </div>
                        </li>
                    </ul>
                    <ul class="navbar-nav align-items-center  ml-auto ml-md-0 ">
                        <li class="nav-item dropdown">
                            <a class="nav-link pr-0" href="#" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                <div class="media align-items-center">
                                    <span class="avatar avatar-sm rounded-circle">
                    <img alt="Image placeholder" src="../assets/img/theme/team-4.jpg">
                  </span>
                                    <div class="media-body  ml-2  d-none d-lg-block">
                                        <span class="mb-0 text-sm  font-weight-bold">John Snow</span>
                                    </div>
                                </div>
                            </a>
                            <div class="dropdown-menu  dropdown-menu-right ">
                                <div class="dropdown-header noti-title">
                                    <h6 class="text-overflow m-0">Welcome!</h6>
                                </div>
                                <a href="#!" class="dropdown-item">
                                    <i class="ni ni-single-02"></i>
                                    <span>My profile</span>
                                </a>
                                <a href="#!" class="dropdown-item">
                                    <i class="ni ni-settings-gear-65"></i>
                                    <span>Settings</span>
                                </a>
                                <div class="dropdown-divider"></div>
                                <a href="#!" class="dropdown-item">
                                    <i class="ni ni-user-run"></i>
                                    <span>Logout</span>
                                </a>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
        <!-- Topnav -->
        <Header></Header>
         <div class="row align-items-center py-4">
                        <div class="col-lg-6 col-7">
                            <nav aria-label="breadcrumb" class="d-none d-md-inline-block ml-md-4">
                                <ol class="breadcrumb breadcrumb-links breadcrumb-dark">
                                    <li class="breadcrumb-item"><router-link to="/dashboard"><i class="fas fa-home"></i></router-link></li>
                                    <li class="breadcrumb-item"><router-link to="/product">Quản lý cửa hàng</router-link></li>
                                </ol>
                            </nav>
                        </div>
                    </div>
      <div class="product">
      <div class="header_pro">
      <p></p>
        <p></p>
        <a href="#open-modal"
              >Thêm cửa hàng</a
            >
      </div>
      <div class="main__product">
        <div class="container">
          <ul class="responsive-table">
            <li class="table-header">
              <div class="col col-1"> Tên cửa hàng</div>
              <div class="col col-2">Hình ảnh</div>
              <div class="col col-3">Địa chỉ</div>
              <div class="col col-4">Chỉnh sửa</div>
              <div class="col col-5">Xóa</div>
            </li>
            <li class="table-row">
              <div class="col col-1" data-label="Job Id">42235</div>
              <div class="col col-2" data-label="Customer Name">John Doe</div>
              <div class="col col-3" data-label="Amount">$350</div>
              <div class="col col-4" data-label="Payment Status">
                <a href="#open-modal">
                  <button @click.prevent="editProduct(product)">
                    <i class="fas fa-edit"> </i>
                  </button>
              </a>
            </div>
              <div class="col col-5" data-label="Payment Status">
                <a @click.prevent="deleteProduct(product.id)">
                  <i class="fas fa-trash-alt"></i>
              </a>
              </div>
            </li>
             <li class="table-row">
              <div class="col col-1" data-label="Job Id">42235</div>
              <div class="col col-2" data-label="Customer Name">John Doe</div>
              <div class="col col-3" data-label="Amount">$350</div>
              <div class="col col-4" data-label="Payment Status">
                <a href="#open-modal">
                  <button @click.prevent="editProduct(product)">
                    <i class="fas fa-edit"> </i>
                  </button>
              </a>
            </div>
              <div class="col col-5" data-label="Payment Status">
                <a @click.prevent="deleteProduct(product.id)">
                  <i class="fas fa-trash-alt"></i>
              </a>
              </div>
            </li>
            
          </ul>
        </div>
      </div>           
    <div id="navigation">
      <ul class="pagination">
        <li class="page-item">
          <button
            type="button"
            class="page-link"
            v-if="page != 1"
            @click="page--"><i class="fas fa-arrow-circle-left"></i>
          </button>
        </li>
        <li class="page-item">
          <button type="button" class="page-link" v-for="pageNumber in pages.slice(page - 1, page + 5)" v-bind:key="pageNumber" @click="page = pageNumber">
            {{ pageNumber }}
          </button>
        </li>
        <li class="page-item">
          <button
            type="button"
            @click="page++"
            v-if="page < pages.length"
            class="page-link"
          >
            <i class="fas fa-arrow-circle-right"></i>
          </button>
        </li>
      </ul>
    </div>
    <div id="open-modal" class="modal-window-product">
      <div class="form">
        <a href="#" title="Close" class="modal-close">Close</a>
        <center>
          <h2>{{ contentForm }}</h2>
        </center>
        <form  @submit.prevent="addProduct">
          <div id="formAdd">
            <div class="item_input">
              <label for="input" class="Input-label">Tên Shop </label>
              <input
                type="text"
                id="input"
                class="Input-text"
                placeholder="Tên Shop"
                v-model="newshop.name"
              />
            </div>
            <div class="item_input">
              <label >Hình ảnh</label><br />
              <input type="text" placeholder="Link ảnh" name="image" id="img" v-model="newshop.img" />
            </div> 
            <div class="item_input">
              <label >Địa chỉ</label><br />
              <input type="text" placeholder="Link ảnh" name="address" id="address" v-model="newshop.address" />
            </div>
          </div>
          <div class="add_resest">
            <button type="submit">{{ buttonAdd }}</button>
            <button type="submit" @click.prevent="clearData"  >Xóa dữ liệu </button>
          </div>
        </form>
      </div>
    </div>
    <router-view></router-view>
  </div>
    </div>
</template>
<script>
import Header from './Header.vue'
export default {
    components:{
         Header
    },
};
</script>
 <script>
export default {
  data() {
    return {
      shops: [],
      newshop: {
           img : null,
          imageUrl: null
      },
      pageSize: 5,
      currentPage: 1,
      page: 1,
      perPage: 4,
      pages: [],
      search: null,
      edit: false,
      buttonAdd: "Thêm",
      contentForm: "Thêm cửa hàng mới",
    };
  },
  created() {
    this.getData();
  },
  methods: {
    onChange(e) {
      const file = e.target.files[0]
      this.img= file
      this.newshop.img = URL.createObjectURL(file)

      console.log(file);
      alert(this.newshop.img);
    },
    getData() {
          fetch('https://damp-woodland-88343.herokuapp.com/api/products')
        .then((response) => response.json())
        .then((data) => (this.shops = data));
    },
    deleteProduct(id) {
      axios.delete('https://damp-woodland-88343.herokuapp.com/api/products/'+id);
      this.getData();
    },

    addProduct() {
      if (this.edit == false) {
        axios.post('https://damp-woodland-88343.herokuapp.com/api/products', this.newshop);
        alert(" Insert product success");
        this.getData();
      } else {
        axios.put('https://damp-woodland-88343.herokuapp.com/api/products/'+this.newshop.id,this.newshop);
        alert(" Update product success");
        this.getData();
        this.edit ==false;
      }
    },
    editProduct(shop) {
      this.edit = true;
      this.buttonAdd = "Cập nhật";
      this.contentForm = "Cập Nhật Thông Tin Shop";
      this.newshop.id = shop.id;
      this.newshop.name = shop.name;
      this.newshop.img = shop.img;
      this.newshop.desciption = shop.desciption;
      this.newshop.type = shop.type;
    },
    setPages() {
      let numberOfPages = Math.ceil(this.shops.length / this.perPage);
      for (let index = 1; index <= numberOfPages; index++) {
        this.pages.push(index);
      }
    },
    clearData() {
      this.newproduct.name = "";
      this.newproduct.img = "";
      this.newproduct.desciption = "";
      this.newproduct.type = "";
      this.newproduct.quantity = "";
      this.newproduct.price = "";
      this.newproduct.discount = "";
      this.newproduct.heart = 0;
    },
    paginate(shops) {
      let page = this.page;
      let perPage = this.perPage;
      let from = page * perPage - perPage;
      let to = page * perPage;
      return shops.slice(from, to);
    },
  },
  computed: {
    showProducts() {
      if (this.search) {
        return this.shops.filter((item) => {
          return this.search
            .toLowerCase()
            .split(" ")
            .every((v) => item.name.toLowerCase().includes(v));
        });
      } else {
        return this.paginate(this.shops);
      }
    },
  },
  watch: {
    products() {
      this.setPages();
    },
  },
  filters: {
    trimWords(value) {
      return value.split(" ").splice(0, 20).join(" ") + "...";
    },
  },
};
</script>
<style lang="scss">
.product{
    width: 100%;
}

// Table

body {
  font-family: 'lato', sans-serif;
}
.container {
  max-width: 80%;
  margin-left: auto;
  margin-right: auto;
  padding-left: 10px;
  padding-right: 10px;
}

h2 {
  font-size: 26px;
  margin: 20px 0;
  text-align: center;
  small {
    font-size: 0.5em;
  }
}

.responsive-table {
  li {
    border-radius: 3px;
    padding: 25px 30px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 25px;
  }
  .table-header {
    background-color: #95A5A6;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 0.03em;
  }
  .table-row {
    background-color: #ffffff;
    box-shadow: 0px 0px 9px 0px rgba(0,0,0,0.1);
  }
  .col-1 {
    flex-basis: 20%;
  }
  .col-2 {
    flex-basis: 30%;
  }
  .col-3 {
    flex-basis: 30%;
  }
  .col-4 {
    flex-basis: 10%;
  }
   .col-5 {
    flex-basis: 10%;
  }
  
  @media all and (max-width: 767px) {
    .table-header {
      display: none;
    }
    .table-row{
      
    }
    li {
      display: block;
    }
    .col {
      
      flex-basis: 100%;
      
    }
    .col {
      display: flex;
      padding: 10px 0;
      &:before {
        color: #6C7A89;
        padding-right: 10px;
        content: attr(data-label);
        flex-basis: 50%;
        text-align: right;
      }
    }
  }
}
/// table
.main__product {
    width: 100%;
        .col-4 {
          margin-bottom: 1px;
          a {
            background-color: crimson;
            /* Màu của Quản trị mạng ^^ */
            border: none;
            color: white;
            padding: 13px 14px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: auto 2% 0 0;
            -webkit-transition-duration: 0.4s;
            /* Safari */
            transition-duration: 0.4s;
            cursor: pointer;
            border-radius: 15px;
          }

          a:hover {
            background-color: seagreen;
          }
       }
       .col-5{
        a {
            background-color: crimson;
            /* Màu của Quản trị mạng ^^ */
            border: none;
            color: white;
            padding: 13px 15px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: auto 2% 0 0;
            -webkit-transition-duration: 0.4s;
            /* Safari */
            transition-duration: 0.4s;
            cursor: pointer;
            border-radius: 15px;
          }

          a:hover {
            background-color: seagreen;
            color: white;
          }
       }
}

  .header_pro {
    width:80%;
    display: grid;
    grid-template-columns: 2fr 1.5fr 1fr;
    margin-bottom: 3%;

    a {
      background-color: crimson;
      /* Màu của Quản trị mạng ^^ */
      border: none;
      color: white;
      padding: 13px 18px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
      font-size: 16px;
      -webkit-transition-duration: 0.4s;
      /* Safari */
      transition-duration: 0.4s;
      cursor: pointer;
      outline: none;
      border-radius: 25px;
    }

    button:hover {
      background-color: seagreen;
    }

    input {
      padding-left: 1%;
      outline: none;
      border-radius: 20px;
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    }
  }
.pro_header {
  display: flex;
}
.pro_header button {
  float: right;
}
.form h2 {
  margin-bottom: 4%;
}

div#formAdd {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-row-gap: 30px;
}

.add_resest{
  display: flex;
  justify-content: center ;
  >button{
    margin-left: 1%;
  }
}
form button {
  margin-top: 5%;
  background-color: crimson; /* Màu của Quản trị mạng ^^ */
  border: none;
  color: white;
  padding: 13px 18px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
  cursor: pointer;
  border-radius: 4px;
}
.item_input label {
  top: 2%;
  bottom: 2%;
}
.item_input input {
  border-radius: 0.4rem;
  height: 75%;
  width: 85%;
  padding: 10px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 10px 10px 0 rgba(0, 0, 0, 0.19);
}
.item_input textarea {
  border-radius: 0.4rem;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 10px 10px 0 rgba(0, 0, 0, 0.19);
}
.modal-window-product {
  position: fixed;
  background-color: rgba(255, 255, 255, 0.25);
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 999;
  visibility: hidden;
  opacity: 0;
  pointer-events: none;
  transition: all 0.3s;
  &:target {
    visibility: visible;
    opacity: 1;
    pointer-events: auto;
  }
  & > div {
    width: 60%;
    position: absolute;
    top: 50%;
    left: 50%;
    height: 80%;
    overflow: auto;
    border-radius: 0.4rem;
    transform: translate(-50%, -50%);
    padding: 2em;
    background-image: linear-gradient(to right, #f2709c, #ff9472);
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2),
      0 20px 20px 0 rgba(0, 0, 0, 0.19);
  }
  header {
    font-weight: bold;
  }
  h1 {
    font-size: 150%;
    margin: 0 0 15px;
  }
}
.modal-close {
  color: #aaa;
  line-height: 50px;
  font-size: 80%;
  position: absolute;
  right: 0;
  text-align: center;
  top: 0;
  width: 70px;
  text-decoration: none;
  &:hover {
    color: black;
  }
}

///// PAGINATION
ul li {
  list-style: none;
}
.page-item {
  padding: 10px;
}
.pagination {
  display: flex;
  padding: 20px;
}

#navigation {
  margin-left: 30%;
  display: flex;
}
.pagination {
  margin-top: 5%;
  width: 50%;
  transform: translate(-50%, -50%);
  margin-left: 50px;
  padding: 10px;
  li {
    display: flex;
    list-style: none;
  }
  button {
    display: block;
    width: 100px;
    height: 40px;
    line-height: 40px;
    background-color: #fff;
    text-align: center;
    text-decoration: none;
    color: #252525;
    border-radius: 4px;
    font-size: 17px;
    margin: 5px;
    box-shadow: inset 0 5px 10px rgba(0, 0, 0, 0.1),
      0 2px 5px rgba(0, 0, 0, 0.5);
    transition: all 0.3s ease;
    &:hover,
    &.active {
      color: white;
      background-color: yellow;
    }
  }
  &:first-child button {
    border-radius: 30px;
  }

  &:last-child button {
    border-radius: 30px;
  }
}
</style>
