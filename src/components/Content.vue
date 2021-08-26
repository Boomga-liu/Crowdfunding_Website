<template>
  <section class="content">
    <div class="content-title bg-white border-top border-bottom border-1 position-sticky top-0">
      <div class="container">
        <ul class="nav justify-content-between justify-content-md-start" id="myTab" role="tablist">
          <li class="nav-item" role="presentation">
            <a
              class="nav-link link-dark py-3 active fs-6"
              data-bs-toggle="tab"
              href="#project"
              role="tab"
            >專案介紹</a>
          </li>
          <li class="nav-item" role="presentation">
            <a
              class="nav-link link-dark py-3 fs-6"
              data-bs-toggle="tab"
              href="#quesition"
              role="tab"
            >常見問答</a>
          </li>
          <li class="nav-item" role="presentation">
            <a
              class="nav-link link-dark py-3 fs-6"
              data-bs-toggle="tab"
              href="#progress"
              role="tab"
            >目前進度</a>
          </li>
          <li class="nav-item" role="presentation">
            <a
              class="nav-link link-dark py-3 fs-6"
              id="contact-tab"
              data-bs-toggle="tab"
              href="#message"
              role="tab"
            >留言</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="my-5">
      <div class="container">
        <div class="row">
          <div class="col-md-7">
            <div class="tab-content" id="myTabContent">
              <div
                class="tab-pane fade show active mb-5"
                id="project"
                role="tabpanel"
                aria-labelledby="home-tab"
              >
                <img src="@/assets/images/p1.jpeg" class="img-fluid" alt="image" />
                <h4 class="mb-0 mt-4 px-3 border-start border-warning border-3">施了魔法的照片</h4>
                <p
                  class="mt-3 mb-4"
                >受就相法大夠局來畫師我只這然以放灣得的後人心年我物我年，或人有動與次出女親構算帶年行著所間女，外成認心香吸工並知日成展源大超時動為生葉衣致長山對精做英密差家他微熱建取示濟定心一，品定把別銀動，深青輪一物加，生明果。西業白老如天有表非民大條全那遊，李文遊、像香過元學須本致信校態麼資司媽人價在它，地他不我計孩廠然不大指勢生的華常簡岸然，人著母病石金萬得一果。</p>
                <img src="@/assets/images/p2.jpeg" class="img-fluid" alt="image" />
                <h4 class="mb-0 mt-4 px-3 border-start border-warning border-3">留下當下的美好</h4>
                <p
                  class="mt-3 mb-0"
                >受就相法大夠局來畫師我只這然以放灣得的後人心年我物我年，或人有動與次出女親構算帶年行著所間女，外成認心香吸工並知日成展源大超時動為生葉衣致長山對精做英密差家他微熱建取示濟定心一，品定把別銀動，深青輪一物加，生明果。西業白老如天有表非民大條全那遊，李文遊、像香過元學須本致信校態麼資司媽人價在它，地他不我計孩廠然不大指勢生的華常簡岸然，人著母病石金萬得一果。</p>
              </div>
              <div
                class="tab-pane fade mb-5"
                id="quesition"
                role="tabpanel"
                aria-labelledby="profile-tab"
              >
                <div class="accordion" id="accordionExample">
                  <div class="accordion-item mb-3">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q1"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q1</span>
                        影片拍完之後可以編輯嗎？
                      </button>
                    </h2>
                    <div id="Q1" class="accordion-collapse collapse show">
                      <div
                        class="accordion-body text-secondary"
                      >可以進行簡易的編輯，內建 5 種濾鏡，影片秒數有3秒、5秒、10秒可以選擇，拍完的當下可以編輯要印出來的影片範圍哦！</div>
                    </div>
                  </div>
                  <div class="accordion-item mb-3">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button collapsed"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q2"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q2</span>有提供保固或維修服務嗎？
                      </button>
                    </h2>
                    <div
                      id="Q2"
                      class="accordion-collapse collapse"
                      aria-labelledby="headingTwo"
                      data-bs-parent="#accordionExample"
                    >
                      <div
                        class="accordion-body text-secondary"
                      >This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables.</div>
                    </div>
                  </div>
                  <div class="accordion-item mb-3">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button collapsed"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q3"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q3</span>補充包底片要去哪裡購買呢？
                      </button>
                    </h2>
                    <div
                      id="Q3"
                      class="accordion-collapse collapse"
                      aria-labelledby="headingThree"
                      data-bs-parent="#accordionExample"
                    >
                      <div
                        class="accordion-body text-secondary"
                      >This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables.</div>
                    </div>
                  </div>
                  <div class="accordion-item mb-3">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button collapsed"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q4"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q4</span>印出來的拍立得照片需要充電嗎？
                      </button>
                    </h2>
                    <div
                      id="Q4"
                      class="accordion-collapse collapse"
                      aria-labelledby="headingThree"
                      data-bs-parent="#accordionExample"
                    >
                      <div
                        class="accordion-body text-secondary"
                      >This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables.</div>
                    </div>
                  </div>
                  <div class="accordion-item mb-3">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button collapsed"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q5"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q5</span>運送方式及付款方式有哪些呢？
                      </button>
                    </h2>
                    <div
                      id="Q5"
                      class="accordion-collapse collapse"
                      aria-labelledby="headingThree"
                      data-bs-parent="#accordionExample"
                    >
                      <div
                        class="accordion-body text-secondary"
                      >This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables.</div>
                    </div>
                  </div>
                  <div class="accordion-item">
                    <h2 class="accordion-header">
                      <button
                        class="accordion-button collapsed"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#Q6"
                      >
                        <span class="badge bg-warning text-dark ff-bt2 fs-6 px-2 py-2 me-3">Q6</span>退換貨方式及規則
                      </button>
                    </h2>
                    <div
                      id="Q6"
                      class="accordion-collapse collapse"
                      aria-labelledby="headingThree"
                      data-bs-parent="#accordionExample"
                    >
                      <div
                        class="accordion-body text-secondary"
                      >This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables.</div>
                    </div>
                  </div>
                </div>
              </div>
              <div
                class="tab-pane fade mb-5"
                id="progress"
                role="tabpanel"
                aria-labelledby="contact-tab"
              >
                <div class="card mb-3">
                  <div class="row g-0">
                    <div class="col-md-4">
                      <img src="@/assets/images/news01.jpeg" class="img-fluid w-100" alt="image" />
                    </div>
                    <div class="col-md-8">
                      <div class="card-body d-flex flex-column h-100">
                        <div class="card-title">
                          <h4 class="mb-0 fs-5">高雄體驗會｜免費參加送帆布袋</h4>
                          <small class="text-muted">2021-6-20</small>
                        </div>
                        <p
                          class="card-text text-secondary mt-2"
                        >大家安安！謝謝每位贊助者的熱情支持，讓我們離夢想更進一步，我們將於下個月舉辦體驗會，歡迎各位踴躍參與！</p>
                        <p class="card-text">
                          <a href="#" class="text-decoration-none" style="color:#FF785E;">more</a>
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="card mb-3">
                  <div class="row g-0">
                    <div class="col-md-4">
                      <img src="@/assets/images/news02.jpeg" class="img-fluid w-100" alt="image" />
                    </div>
                    <div class="col-md-8">
                      <div class="card-body d-flex flex-column h-100">
                        <div class="card-title">
                          <h4 class="mb-0 fs-5">高雄體驗會｜免費參加送帆布袋</h4>
                          <small class="text-muted">2021-6-20</small>
                        </div>
                        <p
                          class="card-text text-secondary mt-2"
                        >大家安安！謝謝每位贊助者的熱情支持，讓我們離夢想更進一步，我們將於下個月舉辦體驗會，歡迎各位踴躍參與！</p>
                        <p class="card-text">
                          <a href="#" class="text-decoration-none" style="color:#FF785E;">more</a>
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="card mb-3">
                  <div class="row g-0">
                    <div class="col-md-4">
                      <img src="@/assets/images/news03.jpeg" class="img-fluid w-100" alt="image" />
                    </div>
                    <div class="col-md-8">
                      <div class="card-body d-flex flex-column h-100">
                        <div class="card-title">
                          <h4 class="mb-0 fs-5">高雄體驗會｜免費參加送帆布袋</h4>
                          <small class="text-muted">2021-6-20</small>
                        </div>
                        <p
                          class="card-text text-secondary mt-2"
                        >大家安安！謝謝每位贊助者的熱情支持，讓我們離夢想更進一步，我們將於下個月舉辦體驗會，歡迎各位踴躍參與！</p>
                        <p class="card-text">
                          <a href="#" class="text-decoration-none" style="color:#FF785E;">more</a>
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div
                class="tab-pane fade mb-5"
                id="message"
                role="tabpanel"
                aria-labelledby="contact-tab"
              >
                <div class="p-3 border rounded mb-3">
                  <div class="d-flex align-items-center mb-3">
                    <img src="@/assets/images/user_img01.jpeg" class="img-fluid" alt="image" />
                    <div class="ms-2">
                      <h5 class="mb-0">王小明</h5>
                      <span class="text-secondary">2020年5月22日 11:32</span>
                    </div>
                  </div>
                  <p>晚上起床上廁所看到照片裡的人一直動其實有點恐怖，希望可以有暫停或是定時的功能！</p>
                  <div class="p-3 rounded" style="background-color:#F8F9FA;">
                    <span class="text-danger fs-sm">提案者回覆</span>
                    <p class="mb-0 mt-1">你要嘛起床的時候開燈，要嘛給我們更多錢開發阿</p>
                  </div>
                </div>
                <div class="p-3 border rounded mb-3">
                  <div class="d-flex align-items-center mb-3">
                    <img src="@/assets/images/user_img02.jpeg" class="img-fluid" alt="image" />
                    <div class="ms-2">
                      <h5 class="mb-0">王大明</h5>
                      <span class="text-secondary">2020年5月22日 11:32</span>
                    </div>
                  </div>
                  <p>希望有更多花色可以選擇！我女兒最近喜歡綠色</p>
                </div>
                <div class="p-3 border rounded mb-3">
                  <div class="d-flex align-items-center mb-3">
                    <img src="@/assets/images/user_img02.jpeg" class="img-fluid" alt="image" />
                    <div class="ms-2">
                      <h5 class="mb-0">帥哥</h5>
                      <span class="text-secondary">2020年5月22日 11:32</span>
                    </div>
                  </div>
                  <p>可以做個相簿功能嗎？拍出好看的影片再讓我們選擇要印出哪一張這樣</p>
                </div>
                <div class="p-3 border rounded mb-3">
                  <div class="d-flex align-items-center mb-3">
                    <img src="@/assets/images/user_img02.jpeg" class="img-fluid" alt="image" />
                    <div class="ms-2">
                      <h5 class="mb-0">美女</h5>
                      <span class="text-secondary">2020年5月22日 11:32</span>
                    </div>
                  </div>
                  <p>test123 看一下我是不是真的可以留言</p>
                </div>
              </div>
            </div>
            <ProjectSelection class="d-block d-md-none"></ProjectSelection>
            <Form></Form>
          </div>
          <div class="col-md-5">
            <ProjectSelection class="d-none d-md-block"></ProjectSelection>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Form from '@/components/Form.vue'
import ProjectSelection from '@/components/ProjectSelection.vue'
export default {
  data () {
    return {

    }
  },
  components: {
    Form,
    ProjectSelection
  }
}
</script>
