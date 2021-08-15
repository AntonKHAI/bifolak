<template>
  <div class="main">
    <b-navbar fixed="top" class="justify-content-between">
      <b-navbar-brand href="#" class="title text-uppercase">
        Бифолак<sup>®</sup>
      </b-navbar-brand>

      <b-collapse is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto nav-desktop">
          <b-nav-item @click="scrollToBlock('#vaginal')">Вагинальный дисбиоз</b-nav-item>
          <b-nav-item @click="scrollToBlock('#how-fix')">Как лечить?</b-nav-item>
          <b-nav-item @click="scrollToBlock('#why')">Почему Бифолак?</b-nav-item>
          <b-nav-item @click="scrollToBlock('#how-use')">Как использовать Бифолак?</b-nav-item>
          <b-nav-item @click="scrollToBlock('#buy')">Где купить?</b-nav-item>
        </b-navbar-nav>
        <div id="hamburger" v-b-toggle.sidebar-1 header-close class="nav-mobile" :class="{ 'open': openSidebar }" @click="toggle">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </b-collapse>
    </b-navbar>
    <div>
      <b-sidebar id="sidebar-1" backdrop shadow @hidden="toggle" v-if="openSidebar">
        <template #header>
          <span class="green-title text-uppercase">
            Бифолак<sup>®</sup>
          </span>
        </template>
        <div class="px-2">
          <div class="mob-nav-item pointer" @click="scrollToBlock('#vaginal')">Вагинальный дисбиоз</div>
          <div class="mob-nav-item pointer" @click="scrollToBlock('#how-fix')">Как лечить?</div>
          <div class="mob-nav-item pointer" @click="scrollToBlock('#why')">Почему Бифолак?</div>
          <div class="mob-nav-item pointer" @click="scrollToBlock('#how-use')">Как использовать Бифолак?</div>
          <div class="mob-nav-item pointer" @click="scrollToBlock('#buy')">Где купить?</div>
        </div>
        <hr>
        <div class="flex my-2 mob-nav-item">
          <a href="#">
            <img src="../assets/Instagram.png" alt="" class="mb-2 mx-1" style="max-width: 35px">
          </a>
          <a href="#">
            <img src="../assets/Facebook.png" alt="" class="mb-2 mx-1" style="max-width: 35px">
          </a>
        </div>
      </b-sidebar>
    </div>
    <div class="mt-5 py-2">
      <div class="mb-4 px-3">
        <h2 class="main-title mt-2">
          БЕРЕЖНАЯ КОРРЕКЦИЯ <br>
          МИКРОФЛОРЫ ВЛАГАЛИЩА
        </h2>
      </div>
      <div class="mb-4">
        <img src="../assets/roses.jpg" alt="main" style="max-width: 100%">
      </div>
      <p class="text-justify mb-4 px-3" id="vaginal">
        В норме во влагалище у женщины обитает так называемая <b>нормальная микрофлора</b>. Она состоит примерно <b>на 90% из лактобактерий, на 10% - из бифидобактерий</b>, и меньше 1% составляют так называемые «ключевые клетки влагалища». Нормальная микрофлора находится в постоянном равновесии между собой и с окружающей средой. Она не допускает появление никакой другой инфекции, и не допускает изменение соотношения возбудителей, живущих во влагалище в норме.
      </p>
      <div class="mt-2 mb-4 px-3">
        <img src="../assets/list.jpeg" alt="main" style="max-width: 100%">
      </div>
      <div class="colored-block">
        <b>Дисбактериоз влагалища (дисбиоз)</b> – нарушения естественной микрофлоры, которое характеризуется изменением равновесия между полезными и патогенными «обитателями» флоры. Данный процесс сопровождается снижением количества бифидо- и лактобактерий и увеличением численности возбудителя заболевания.
      </div>
    </div>
     <b-container fluid>
      <b-row data-aos="fade-up" class="mt-1 px-3 py-1">
        <h2 class="mb-4 main-block-title" style="color: #333333">
          На изменение микрофлоры влияет множество факторов
        </h2>
        <b-col md="2" sm="12" class="flex justify-content-center mb-3">
          <img src="../assets/snow.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
              Переохлаждение организма
            </span>
            <br>
            Как однократное сильное переохлаждение, так и постоянное замерзание. Все это ведет к снижению общего и местного иммунитета, что сказывается и на вагинальной микрофлоре.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-3">
          <img src="../assets/clear.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
              Неправильное использование тампонов при месячных
            </span>
            <br>
            Тампоны следует менять строго каждые 2 часа и днем, и ночью. Это достаточно неудобно, но иначе во влагалище создаются хорошие условия для роста инфекции.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-3">
          <img src="../assets/bull.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
             Изменения и нарушения гормонального фона
            </span>
            <br>
           Сюда можно отнести нерегулярную половую жизнь, беременность, роды, аборты, любые виды нарушений цикла, половое созревание, предклимакс и климакс и т.д.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-3">
          <img src="../assets/arrow.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
              Инфекционно-воспалительные заболевания
            </span>
            <br>
            Любые инфекционно-воспалительные заболевания органов малого таза, инфекции передающиеся половым путем.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-3">
          <img src="../assets/couple.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
             Беспорядочная половая жизнь
            </span>
            <br>Большое количество половых партнеров, пренебрежение средствами контрацепции.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-2">
          <img src="../assets/plane.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
              Смена климатической зоны
            </span>
            <br>
            Случаются обострения дисбиоза влагалища во время поездок в теплые страны.
          </p>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-1">
        <b-col md="2" sm="12" class="flex justify-content-center mb-2">
          <img src="../assets/stuff.jpg" alt="main" style="max-width: 120px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <p>
            <span class="green-title">
              Лекарственные препараты
            </span>
            <br>
            Лечение антибиотиками, особенно продолжительное или многократное.
          </p>
        </b-col>
      </b-row>
     </b-container>
    <h2 class="main-block-title purple-title py-2">
      Симптомы <br> вагинального дисбиоза
    </h2>
     <div>
       <b-container fluid>
      <b-row data-aos="fade-up" class="px-3 py-3">
        <b-col md="2" sm="12" class="flex justify-content-center mb-4">
          <img src="../assets/tap.png" alt="main" style="max-width: 40%; max-height: 300px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <ul>
            <li class="mb-1 text-justify">
              первоначально бели сероватого цвета, с развитием патологического состояния цвет становится желтовато-зеленый;
            </li>
            <li class="mb-1 text-justify">
              при длительном течении бели становятся липкими и пенистыми;
            </li>
            <li class="mb-1 text-justify">
              обильные выделения (бели): до 20-30 мл в сутки;
            </li>
          </ul>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-3">
        <b-col md="2" sm="12" class="flex justify-content-center mb-4">
          <img src="../assets/fish.png" alt="main" style="max-width: 40%; max-height: 300px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
          <ul>
            <li class="mb-1 text-justify">
              выделения имеют неприятный (рыбный) запах, который усиливается после полового акта и во время месячных;
            </li>
          </ul>
        </b-col>
      </b-row>
      <b-row data-aos="fade-up" class="px-3 py-3">
        <b-col md="2" sm="12" class="flex justify-content-center mb-4">
          <img src="../assets/heart.png" alt="main" style="max-width: 40%; max-height: 300px">
        </b-col>
        <b-col md="10" sm="12" class="flex justify-content-md-start align-items-center">
         <ul>
           <li class="mb-1 text-justify">
            зуд и жжение во влагалище;
           </li>
           <li class="mb-1 text-justify">
            дизурические расстройства;
           </li>
           <li class="mb-1 text-justify">
            болезненность при половом акте;
           </li>
         </ul>
        </b-col>
      </b-row>
     </b-container>
      <h6 data-aos="zoom-out-up" class="mb-4 colored-block" id="how-fix">
        Необходимо знать и помнить, что <b>нарушенный баланс микрофлоры повышает риск развития воспалительных и инфекционных заболеваний</b>.
      </h6>

       <b-container>
         <div data-aos="zoom-out-up" class="text-justify">
           <b>Основные принципы лечения</b> дисбиоза влагалища направлены на подавление роста болезнетворных и условно-патогенных бактерий с последующим восстановлением численности лактобактерий. Поэтому лечение женщин с бактериальным вагинозом рекомендуется проводить <b>в два этапа:</b>
         </div>
       </b-container>

      <div class="mt-3">
        <div class="mb-2">
          <div data-aos="zoom-out-up">
            <b-container fluidxs>
              <h3 style="font-size: 18px">
                <span class="green-title mr-1" style="font-size: 22px"> 1 этап: </span>  ликвидация «плохих» бактерий;
              </h3>
              <h3 style="font-size: 18px">
                <span class="green-title mr-1" style="font-size: 22px"> 2 этап: </span>  восстановление численного количества лактобактерий.
            </h3>
            </b-container>
            <img src="../assets/bio.jpg" alt="" style="max-width: 100%">
          </div>
        </div>
        <b-container fluidxs>
          <div data-aos="zoom-out-up" class="text-justify">
            Необходимость второго этапа обусловлена тем, что антимикробные средства помимо подавления роста болезнетворных бактерий оказывают также отрицательное значение и на численность лактобактерий, обеспечивающих в норме защитную функцию. Поэтому для скорейшего обеспечения их численного превосходства в экосистеме половых путей <b>специалисты рекомендуют курсовое применение специальных «женских» пробиотиков.</b>
          </div>
        </b-container>
      </div>

       <div class="mb-5 py-3 mt-5 purple-title main-title">
         БИФОЛАК – СУППОЗИТОРИИ ДЛЯ ЭФФЕКТИВНОГО ВОССТАНОВЛЕНИЯ ВАГИНАЛЬНОЙ МИКРОФЛОРЫ
       </div>

      <div class="mt-3 px-2" id="why">
        <div class="main-block-title mb-2 pt-2">
          Почему Бифолак?
        </div>
        <div data-aos="zoom-out-up" class="slide-wrap">
          <b-container fluid>
          <VueSlickCarousel v-bind="settings">
            <div><img src="../assets/1slide.jpg" alt="" class="slide-img"></div>
            <div><img src="../assets/2slide.jpg" alt="" class="slide-img"></div>
            <div><img src="../assets/3slide.jpg" alt="" class="slide-img"></div>
            <div><img src="../assets/4slide.jpg" alt="" class="slide-img"></div>
            <div><img src="../assets/5slide.jpg" alt="" class="slide-img"></div>
            <div><img src="../assets/6slide.jpg" alt="" class="slide-img"></div>
          </VueSlickCarousel>
          </b-container>
        </div>
      </div>

      <b-container fluid>
        <div data-aos="zoom-out-up" class="mt-5" id="how-use">
          <div class="mb-3 main-block-title">
            Как использовать Бифолак?
          </div>
          <h4 style="font-size: 20px; letter-spacing: 1.3px">
            Бифолак применяют <br> по <b>1-2</b> суппозитория <br>в течении <b>10</b> дней <b>на ночь</b>
          </h4>
          <img class="mb-1" src="../assets/how-use2.png" alt="" style="max-width: 70%">
          <h6 class="mb-3 descr">
            Суппозитории растворяются во влагалище и могут вытекать вместе с выделениями, поэтому их лучше всего вводить перед сном
          </h6>

          <ol class="gradient-list">
            <li data-aos="fade-up">Посетите туалет и сделайте гигиенические процедуры без использования мыла и других моющих средств, только водой.</li>
            <li data-aos="fade-up">Манипуляции проводятся руками, так что тщательно их вымойте или воспользуйтесь напальчником или перчаткой.</li>
            <li data-aos="fade-up">Оторвите или отрежьте упаковку с одним суппозиторием.</li>
            <li data-aos="fade-up">Чтобы раскрыть упаковку, со стороны острого конца свечи потяните за «ушки» в разные стороны. Упаковка отрывается очень легко!</li>
            <li data-aos="fade-up">Принять лежачее положение и пальцем ввести свечу, как можно глубже, во влагалище.</li>
            <img data-aos="fade-up" src="../assets/how-use1.jpg" alt="" style="max-width: 320px">
            <div class="mb-4">
              Схема введения свечи во влагалище
            </div>
            <li data-aos="fade-up">На этом все. В течение получаса нежелательно вставать, чтобы свеча успела растаять во влагалище. После введения суппозиторий используйте обычную или ежедневную прокладку, чтобы собрать выделения.</li>
          </ol>
          <img src="../assets/how-use3.jpeg" alt="" style="max-width: 80%">
        </div>
      </b-container>
      <div class="px-3 py-3 mt-1">
        <div data-aos="zoom-out-up">
          <div class="main-block-title">
            ПРИОБРЕСТИ <span style="color: #2e6525">БИФОЛАК</span> МОЖНО ЗДЕСЬ
          </div>
        </div>
        <b-container data-aos="zoom-out-up" fluid>
          <b-row class="mt-2 px-3 py-3 justify-content-between">
            <b-col md="6" sm="12" class="flex justify-content-center mb-4">
              <div class="card-link card-link__liki-24" @click="buyIn('https://liki24.com/uk/search/?q=%D0%B1%D0%B8%D1%84%D0%BE%D0%BB%D0%B0%D0%BA')">
                <div class="light-blue-title">
                  LIKI 24
                </div>
              </div>
            </b-col>
            <b-col id="buy" md="6" sm="12" class="flex justify-content-center mb-4">
              <div class="card-link card-link__tabletki" @click="buyIn('https://tabletki.ua/uk/Бифолак-Печаевские/1040776/pharmacy/kharkov/')">
                <div class="green-title">
                  TABLETKI.UA
                </div>
              </div>
            </b-col>
          </b-row>
        </b-container>
