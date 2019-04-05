<template lang="pug">
  .wrapper
    .login
      .login__content
        button(type="button").login__form-close
        form.login__form(@submit.prevent="login")
          h1.login__form-title Авторизация
          .login__row
            app-input(
              title="Логин"
              icon="user"
              v-model="user.name"
              :errorText="validation.firstError('user.name')"
            )
          .login__row
            app-input(
              title="Пароль"
              icon="key"
              type="password"
              v-model="user.password"
              :errorText="validation.firstError('user.password')"
            )
          .login__btn
            button(
              type="submit"
              :disabled="disableSubmit"
            ).login__send-data Отправить
          .login__btn-close

    header.header
      .container.header__container
        .header__col.header__col_left
          .header__user-avatar
            img(src="../images/content/uMmrjh-M3HA.jpg" alt="User Photo").header__user-avatar-pic
          .header__user-name Дарья Марченко
          .header__desc Панель администрирования
        .header__col.header__col_right
          a(href="#").header__link-close Выйти

    nav.nav
      .container.nav__container
        ul.nav__list
          li.nav__item
            a(href="#").nav__link Обо мне
          li.nav__item
            a(href="#").nav__link Работы
          li.nav__item
            a(href="#").nav__link Отзывы
    
    .main-content
      .section.about
        .container.about__container
          .about__top
            h1.title.about__title Блок «Обо мне»  
            button(type="button").btn.about__top-btn Добавить группу

          .about__content

            .cards
              ul.cards__list
                li.cards__item.cards__item_new
                  .cards__top
                    label.cards__form-block
                      input(type="text" placeholder="Название новой группы").cards__input
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove
                  .cards__main-content
                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input.cards__input-new-skill
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn
                    
                
                li.cards__item
                  .cards__top
                    label.cards__form-block.cards__form-block-name
                      input(type="text" placeholder="Название новой группы" value="Workflow").cards__input.cards__input_title
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove

                  .cards__main-content
                    table.cards__table
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name GIT
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 100
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete
                          
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Terminal
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 90
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Gulp
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 80
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Webpack
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 85
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                    


                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn 


                li.cards__item
                  .cards__top
                    label.cards__form-block.cards__form-block-name
                      input(type="text" placeholder="Название новой группы" value="Workflow").cards__input
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove

                  .cards__main-content
                    table.cards__table
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name GIT
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 100
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete
                          
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Terminal
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 90
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Gulp
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 80
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Webpack
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 85
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                    


                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input.cards__input-new-skill
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn 
      section.works
        .container.works__container
          h1.title.works__title Блок «Работы»
          .works__content
            ul.works__content-list

              li.works__content-item.works__content-item_edit-card
                h2.title.works__new-title Редактирование работы
                form.works__form
                  .form__main-content.form__main-content_works
                    .form__col.form__col_left
                      .form__add-photo Перетащите или загрузите для загрузки изображения
                        button(type="button").form__add-photo-btn Загрузить

                    .form__col.form__col_right
                      .form__row
                        label.form__block
                          span.form__block-title.form__block-title_user Название
                          .form__block-container
                            input(type="text" placeholder="Дизайн сайта для автосалона Porsche" required).form__input.form__input_works

                      .form__row
                        label.form__block
                          span.form__block-title.form__block-title_user Ссылка
                          .form__block-container
                            input(type="text" placeholder="https://www.porsche-pulkovo.ru" required).form__input.form__input_works

                      .form__row
                        label.form__block.form__block_textarea
                          span.form__block-title.form__block-title_textarea Описание
                          .form__block-container.form__block-container_textarea
                            textarea(placeholder="Порше Центр Пулково - является официальным дилером марки Порше в Санкт-Петербурге и предоставляет полный цикл услуг по продаже и сервисному обслуживанию автомобилей").form__input_textarea
                      .form__row
                        label.form__block
                          span.form__block-title.form__block-title_user Добавление тэга
                          .form__block-container
                            input(type="text" placeholder="Jquery, Vue.js, HTML5").form__input
                      .form__row
                        ul.works__tags-list.works__tags-list_edit
                          li.works__tags-item.works__tags-item_edit HTML
                          li.works__tags-item.works__tags-item_edit CSS
                          li.works__tags-item.works__tags-item_edit Javascript
                      
                  .form__btns
                    button(type="button").form__btn-cancel Отмена
                    button(type="button").form__btn-save Сохранить

              
              li.works__content-item.works__content-item_edit-card-mobile
                h2.title.works__new-title Редактирование работы
                .works__content-top-mobile
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-preview-mobile
                  button(type="button").works__content-mobile-btn Изменить превью
                .form__row
                  label.form__block
                    span.form__block-title.form__block-title_user Название
                    .form__block-container
                      input(type="text" placeholder="Дизайн сайта для автосалона Porsche" required).form__input.form__input_works

                .form__row
                  label.form__block
                    span.form__block-title.form__block-title_user Ссылка
                    .form__block-container
                      input(type="text" placeholder="https://www.porsche-pulkovo.ru" required).form__input.form__input_works

                .form__row
                  label.form__block.form__block_textarea
                    span.form__block-title.form__block-title_textarea Описание
                    .form__block-container.form__block-container_textarea
                      textarea(placeholder="Порше Центр Пулково - является официальным дилером марки Порше в Санкт-Петербурге и предоставляет полный цикл услуг по продаже и сервисному обслуживанию автомобилей").form__input_textarea
                .form__row
                  label.form__block
                    span.form__block-title.form__block-title_user Добавление тэга
                    .form__block-container
                      input(type="text" placeholder="Jquery, Vue.js, HTML5").form__input
                .form__row
                  ul.works__tags-list.works__tags-list_edit
                    li.works__tags-item.works__tags-item_edit HTML
                    li.works__tags-item.works__tags-item_edit CSS
                    li.works__tags-item.works__tags-item_edit Javascript
                    
                .form__btns
                  button(type="button").form__btn-cancel Отмена
                  button(type="button").form__btn-save Сохранить

              li.works__content-item.works__content-item_new-card
                button(type="button").works__content-item_new-card-btn
                  span.works__content-item_new-card-title Добавить работу

              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
      section.reviews
        .container.reviews__container
          h1.title.reviews__title Блок «Отзывы»
          .reviews__new
            h2.title.reviews__new-title Новый отзыв
            form.reviews__form
              .form__main-content.form__main-content_reviews
                .form__col.form__col_left.form__col_left-reviews
                  .form__user-photo
                  button(type="button").form__user-add-photo Добавить фото

                .form__col.form__col_right
                  .form__row.form__row-reviews
                    label.form__block
                      span.form__block-title.form__block-title_user Имя автора
                      .form__block-container
                        input(type="text" placeholder="Дмитрий Ковальчук" required).form__input

                    label.form__block
                      span.form__block-title Титул автора
                      .form__block-container
                        input(type="text" placeholder="Основатель LoftSchool" required).form__input

                  .form__row
                  label.form__block.form__block_textarea
                    span.form__block-title.form__block-title_textarea Сообщение к письму
                    .form__block-container.form__block-container_textarea
                      textarea(placeholder="Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелых испытаний и бессонных ночей!").form__input_textarea
              .form__btns
                button(type="button").form__btn-cancel Отмена
                button(type="button").form__btn-save Сохранить
            
          ul.reviews__list
            li.reviews__item.reviews__item_new
              button(type="button").reviews__item_new-btn
                span.reviews__item_new-title Добавить отзыв

            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить

            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить
            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить
            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить


        


              
                  






    









