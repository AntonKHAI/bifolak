<template>
  <div class="main">
    <b-navbar fixed="top" class="justify-content-between">
      <b-navbar-brand href="#">Lek Prime</b-navbar-brand>

      <b-collapse is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item>Для кого?</b-nav-item>
          <b-nav-item>Консультант по продукту</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <div class="mt-5 px-3 py-5">
      <div class="mb-5">
        <h2 class="green-title">
          БЕРЕЖНАЯ КОРРЕКЦИЯ <br>
          МИКРОФЛОРЫ ВЛАГАЛИЩА
        </h2>
      </div>
      <div class="mb-5">
        <h2>
          СУПОЗИТОРІЇ ДЛЯ ЕФЕКТИВНОГО ВІДНОВЛЕННЯ <br>
          ВАГІНАЛЬНОІ МІКРОФЛОРИ
        </h2>
      </div>
      <div>
        <img src="../assets/main.png" alt="main" style="max-width: 100%">
      </div>
    </div>
    <div class="mt-5 px-3  py-3">
      <div class="mb-5">
        <h2 class="green-title">
          В житті жінки існує багато причин, через які <br> в неї можуть виникати несприятливі зміни мікрофлори піхви
        </h2>
      </div>
      <ol class="gradient-list">
        <li><b>ЗМІНИ ГОРМОНАЛЬНОГО ФОНУ:</b> вагітність, пологи, менопауза</li>
        <li><b>ЛІКАРСЬКІ ЗАСОБИ:</b> антибіотики, гормональні препарати та ін.</li>
        <li><b>ГІНЕКОЛОГІЧНІ ЗАХВОРЮВАННЯ:</b> бактеріальний вагіноз, вагініт, кандидоз</li>
      </ol>
    </div>
    <div class="mt-5 px-3  py-3">
      <div class="mb-5">
        <h2 class="green-title">
          Зачем нужны вагинальные пробиотики
        </h2>
      </div>
      <ol class="gradient-list">
        <li>Рекомендується жінкам з проявами вагінозів та вагінітів різної етиології (кандидозних, бактеріальних, трихомонадних)</li>
        <li>При призначенні антибактеріальної, гормональної та інших видах терапії, що можуть призводити до порушення мікрофлори піхви</li>
        <li>При дизбіозі піхви у вагітних з метою підвищення якості життя цієї категорії жінок</li>
        <li>Вживають як джерело життєздатних лактобактерій з метою відновлення та збереження біоплівки, що запобігає заселенню піхви патогенною флорою</li>
        <li>Вживають як джерело лакто- та біфідобактерій з метою стимулювання імунної системи</li>
      </ol>
    </div>
    <b-container fluid>
    <b-row class="mt-5 px-3 py-3 justify-content-between">
      <b-col md="6" sm="12" class="flex justify-content-center mb-4">
        <b-card
          img-src="https://onclinic.ua/storage/media/articles/331/SwHBEBwYqgaynnsmyZ8rExh0pMmRKby9UXp11gBJ.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 35rem;"
          class="mb-2"
        >
          <b-card-text>
            Лечение и профилактика
            вагинальных дисбиозов
          </b-card-text>
        </b-card>
      </b-col><b-col md="6" sm="12" class="flex justify-content-center mb-4">
        <b-card
          img-src="https://ginokomfort.ru/upload/medialibrary/086/x0868ca29e7272cc29750e87588a14cb5.jpg.pagespeed.ic.d_tHlY-EzZ.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 35rem;"
          class="mb-2"
        >
          <b-card-text>
            Комплексное лечение:
            острых, подострых, хронических вульвитов и вагинитов, постменопаузального атрофического вагинита, бактериального вагиноза
          </b-card-text>
        </b-card>
      </b-col><b-col md="6" sm="12" class="flex justify-content-center mb-4">
        <b-card
          img-src="https://lh3.googleusercontent.com/proxy/3p1iWxX8TEF6S-TNFqhfcz7LcsWNXDw16R6fu13e3nxlRd3baN7A5WFWS9OyEkMjE5mOpfJcHQCcvd3LK9wRNtumtsA0uQNHto4IT_bW616DNcSrzA"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 35rem;"
          class="mb-2"
        >
          <b-card-text>
            Профилактика:
            послеоперационных инфекционных осложнений,
            дисбиотических изменений урогенитального тракта на фоне антибактериальной терапии
          </b-card-text>
        </b-card>
      </b-col><b-col md="6" sm="12" class="flex justify-content-center mb-4">
        <b-card
          img-src="https://uni-center.com/upload/medialibrary/468/4685a9569dbb75ef66fb88004463319c.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 35rem;"
          class="mb-2"
        >
          <b-card-text>
            Предродовая подготовка беременных женщин, входящих в группу риска в отношении воспалительных заболеваний
          </b-card-text>
        </b-card>
      </b-col>
    </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
@import url(https://fonts.googleapis.com/css?family=Montserrat:900|Raleway:400,400i,700,700i);

$main-green: '#eee';
$black: #1d1f20;
$blue: #83e4e2;
$green: #a2ed56;
$yellow: #fddc32;
$white: #fafafa;

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
      align-items: flex-end;
      @extend %boxshadow;
      content: counter(gradient-counter);
      color: $black;
      display: flex;
      font: 900 1.5em/1 'Montserrat';
      justify-content: flex-end;
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

.flex {
  display: flex !important;
}

.navbar {
  padding: .5rem 1rem;
  background-color: rgba(48, 255, 0, 0.25);
  -webkit-backdrop-filter: blur(7px);
  backdrop-filter: blur(7px);
}

.navbar-collapse {
  flex-grow: 0;
}

.full-height-display {
  height: calc(100vh - 48px);
}

.green-title {
  color: rgb(89, 163, 77);
  font-weight: 600;
}
</style>