<!--        <b-container fluid>-->
<!--          <b-row class="mt-5 px-3 py-3 justify-content-between">-->
<!--            <b-col class="flex justify-content-center mb-4">-->
<!--              <div class="card-link card-link__invert" @click="buyIn('https://t.me/alexandrarebrova')">-->
<!--                <div>-->
<!--                  Консультант по продукту-->
<!--                </div>-->
<!--              </div>-->
<!--            </b-col>-->
<!--          </b-row>-->
<!--        </b-container>-->
        <h6 data-aos="zoom-out-up" class="mb-2">
          <div class="mb-3 main-block-title" style="color: #333333">
            Остались вопросы или <br>не можете найти <br> <span style="color: #2e6525">Бифолак</span> в аптеке?
          </div>
          <b>Выберите свой город</b> для связи с нашим консультантом и мы <b>обязательно поможем Вам</b>
        </h6>
        <b-container data-aos="zoom-out-up" fluid>
          <b-row class="flex-column px-3 py-3 justify-content-between">
            <b-col class="flex justify-content-center mb-4">
              <vSelect
                  style="width: 300px"
                  v-model="consultant"
                  label="place"
                  placeholder="Выберите город"
                  :clearable="false"
                  :filterable="false"
                  :options="options"
                  :searchable="false"
              />
            </b-col>
            <b-col v-if="consultant" class="flex justify-content-center mb-4">
              <img src="../assets/phone.png" alt="" style="max-width: 36px; margin-right: 6px; border-radius: 50%;">
              <div class="card-link__call flex">
                <div>
                  <a :href="`tel:${consultant.phone}`" type="tel">
                    Позвонить
                  </a>
                </div>
              </div>
            </b-col>
            <b-col v-if="consultant" class="flex justify-content-center mb-4">
              <img src="../assets/telegram.png" alt="" style="max-width: 36px; margin-right: 6px">
              <div class="card-link__telegram flex" @click="buyIn(`https://t.me/${consultant.nick}`)">
                  <div>
                    Связаться через Telegram
                  </div>
              </div>
            </b-col>
          </b-row>
        </b-container>
      </div>
    </div>
    <b-container fluid>
      <div class="mb-1 social-title" style="color: #333333">
        Мы в социальных сетях
      </div>
      <div class="flex justify-content-center">
        <a href="#">
          <img src="../assets/Instagram.png" alt="" class="mb-2 mx-1" style="max-width: 45px">
        </a>
        <a href="#">
          <img src="../assets/Facebook.png" alt="" class="mb-2 mx-1" style="max-width: 43px">
        </a>
      </div>
    </b-container>
    <img src="../assets/not-lik.jpg" alt="" class="mb-3" style="max-width: 90%">
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

