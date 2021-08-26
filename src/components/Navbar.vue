<template>
  <div>
    <header class="header border-bottom border-warning border-5">
      <div class="container">
        <nav class="navbar navbar-expand-lg navbar-light">
          <div class="container-fluid">
            <a class="navbar-brand" href="#">
              <img src="@/assets/images/logo.jpeg" alt="logo" style="width:111px; height:40px;" />
            </a>
            <button
              class="navbar-toggler border-0"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#navbarNav"
              aria-controls="navbarNav"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav me-auto">
                <li class="nav-item">
                  <a class="nav-link text-dark" aria-current="page" href="#">關於</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-dark" href="#">挖寶</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-dark" href="#">我有個大膽的想法</a>
                </li>
              </ul>
              <div class="justify-content-end d-flex">
                <button
                  class="btn btn-warning text-dark rounded-pill me-3"
                  @click="showLogInModal"
                >登入</button>
                <button
                  class="btn btn-outline-secondary text-secondary rounded-pill"
                  @click="showSignInModal"
                >註冊</button>
              </div>
            </div>
          </div>
        </nav>
      </div>
    </header>
    <!-- LogIn Modal -->
    <div class="modal" tabindex="-1" ref="login">
      <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title">登入</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <label for="login_account" class="form-label mb-1">帳號</label>
            <input
              type="text"
              id="login_account"
              class="form-control border-light bg-light mb-3"
              placeholder="acount"
            />
            <label for="login_passward" class="form-label mb-1">密碼</label>
            <input
              type="text"
              id="login_passward"
              class="form-control border-light bg-light mb-3"
              placeholder="password"
            />
            <span class="text-secondary">忘記密碼？</span>
          </div>
          <div class="p-3 border-0">
            <button
              type="button"
              class="btn btn-lg btn-warning text-dark w-100 rounded-pill"
              data-bs-dismiss="modal"
            >登入</button>
            <div class="position-relative">
              <div class="progress w-100 mb-4 mt-5" style="background-color:#E8E8DB; height:2px;">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="0"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
              <span
                class="position-absolute top-0 start-50 translate-middle text-secondary bg-white fs-sm px-0 px-md-2"
              >
                還沒有帳號？
                <a
                  href="#"
                  class="text-danger text-decoration-none"
                  @click="showSignInModal"
                >註冊一個帳號</a>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- SignIn Modal -->
    <div class="modal" tabindex="-1" ref="signin">
      <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title">註冊</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <label for="signin_account" class="form-label mb-1">帳號</label>
            <input
              type="text"
              id="signin_account"
              class="form-control border-light bg-light mb-3"
              placeholder="acount"
            />
            <label for="signin_passward" class="form-label mb-1">密碼</label>
            <input
              type="text"
              id="signin_passward"
              class="form-control border-light bg-light"
              placeholder="password"
            />
          </div>
          <div class="p-3 border-0">
            <button type="button" class="btn btn-lg btn-warning text-dark w-100 rounded-pill">註冊</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Modal } from 'bootstrap'
export default {
  data () {
    return {
      loginModal: '',
      signinModal: ''
    }
  },
  mounted () {
    this.loginModal = new Modal(this.$refs.login)
    this.signinModal = new Modal(this.$refs.signin)
  },
  methods: {
    showLogInModal () {
      this.loginModal.show()
    },
    showSignInModal () {
      this.loginModal.hide()
      this.signinModal.show()
    }
  }
}
</script>