</template>


<script>
import { Validator } from "simple-vue-validator";
import axios from "axios";
import appInput from "./components/input.vue";
export default {
  mixins: [require("simple-vue-validator").mixin],
  validators: {
    "user.name": value => {
      return Validator.value(value).required("Введите имя пользователя");
    },
    "user.password": value => {
      return Validator.value(value).required("Введите пароль");
    }
  },
  data() {
    return {
      disableSubmit: false,
      user: {
        name: "",
        password: ""
      }
    };
  },
  components: {
    appInput: appInput
  },
  methods: {
    async login() {
      if ((await this.$validate()) === false) return;
      this.disableSubmit = true;
      try {
        axios
          .post("//jsonplaceholder.typicode.com/posts", {
            name: this.user.name,
            password: this.user.password
          })
          .then(response => {
            const report = JSON.stringify(response, null, 2);
            console.log(report);
          });
      } catch (error) {
        console.log(error);
      }
    }
  }
};
</script>


<style lang="postcss">
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800');
@import "normalize.css";
@import "../styles/mixins.pcss";
@import "../styles/layout/base.pcss";
@import "../styles/admin/login.pcss";
@import "../styles/admin/header.pcss";
@import "../styles/admin/nav.pcss";
@import "../styles/admin/main-content.pcss";
@import "../styles/admin/about.pcss";
@import "../styles/admin/cards.pcss";
@import "../styles/admin/works.pcss";
@import "../styles/admin/reviews.pcss";
@import "../styles/admin/form.pcss";