import AOS from 'aos';
import 'aos/dist/aos.css';

import vSelect from 'vue-select'

export default {
  name: 'HelloWorld',
  components: {
    VueSlickCarousel,
    vSelect
  },
  props: {
    msg: String
  },
  data() {
    return {
      openSidebar: false,
      consultant: null,
      options: [
        {
          phone: '0 (66) 770 90 94',
          place: 'Киев',
          nick: 'nik_lek'
        },
        {
          phone: '0 (50) 468 85 76',
          place: 'Днепр',
          nick: 'YevgeniyVdn'
        },
        {
          phone: '0 (99) 945 82 96',
          place: 'Запорожье',
          nick: 'kostyayasen'
        },
        {
          phone: '0 (99) 028 21 79',
          place: 'Николаев',
          nick: 'mariiasolovyova'
        },
        {
          phone: '0 (99) 316 26 60',
          place: 'Херсон',
          nick: 'Vadimdymchenko'
        },
        {
          phone: '0 (95) 893 59 16',
          place: 'Харьков',
          nick: 'alexandrarebrova'
        },
        {
          phone: '0 (95) 931 56 78',
          place: 'Полтава',
          nick: 'Vladislavperederii'
        },
      ],
      settings: {
        "dots": true,
        "autoplay": true,
        autoplaySpeed: 4500,
        "infinite": true,
        // arrows: true,
        "speed": 500,
        "slidesToShow": 2,
        "slidesToScroll": 2,
        "initialSlide": 0,
        "responsive": [
          {
            "breakpoint": 1024,
            "settings": {
              "slidesToShow": 3,
              "slidesToScroll": 3,
              "infinite": true,
              "dots": true
            }
          },
          {
            "breakpoint": 600,
            "settings": {
              "slidesToShow": 2,
              "slidesToScroll": 2,
              "initialSlide": 2
            }
          },
          {
            "breakpoint": 480,
            "settings": {
              "slidesToShow": 1,
              "slidesToScroll": 1
            }
          }
        ]
      }
    }
  },
  created() {
    AOS.init();
  },
  methods: {
    buyIn(link) {
      window.open(
          link,
          '_blank' // <- This is what makes it open in a new window.
      );
    },

    toggle() {
      this.openSidebar = !this.openSidebar
    },

    scrollToBlock(id) {
      document.querySelector(id).scrollIntoView({behavior: 'smooth', block: 'start'});
      document.querySelector(id).scrollTop -= 100;
      this.openSidebar = false
    }
  }
}
</script>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css?family=Montserrat:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i&display=swap&subset=cyrillic');

