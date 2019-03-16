<template>
  <section>
    <!-- TOP -->
    <div class="top-wrap uk-position-relative uk-light uk-background-secondary">
      <!-- NAV -->
      <div
        class="nav"
        data-uk-sticky="cls-active: uk-background-secondary uk-box-shadow-medium; top: 100vh; animation: uk-animation-slide-top"
      >
        <div class="uk-container">
          <nav class="uk-navbar-container uk-navbar-transparent" data-uk-navbar>
            <div class="uk-navbar-right">
              <div class="uk-navbar-item uk-padding-remove-horizontal">
                <a class="uk-logo" title="Logo" href>
                  <img src="/img/marketing-logo.svg" alt="Logo">
                </a>
              </div>
            </div>
          </nav>
        </div>
      </div>
      <!-- /NAV -->
      <div class="uk-cover-container uk-light uk-flex uk-flex-middle top-wrap-height">
        <!-- TOP CONTAINER -->
        <div
          class="uk-container uk-flex-auto top-container uk-position-relative uk-margin-medium-top"
          data-uk-parallax="y: 0,50; easing:0; opacity:0.2"
        >
          <div
            class="uk-width-1-2@s"
            data-uk-scrollspy="cls: uk-animation-slide-left-medium; target: > *; delay: 150"
          >
            <h5 class="uk-text-primary uk-margin-small-bottom">کمپین</h5>
            <h1 class="uk-margin-remove-top">همیاری من و تو نه به تصادف</h1>
            <p class="subtitle-text uk-visible@s">
              ...وَمَنْ أَحْيَاهَا فَكَأَنَّمَا أَحْيَا النَّاسَ
              جَمِيعًا...
              <br>و هر كس كسى را زنده بدارد، چنان است كه گويى تمام مردم را زنده داشته است.(مائده
              32)
            </p>
            <a
              href="#"
              title="Learn More"
              class="uk-button uk-button-primary uk-border-pill"
              data-uk-scrollspy-class="uk-animation-fade"
            >بیشتر بخوانید...</a>
          </div>
        </div>
        <!-- /TOP CONTAINER -->
        <!-- TOP CONTAINER -->
        <div
          class="uk-container uk-flex-auto top-container uk-position-relative uk-margin-medium-top"
          data-uk-parallax="y: 0,50; easing:0; opacity:0.2"
        >
          <div
            class="uk-flex uk-flex-center uk-flex-middle uk-heightMarketing - UIkit 3 KickOffuk-light uk-position-relative uk-position-z-index"
          >
            <div class="uk-position-bottom-center uk-position-smalMarketing - UIkit 3 KickOffle@m"></div>
            <div class="uk-width-medium uk-padding-small" uk-scrollspy="cls: uk-animation-fade">
              <form @submit="login">
                <fieldset class="uk-fieldset">
                  <div class="uk-margin">
                    <div class="uk-inline uk-width-1-1">
                      <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: user"></span>
                      <input
                        id="username"
                        v-model="username"
                        class="uk-input uk-border-pill"
                        required
                        placeholder="نام کاربری"
                        type="text"
                      >
                    </div>
                  </div>
                  <div class="uk-margin">
                    <div class="uk-inline uk-width-1-1">
                      <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: lock"></span>
                      <input
                        id="password"
                        v-model="password"
                        class="uk-input uk-border-pill"
                        required
                        placeholder="کلمه عبور"
                        type="password"
                      >
                    </div>
                  </div>

                  <div class="uk-margin">
                    <label>
                      <input class="uk-checkbox" type="checkbox"> مرا به خاطر داشته باش.
                    </label>
                  </div>
                  <div class="uk-margin">
                    <button
                      type="submit"
                      class="uk-button uk-button-primary uk-border-pill uk-width-1-1"
                    >ورود</button>
                  </div>
                </fieldset>
              </form>
              <div>
                <div class="uk-text-center">
                  <a
                    class="uk-link-reset uk-text-small"
                    data-uk-toggle="target: #recover;animation: uk-animation-slide-top-small"
                  >
                    ثبت نام
                    نکرده اید؟
                  </a>
                </div>
                <div class="uk-margin-small-top" id="recover" hidden>
                  <form @submit="register">
                    <div class="uk-margin">
                      <div class="uk-inline uk-width-1-1">
                        <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: user"></span>
                        <input class="uk-input uk-border-pill" placeholder="کد معرف" type="text">
                      </div>
                    </div>
                    <div class="uk-margin">
                      <div class="uk-inline uk-width-1-1">
                        <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: lock"></span>
                        <input
                          id="phone"
                          v-model="phone"
                          class="uk-input uk-border-pill"
                          required
                          placeholder="تلفن همراه"
                          type="text"
                        >
                      </div>
                    </div>
                    <div class="uk-margin-small">
                      <button
                        type="submit"
                        class="uk-button uk-button-primary uk-border-pill uk-width-1-1"
                      >
                        ثبت
                        نام
                      </button>
                    </div>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- /TOP CONTAINER -->
        <!-- TOP IMAGE -->
        <img
          src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw=="
          data-srcset="https://picsum.photos/640/700/?image=816 640w,
				https://picsum.photos/960/700/?image=816 960w,
				https://picsum.photos/1200/900/?image=816 1200w,
				https://picsum.photos/2000/1000/?image=816 2000w"
          data-sizes="100vw"
          data-src="https://picsum.photos/1200/900/?image=816"
          alt
          data-uk-cover
          data-uk-img
          data-uk-parallax="opacity: 1,0.1; easing:0"
        >
        <!-- /TOP IMAGE -->
      </div>
      <div class="uk-position-bottom-center uk-position-medium uk-position-z-index uk-text-center">
        <a href="#content" data-uk-scroll="duration: 500" data-uk-icon="icon: arrow-down; ratio: 2"></a>
      </div>
    </div>
    <!-- /TOP -->
    <section id="content" class="uk-section uk-section-default">
      <div class="uk-container">
        <div class="uk-section uk-section-small uk-padding-remove-top">
          <ul
            class="uk-subnav uk-subnav-pill uk-flex uk-flex-center"
            data-uk-switcher="connect: .uk-switcher; animation: uk-animation-fade"
          >
            <li>
              <a class="uk-border-pill" href="#">جدول امتیازات</a>
            </li>
            <li>
              <a class="uk-border-pill" href="#">شرکت در آزمون ها</a>
            </li>
          </ul>
        </div>

        <ul class="uk-switcher uk-margin">
          <li>
            <table class="uk-table uk-table-justify uk-table-divider">
              <caption>اسامی پنج نفر برتر سایت تا این لحظه</caption>
              <thead>
                <tr>
                  <th>رتبه</th>
                  <th>نام کاربری</th>
                  <th>مجموع امتیازات</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(item, index) in users" :key="item.username">
                  <td>{{ index+1 }}</td>
                  <td>{{ item.username }}</td>
                  <td>{{ item.score }}</td>
                </tr>
              </tbody>
            </table>
          </li>
          <li>
            <div class="uk-child-width-1-1@s" uk-grid>
              <div>
                <div uk-grid>
                  <div class="uk-width-auto@m">
                    <ul
                      class="uk-tab-right"
                      uk-tab="connect: #component-tab-right; animation: uk-animation-fade"
                    >
                      <li>
                        <a id="learningfile" aria-expanded="true" href="#">فایل های آموزشی</a>
                      </li>
                      <li>
                        <a id="questions" aria-expanded="false" href="#">آزمون ها</a>
                      </li>
                      <li>
                        <a id="result" aria-expanded="false" href="#">نتیجه و رتبه بندی</a>
                      </li>
                    </ul>
                  </div>
                  <div class="uk-width-expand@m">
                    <ul id="component-tab-right" class="uk-switcher">
                      <li id="lilearningfile">
                        <table class="uk-table uk-table-justify uk-table-divider">
                          <thead>
                            <tr>
                              <th class="k-child-width-1-8@s">ردیف</th>
                              <th class="uk-width-small">موضوع</th>
                              <th>توضیحات</th>
                              <th class="uk-width-small">تاریخ شروع آزمون</th>
                              <th></th>
                            </tr>
                          </thead>
                          <tbody>
                            <tr v-for="(item, index) in quizzes" :key="item.id">
                              <td>{{index+1}}</td>
                              <td>
                                <a :href="item.file">دریافت فایل آموزشی</a>
                              </td>
                              <td>{{item.name}}</td>
                              <td>{{ item.date}}</td>
                              <td>
                                <button
                                  @click="quiz(item.questions)"
                                  class="uk-button uk-button-default"
                                  type="button"
                                >شروع آزمون</button>
                              </td>
                            </tr>
                          </tbody>
                        </table>
                      </li>

                      <li id="liquestions">
                        <div
                          class="uk-child-width-1-1@m"
                          uk-grid
                          uk-scrollspy="cls: uk-animation-fade; target: > div > .uk-card; delay: 500; repeat: true"
                        >
                          <form id="formquiz" @submit="submitquize">
                            <button
                              type="submit"
                              class="uk-button uk-button-primary uk-width-1-1 uk-margin-small-bottom"
                            >ارسال جواب ها</button>
                          </form>
                        </div>
                      </li>

                      <li>
                        <div
                          class="uk-child-width-1-2@m uk-grid-match"
                          uk-grid
                          uk-scrollspy="cls: uk-animation-fade; target: > div > .uk-card; delay: 500; repeat: true"
                        >
                          <div>
                            <div class="uk-card uk-card-default uk-card-body">
                              <h3 class="uk-card-title">امتیازات شما</h3>
                              <p>امتیاز حاصل از دعوت افراد و آزمون ها</p>
                            </div>
                          </div>
                          <div>
                            <div class="uk-card uk-card-default uk-card-body">
                              <h3 class="uk-card-title">رتبه بندی</h3>
                              <p>نمایش رتبه</p>
                            </div>
                          </div>
                        </div>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </section>

    <section class="uk-section uk-section-secondary uk-section-large">
      <div class="uk-container">
        <div class="uk-grid uk-child-width-1-2@l uk-flex-middle">
          <div>
            <h6>کمپین نوروزی</h6>
            <h2 class="uk-margin-small-top uk-h1">چطور می توانم جان افراد را نجات دهم</h2>
            <p class="subtitle-text">
              جهت شرکت در کمپین فرم اطلاعات رو به رو را پر کرده تا با شما تماس بگیریم. اگر شرکت کنی امتیاز
              کمپین رو هم دریافت میکنی.مطابی رو هم که باید توی فرم پر کنه بازه حضور و مکان هایی که راغب به
              حضور توشونه
            </p>
            <a
              href="#"
              class="uk-button uk-button-primary uk-border-pill"
              data-uk-icon="arrow-left"
            >
              بیشتر
              بخوانید
            </a>
          </div>
          <div
            class="uk-flex uk-flex-center uk-flex-middle uk-heightMarketing - UIkit 3 KickOffuk-light uk-position-relative uk-position-z-index"
          >
            <div class="uk-position-bottom-center uk-position-smalMarketing - UIkit 3 KickOffle@m"></div>
            <div class="uk-width-medium uk-padding-small" uk-scrollspy="cls: uk-animation-fade">
              <form action="login-dark.html">
                <fieldset class="uk-fieldset">
                  <div class="uk-margin">
                    <div class="uk-inline uk-width-1-1">
                      <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: user"></span>
                      <input
                        class="uk-input uk-border-pill"
                        required
                        placeholder="نام کاربری"
                        type="text"
                      >
                    </div>
                  </div>
                  <div class="uk-margin">
                    <div class="uk-inline uk-width-1-1">
                      <span class="uk-form-icon uk-form-icon-flip" data-uk-icon="icon: lock"></span>
                      <input
                        class="uk-input uk-border-pill"
                        required
                        placeholder="کلمه عبور"
                        type="password"
                      >
                    </div>
                  </div>

                  <div class="uk-margin">
                    <label>
                      <input class="uk-checkbox" type="checkbox"> مرا به خاطر داشته باش.
                    </label>
                  </div>
                  <div class="uk-margin">
                    <button
                      type="submit"
                      class="uk-button uk-button-primary uk-border-pill uk-width-1-1"
                    >ورود</button>
                  </div>
                </fieldset>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- BOTTOM -->
    <!-- BOTTOM -->
    <!-- LOGOS -->
    <!-- /LOGOS -->
    <!-- FOOTER -->
    <footer class="uk-section uk-section-secondary uk-padding-remove-bottom">
      <div class="uk-container">
        <div class="uk-grid uk-grid-large" data-uk-grid>
          <div class="uk-width-1-2@m">
            <h5>درباره ما</h5>
            <p>
              اینجا باید یک متن درباره ما قرار گیرد و تمامی حقوق مربوط به ماست و کلی چیز دیگه و میتونن با این
              ایمیل در ارتباط باشند:
              <a
                href="#"
                title
              >info@company.com</a>
            </p>
            <div>
              <a href class="uk-icon-button" data-uk-icon="twitter"></a>
              <a href class="uk-icon-button" data-uk-icon="facebook"></a>
              <a href class="uk-icon-button" data-uk-icon="instagram"></a>
            </div>
          </div>
        </div>
      </div>

      <div class="uk-text-center uk-padding uk-padding-remove-horizontal">
        <span class="uk-text-small uk-text-muted">
          © 2019 Marketing Layout -
          <a href="https://github.com/zzseba78/Kick-Off">نیرو گرفته از ما</a> | ساخته شده با
          <a
            href="http://getuikit.com"
            title="Visit UIkit 3 site"
            target="_blank"
            data-uk-tooltip
          >
            <span data-uk-icon="uikit"></span>
          </a>
        </span>
      </div>
    </footer>
    <!-- /FOOTER -->
    <!-- OFFCANVAS -->
    <div id="offcanvas-nav" data-uk-offcanvas="flip: true; overlay: false">
      <div class="uk-offcanvas-bar uk-offcanvas-bar-animation uk-offcanvas-slide">
        <button class="uk-offcanvas-close uk-close uk-icon" type="button" data-uk-close></button>
        <ul class="uk-nav uk-nav-default">
          <li class="uk-active">
            <a href="#">Active</a>
          </li>
          <li class="uk-parent">
            <a href="#">Parent</a>
            <ul class="uk-nav-sub">
              <li>
                <a href="#">Sub item</a>
              </li>
              <li>
                <a href="#">Sub item</a>
              </li>
            </ul>
          </li>
          <li class="uk-nav-header">Header</li>
          <li>
            <a href="#js-options">
              <span class="uk-margin-small-left uk-icon" data-uk-icon="icon: table"></span>
              Item
            </a>
          </li>
          <li>
            <a href="#">
              <span class="uk-margin-small-left uk-icon" data-uk-icon="icon: thumbnails"></span>
              Item
            </a>
          </li>
          <li class="uk-nav-divider"></li>
          <li>
            <a href="#">
              <span class="uk-margin-small-left uk-icon" data-uk-icon="icon: trash"></span> Item
            </a>
          </li>
        </ul>
        <h3>Title</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
          dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
          ex ea commodo consequat.
        </p>
      </div>
    </div>
    <!-- /OFFCANVAS -->
  </section>
