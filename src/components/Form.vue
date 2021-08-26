<template>
  <div class="form-area">
    <div class="d-flex justify-content-center">
      <img src="@/assets/images/icon_heart.svg" class="img-fluid" alt="image" />
    </div>
    <div class="position-relative my-4">
      <div class="progress bg-warning" style="height: 3px;">
        <div
          class="progress-bar"
          role="progressbar"
          aria-valuenow="0"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      <span class="position-absolute top-0 start-50 translate-middle bg-white px-3 h3 mb-0">贊助專案</span>
    </div>
    <form class="needs-validation" novalidate ref="Sponsorforms" @submit.prevent="feedBack">
      <div class="mb-3">
        <label for="project" class="form-label">贊助方案</label>
        <select
          id="project"
          class="form-select border-light bg-light text-muted"
          v-model="forms.plan"
          required
        >
          <option value selected disabled>請選擇一個方案</option>
          <option value="project-one">方案1</option>
          <option value="project-two">方案2</option>
        </select>
        <div class="invalid-feedback">請選擇方案</div>
      </div>
      <div class="mb-3">
        <label for="name" class="form-label">收件人姓名</label>
        <input
          type="name"
          id="name"
          class="form-control border-light bg-light"
          v-model="forms.name"
          required
        />
        <div class="invalid-feedback">請輸入姓名</div>
      </div>
      <div class="mb-3">
        <label for="phone" class="form-label">聯絡電話</label>
        <input
          type="number"
          id="phone"
          class="form-control border-light bg-light"
          v-model="forms.phone"
          required
        />
        <div class="invalid-feedback">請輸入電話</div>
      </div>
      <div class="mb-3">
        <label for="mail" class="form-label">聯絡信箱</label>
        <input
          type="mail"
          id="mail"
          class="form-control border-light bg-light"
          v-model="forms.mail"
          required
        />
        <div class="invalid-feedback">請輸入信箱</div>
      </div>
      <div class="mb-3">
        <label for="pay" class="form-label">付款方式</label>
        <select
          id="pay"
          class="form-select bg-light border-light text-muted"
          v-model="forms.pay"
          required
        >
          <option value="pay-one" selected>信用卡付款</option>
          <option value="pay-two">現金付款</option>
        </select>
        <div class="invalid-feedback">請選擇付款方式</div>
      </div>
      <div class="text-center mt-4">
        <button type="submit" class="btn btn-warning btn-lg text-dark rounded-pill px-5">贊助專案</button>
      </div>
    </form>
  </div>
</template>
<script>
export default {
  data () {
    return {
      Sponsorforms: '',
      forms: {
        plan: '',
        name: '',
        phone: '',
        pay: ''
      },
      checkResult: []

    }
  },
  methods: {
    PlanCheck () {
      if (this.forms.plan === '') {
        return false
      } else {
        return true
      }
    },
    NameCheck () {
      if (this.forms.plan === '') {
        return false
      } else {
        return true
      }
    },
    PhoneCheck (phone) {
      const regex = /^(09)[0-9]{8}$/
      if (!regex.test(phone)) {
        return false;
      } else {
        return true;
      }
    },
    MailCheck (mail) {
      const regex = /^([a-zA-Z0-9_\.\-\+])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/
      if (!regex.test(mail)) {
        return false;
      } else {
        return true;
      }
    },
    feedBack () {
      const isPlanCheck = this.PlanCheck()
      const isNameCheck = this.NameCheck()
      const isPhoneCheck = this.PhoneCheck(this.forms.phone)
      const isMailCheck = this.MailCheck(this.forms.mail)
      this.checkResult.push(isPlanCheck, isNameCheck, isPhoneCheck, isMailCheck)
      this.checkResult.forEach(item => {
        if (!item) {
          this.$refs.Sponsorforms.classList.add('was-validated')
        }
      })
    }
  }
}
</script>