$main-green: '#eee';
$black: #1d1f20;
$blue: #83e4e2;
$green: #a2ed56;
$yellow: #fddc32;
$white: #fafafa;

.main-title {
  font-weight: bold;
  letter-spacing: 1.5px;
}

.main-block-title {
  font-weight: bold;
  font-size: 20px;
}

.social-title {
  font-size: 18px;
}

.title {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 22px;
  padding: 0 !important;
  color: #fff !important;
}

%boxshadow {
  box-shadow: 0.25rem 0.25rem 0.6rem rgba(0,0,0,0.05), 0 0.5rem 1.125rem rgba(75,0,0,0.05);
}

ol.gradient-list {
  counter-reset: gradient-counter;
  list-style: none;
  margin: 1.75rem 0;
  padding-left: 1rem;
  > li {
    background: white;
    border-radius: 0 0.5rem 0.5rem 0.5rem;
    @extend %boxshadow;
    counter-increment: gradient-counter;
    min-height: 3rem;
    max-width: 800px;
    margin: 0 auto;
    margin-top: 1rem;
    padding: 1rem 1rem 1rem 3rem;
    position: relative;
    &::before,
    &::after {
      background: linear-gradient(135deg, $blue 0%,$green 100%);
      border-radius: 1rem 1rem 0 1rem;
      content: '';
      height: 3rem;
      left: -1rem;
      overflow: hidden;
      position: absolute;
      top: -1rem;
      width: 3rem;
    }
    &::before {
      align-items: center;
      @extend %boxshadow;
      content: counter(gradient-counter);
      color: $black;
      display: flex;
      font: 900 1.5em/1 'Montserrat';
      justify-content: center;
      padding: 0.125em 0.25em;
      z-index: 1;
    }
    @for $i from 1 through 5 {
      &:nth-child(10n+#{$i}):before {
        background: linear-gradient(135deg, rgba($green, $i * 0.2) 0%,rgba($yellow, $i * 0.2) 100%);
      }
    }
    @for $i from 6 through 10 {
      &:nth-child(10n+#{$i}):before {
        background: linear-gradient(135deg, rgba($green, 1 - (($i - 5) * 0.2)) 0%,rgba($yellow, 1 - (($i - 5) * 0.2)) 100%);
      }
    }
    + li {
      margin-top: 2rem;
    }
  }
}