</template>

<script>
const uuidv4 = require("uuid/v4");
import axios from "axios";

export default {
  async asyncData(context) {
    let leaderboard = await axios.get(
      'http://[::1]:8080/users?filter={"order":"score DESC","limit":5}'
    );

    let quizzes = await axios.get(
      'http://[::1]:8080/quizzes?filter={"order":"date DESC","limit":5}'
    );

    return {
      phone: "",
      username: "",
      password: "",
      users: leaderboard.data,
      quizzes: quizzes.data
    };
  },
  methods: {
    login(e) {
      e.preventDefault();
      let path =
        'http://[::1]:8080/users?filter={"where":{"username":"' +
        this.username +
        '","password":"' +
        this.password +
        '"}}';
      axios.get(path).then(
        sux => {
          if (sux.data === []) {
            return window.alert("ابتدا در سیستم ثبت نام کنید");
          }

          window.alert("ورود با موفقیت انجام شد");
          Object.assign(this.$data, {
            username: this.username,
            password: this.password
          });

          document.getElementById("username").text = "";
          document.getElementById("username").value = "";
          document.getElementById("password").text = "";
          document.getElementById("password").value = "";
        },
        err => {
          window.alert("مشکلی در زمان ورود به سیستم رخ داده");
        }
      );
    },
    register(e) {
      e.preventDefault();

      Object.assign(this.$data, {
        username: this.username,
        password: this.password
      });

      axios
        .post("http://[::1]:8080/users", {
          id: uuidv4(),
          username: this.username,
          password: this.password,
          phone: this.phone
        })
        .then(
          sux => {
            window.alert("ثبت نام با موفقیت انجام شد");
          },
          err => {
            window.alert("ایراد در هنگام ثبت نام رخ داده است");
          }
        );
    },
    quiz(questions) {
      document
        .getElementById("learningfile")
        .setAttribute("aria-expanded", "false");
      document
        .getElementById("learningfile")
        .parentNode.setAttribute("class", "");
      document.getElementById("lilearningfile").setAttribute("class", "");
      document
        .getElementById("questions")
        .setAttribute("aria-expanded", "true");
      document
        .getElementById("questions")
        .parentNode.setAttribute("class", "uk-active");
      document.getElementById("liquestions").setAttribute("class", "uk-active");

      var iter = 0;
      let fq = document.getElementById("formquiz");
      var q =
        '<div class="uk-card uk-card-default uk-card-body"><p>{0}</p><div class="uk-margin uk-grid-small uk-child-width-auto uk-grid"><label><input class="uk-radio" type="radio" name="radio{1}">{2}</label><label><input class="uk-radio" type="radio" name="radio{1}">{3}</label><label><input class="uk-radio" type="radio" name="radio{1}">{4}</label><label><input class="uk-radio" type="radio" name="radio{1}">{5}</label></div></div>';
      questions.forEach(element => {
        var _q = q.replace("{0}", element.q);
        _q = _q.split("{1}").join(iter);
        var ops = element.ops.split("$");
        _q = _q.replace("{2}", ops[0]);
        _q = _q.replace("{3}", ops[1]);
        _q = _q.replace("{4}", ops[2]);
        _q = _q.replace("{5}", ops[3]);
        iter = iter + 1;
        fq.innerHTML = _q + fq.innerHTML;
      });
    }
  }
};
</script>