.root-wrapper-container {
  height: 100%;
}
.header-container {
  background: linear-gradient(to right, #3e3e59, #454573);
  padding: 15px 0;
  @include phones {
    padding: 20px 0;
  }
}
.root-container {
  display: flex;
  flex-direction: column;
  height: 100%;
}
.admin-wrapper {
  display: flex;
  .maincontent {
    width: 100%;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
}
.page-title {
  margin-bottom: 60px;
  font-size: 21px;
  font-weight: bold;
}
.tooltips-container {
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 110%);
  visibility: hidden;
  transition: 0.3s;
  &.showed {
    transform: translate(-50%, 0%);
    visibility: visible;
  }
}
button {
  background: transparent;
}
/* Форма логина */
@import "../../../styles/mixins.pcss";
.login {
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background: url("~images/icons/user.svg") center center / cover no-repeat;
  &:before {
    content: "";
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    opacity: 0.5;
    background: $text-color;
  }
}
.login__form-title {
  font-size: 36px;
  text-align: center;
  font-weight: 600;
}
.login__content {
  position: relative;
  @include phones {
    height: 100%;
    width: 100%;
  }
}
.login__row {
  margin-bottom: 35px;
}
.login__btn {
  display: flex;
  width: 100%;
  padding: 0 8%;
  justify-content: center;
  
}
.login__send-data {
  width: 100%;
  padding: 30px;
  background-image: linear-gradient(to right, #ad00ed, #5500f2);
  border-radius: 40px 0 40px;
  color: #fff;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 18px;
  transition-duration: .2s;
  &[disabled] {
    opacity: 0.5;
    filter: grayscale(100%);
  }

    &:hover {
  background-image: none;
  background-color: #5500f2;
  }

  &:active {
  background-image: none;
  background-color: #5500f2;
  }

  &:focus {
  background-image: none;
  background-color: #414c63;
  }
}
.login__form {
  width: 563px;
  padding: 50px 77px 60px;
  background: #fff;
  @include phones {
    width: 100%;
    padding-right: 7%;
    padding-left: 7%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
}

.login__btn-close {
    background: svg-load("cross.svg", fill=rgba(#2d3c4e, 0.7), width=100%, height=100%);
    width: 20px;
    height: 20px;
    position: absolute;
    top: 0;
    right: 0;
    margin-top: 3%;
    margin-right: 3%;
    transition-duration: .2s;
    cursor: pointer;

    @include phones() {
    right: 45px;
    }
    &:hover {
    background: svg-load("cross.svg", fill=rgba(#5500f2, 0.7), width=100%, height=100%);
    }

    &:active {
    background: svg-load("cross.svg", fill=rgba(#5500f2, 0.7), width=100%, height=100%);
    }

    &:focus {
    background: svg-load("cross.svg", fill=rgba(#5500f2, 0.7), width=100%, height=100%);
    }
}
</style>