#hamburger {
  width: 35px;
  height: 30px;
  display: block;
  position: relative;
  float: right;
  transform: rotate(0deg);
  transition: .5s ease-in-out;
  cursor: pointer;
}
#hamburger span {
  display: block;
  position: absolute;
  height: 4px;
  width: 100%;
  background: white;
  border-radius: 9px;
  opacity: 1;
  left: 0;
  transform: rotate(0deg);
  transition: .25s ease-in-out;
}
#hamburger span:nth-child(1) {
  top: 0px;
}
#hamburger span:nth-child(2) {
  top: 12px;
}
#hamburger span:nth-child(3) {
  top: 24px;
}
#hamburger.open span:nth-child(1) {
  top: 14px;
  transform: rotate(135deg);
}
#hamburger.open span:nth-child(2) {
  opacity: 0;
  left: -60px;
}
#hamburger.open span:nth-child(3) {
  top: 14px;
  transform: rotate(-135deg);
}

.slick-prev:before,
.slick-next:before {
    font-family:initial!important;
    color:red;
}
.pointer {
  cursor: pointer;
}

.text-justify {
  text-align: justify;
}

.flex {
  display: flex !important;
}

.navbar {
  padding: .5rem 1rem;
  background-color: #079045ab;
  -webkit-backdrop-filter: blur(7px);
  backdrop-filter: blur(7px);
}

