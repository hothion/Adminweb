<template>
    <div class="main-content" id="panel">
        <!-- Topnav -->
        <Header></Header>
             <div class="row align-items-center py-4">
                        <div class="col-lg-6 col-7">
                            <nav aria-label="breadcrumb" class="d-none d-md-inline-block ml-md-4">
                                <ol class="breadcrumb breadcrumb-links breadcrumb-dark">
                                    <li class="breadcrumb-item"><router-link to="/dashboard"><i class="fas fa-home"></i></router-link></li>
                                    <li class="breadcrumb-item"><router-link to="/order">Quản lý người dùng</router-link></li>
                                </ol>
                            </nav>
                        </div>
                    </div>
            <div class="content table">
                <div class="content table_title">
                    <p> Tên người dùng</p>
                    <p> Tên đăng nhập</p>
                    <p>Địa chỉ</p>
                    <p>Email</p>
                    <p>Điện thoại</p>
                    <p>Ngày sinh</p>
                    <p>Xóa</p>
                </div>
                <div class="content table_content" v-for="user in users" :key="user.id">
                    <p>{{ user.firstName }} {{ user.lastName }}</p>
                    <p>{{ user.account }}</p>
                    <p>{{ user.address }}</p>
                    <p>{{user.email}}</p>
                    <p>{{user.phone}}</p>
                    <p>{{user.birthday}}</p>
                    <p>
                        <button @click.prevent="deleteUser(user.id)"><i class="fas fa-minus-circle"></i></button>
                    </p>
                </div>
            </div>
           <router-view></router-view>
    </div>
</template>
<script>
import Vue from 'vue';
import VueAxios from 'vue-axios';
import axios from 'axios';
Vue.use(VueAxios, axios);
import Header from './Header.vue'
export default {
   components:{
         Header
    },
    data() {
        return {
            users: [],
        };
    },
    created() {
        this.getData();
    },
    methods: {
        deleteUser(id) {
            axios.delete(
                'https://damp-woodland-88343.herokuapp.com/api/account/'+id
            );
            alert("Delete order succes");
            this.getData();
        },
        getData() {
                fetch('https://damp-woodland-88343.herokuapp.com/api/account')
                    .then((response) => response.json())
                    .then((data) => (this.users = data));          
        },
    },
};
</script>
<style lang="scss">
#img_order_detail{
    width: 150px;
    height: 150px;
}
#product_detail{
    display: flex;

}
.content .table_content,
.content .table_title {
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr ;
    grid-column-gap: 10px;
    grid-row-gap: 20px;
    border-radius: 10px;
}

.content .table {
    width: 100%;
}

.content {
    width: 95%;
    margin-left: 2%;
    h1 {
        margin-bottom: 10px;
        color: black;
        font-size: 2rem;
        font-size: 1.5rem;
        font-family: Helvetica, Arial, sans-serif;
    }
    .list {
        display: flex;
        margin-bottom: 10px;
        button {
        padding: 10px;
        background: none;
        border-bottom: 2px solid red;
        border-right: 2px solid red;
        border-radius: 10px;
        font-size: 1rem;
    }
    }
    .table_title {
        margin-left: 0;
        text-align: center;
        background: #009688;
        color: white;
        font-size: 1.2rem;
        padding: 10px 0;
        box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.35);
    }
    .table_content {
        margin-top: 10px;
        font-size: 1.1rem;
        background: white;
        margin-left: 0;
        text-align: center;
        box-shadow: 0px 7px 29px 0px rgba(100, 100, 111, 0.2);
        p {
            padding: 17px 15px;
        }
        a {
            padding: 8px;
            background: red;
            color: white;
            border: 0;
            border-radius: 10px;
        }
        button {
            padding: 8px;
            background: rgba(244,63,94);;
            color: white;
            border: 0;
            border-radius: 10px;
        }
    }
}

.modal-window-order {
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
    width: 40%;
    position: absolute;
    top: 50%;
    left: 50%;
    height: 70%;
    overflow: auto;
    border-radius: 0.4rem;
    transform: translate(-50%, -50%);
    padding: 2em;
    background-image: linear-gradient(to right, #f2e6eb, #e6d3e8);
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

</style>