.navbar-collapse {
  flex-grow: 0;
}

.full-height-display {
  height: calc(100vh - 48px);
}

.colored-block {
  background-color: #089246;
  color: #fff;
  padding: 10px;
}

.slide-wrap {
  //padding: 30px;
}

.green-title {
  color: #2e6525;
  font-weight: 600;
  font-size: 18px;
}

.most-title {
  font-size: 23px;
  color: #2e6525;
}

.descr {
  font-weight: normal;
  font-size: 16px;
}

.purple-title {
  background-color: rgba(220, 137, 210, 0.29) !important;
  color: #333333 !important;
}

.purple-block {
  background-color: rgba(220, 137, 210, 0.29) !important;
  color: #FFFFFF !important;
}

.white-color {
  color: #FFF !important;
}

.light-blue-title {
  color: #00acc1;
  font-weight: 600;
  font-size: 18px;
}

.card-link {
  display: flex;
  align-items: center;
  width: 100%;
  max-width: 550px;
  cursor: pointer;
  font-size: 22px;
  text-transform: uppercase;
  justify-content: center;
  border-radius: 5px;
  border: 1px solid #e3e3e3;
  padding: 12px 20px;
}

.card-link__telegram {
  padding: 5px;
  border: 1px solid #0088CC;
  border-radius: 5px;
  color: #fff;
  background-color: #0088CC;
}

.card-link__call {
  padding: 5px;
  border: 1px solid #0088CC;
  border-radius: 5px;
  color: #fff;
  background-color: #1e931e;

  a {
    color: #fff;
    text-decoration: none;
  }
}

.card-link__invert {
  color: #fff;
  background-color: #59a34d;
}

.card-link__tabletki {
  box-shadow: 3px 3px 20px 3px rgba(89, 163, 77, 0.35);
}

.card-link__liki-24 {
  box-shadow: 3px 3px 20px 3px rgba(0, 172, 193, 0.35);
}

.nav-mobile {
  display: none !important;
}

.why-bifolak {
  padding: 15px;
  border-radius: 5px;
  max-width: 450px;
  width: 100%;
  box-shadow: 5px 5px 23px 5px rgba(57, 94, 44, 0.23);
}

.why-bifolak__count {
  font-size: 65px;
  color: #59a34d;
}

.mob-nav-item {
  text-align: left;
  padding: 10px;
  color: #59a34d;
  font-weight: 600;
}

.slick-slide img {
  max-width: 100%;
}

.v-select {
  border-radius: 3px;
}

.vs__dropdown-toggle {
  border-radius: 3px;
  border-color: #e3e3e3 !important;
  min-height: 40px;
  padding: 0 8px 4px !important;
  font-size: 14px;
}

.vs__deselect {
  fill: rgba(0,0,0,0.6);
}

.vs__dropdown-menu {
  background: #e3e3e3 !important;
}

.vs__dropdown-menu {
  background: #fff !important;
  font-weight: 500;
  max-height: 200px !important;
}

.vs__dropdown-option--selected {
  color: #59a34d !important;
}

.vs__dropdown-option--highlight {
  background: #e3e3e3 !important;
  color: #333 !important;
}

@media only screen and (max-width: 768px) {
  h2 {
    font-size: 19px;
  }

  .nav-desktop {
    display: none;
  }

  .nav-mobile {
    display: block !important;
  }
}
</style>
